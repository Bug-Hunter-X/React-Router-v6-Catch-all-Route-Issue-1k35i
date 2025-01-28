# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other routes, preventing proper navigation.  The catch-all route is incorrectly activated even when other routes match.

## Problem
The `/*` route is intended to handle any unmatched paths, but it's inappropriately overriding other more specific routes.

## Solution
The issue can be solved by ensuring that the catch-all route (`/*`) is placed last in the `Routes` component.  This ensures that other routes are checked before it.