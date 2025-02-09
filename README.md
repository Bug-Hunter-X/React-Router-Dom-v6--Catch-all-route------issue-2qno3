# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router v6. The catch-all route unexpectedly matches the root path (`/`), preventing other routes from rendering correctly.

## Problem
The provided `App.js` contains a catch-all route that incorrectly intercepts all navigation, including the root path. This leads to the 'Not Found' component always being displayed.

## Solution
The solution, demonstrated in `AppSolution.js`, involves using an order-sensitive approach. The catch-all route is placed after all other specific routes, ensuring it only matches when no other route matches.  In addition, more precise path matching is employed in order to prevent issues in certain route patterns.