# React Router Dom v6 Nested Routes Issue

This repository demonstrates an unexpected route matching behavior in React Router Dom v6 when using nested routes with parameters. The route `/users/:id` unexpectedly matches even when the URL is `/about`, leading to incorrect component rendering.

## Problem
The issue arises when a route with parameters is placed alongside other routes without specific path matching.  The parameterized route seems to have a higher precedence than it should, even overlapping with other routes. 

## Solution
The solution involves using the `useParams` hook correctly and ensuring that route paths are specific enough to prevent unintended matches.  The solution also includes improved error handling for cases where a parameter is not found or is malformed.  Adding more specific paths prevents the issue of unexpected route matching.