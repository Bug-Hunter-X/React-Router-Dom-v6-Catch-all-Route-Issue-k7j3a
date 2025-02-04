# React Router Dom v6 Catch-all Route Issue

This repository demonstrates an uncommon issue with catch-all routes (`/*`) in React Router Dom v6.  The catch-all route is inappropriately matching, even when more specific routes should be matched.

## Problem
The provided `App.js` demonstrates a simple React Router setup.  However, the catch-all route (`/*`) always matches, overriding the other routes, even if the URL matches a specific path like `/about`.

## Solution
The `AppSolution.js` file provides the solution to this problem.  The issue is resolved by ensuring the catch-all route is placed last in the `Routes` component.