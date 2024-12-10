# Next.js router.push with Query Parameters Issue

This repository demonstrates an uncommon bug encountered when using `router.push` in Next.js to redirect to the home page with query parameters. The query parameters are unexpectedly dropped from the URL.

## Bug Description

The `router.push` method in Next.js is used to redirect to a different route. When redirecting to the home page with query parameters, the query parameters are sometimes ignored, resulting in the URL not containing the expected query parameters.  This issue is more subtle and not easily reproducible in all conditions and setups.

## Reproduction Steps
1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.
5. Click the "Go Home with Query" button. Observe that the query parameter is missing from the URL.

## Solution
The solution provided addresses the issue, ensuring query parameters are correctly appended to the URL when redirecting to the homepage.

## Technologies Used
* Next.js