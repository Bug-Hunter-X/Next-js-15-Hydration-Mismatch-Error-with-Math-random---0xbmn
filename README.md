# Next.js 15 Hydration Mismatch Bug

This repository demonstrates a common hydration mismatch error in Next.js 15 applications and provides a solution.

The error occurs when using dynamic values in client components without proper handling.  The server renders the component with a placeholder, and the client-side renders it with a different value, causing a mismatch. 

## Steps to Reproduce
1. Clone the repository.
2. Install dependencies: `npm install`
3. Run the development server: `npm run dev`
4. Navigate to `/about`.
5. You will see the hydration mismatch error in your browser's console. 

## Solution
The solution involves moving the dynamic value calculation to the client side, using useEffect hook.