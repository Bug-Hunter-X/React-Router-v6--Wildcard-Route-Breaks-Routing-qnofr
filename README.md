# React Router v6 Wildcard Route Bug

This repository demonstrates a subtle bug in React Router v6 related to wildcard routes ('/*').  The issue occurs when a wildcard route is defined, even if it's not nested and doesn't have any child routes. This can lead to routing issues where other routes are not properly matched.

## Reproduction

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the app: `npm start`
4. Observe that navigation to `/about` might not work as expected.  The wildcard route interferes with the route matching process.

## Solution

The solution involves careful consideration of route ordering and potentially avoiding the use of wildcard routes unless absolutely necessary.  The solution branch demonstrates a way to resolve this specific problem.