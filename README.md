# React Router DOM v6 Catch-all Route '*' Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router DOM v6. The catch-all route should only match if no other routes match, but in this example it always matches, regardless of the URL.

## Problem

The `/*` route in `App.js` is intended to act as a 404 Not Found page. However, it always matches, even when navigating to `/` or `/about`.

## Solution

The solution is to ensure that the catch-all route is placed at the end of your route definitions within the `Routes` component as shown in `AppSolution.js`.