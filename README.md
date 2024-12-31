# Next.js 15 - Invalid Hook Call Error

This repository demonstrates a strange issue encountered in Next.js 15 where a simple functional component throws an 'invalid hook call' error.  The error occurs even without any custom hooks being used, pointing towards a potential configuration or setup problem within the Next.js 15 environment.

## Steps to Reproduce

1. Clone this repository.
2. Install dependencies: `npm install`
3. Start the development server: `npm run dev`

The application will likely throw the `Error: invalid hook call` error in the browser console.

## Potential Causes and Solutions

The root cause is still under investigation. However, potential solutions to explore include:

* **Strict Mode:** Check if strict mode is improperly applied within the component or at a higher level in the component tree.
* **React Version Compatibility:** Ensure compatibility between the React version and Next.js 15.
* **Incorrect Import Statements:** While unlikely in this simple app, make sure that all necessary React components are imported correctly and not conflicting with other imports.
* **Server-Side Rendering (SSR) Issues:** Explore if there's a conflict in how the component is rendered on the server vs client side.
* **Next.js Configuration:** Review the Next.js `next.config.js` file for potential misconfigurations that might be impacting the application’s lifecycle.

The solution provided in `bugSolution.js` offers one potential workaround; however, the fundamental issue might lie deeper within the Next.js 15 setup itself.