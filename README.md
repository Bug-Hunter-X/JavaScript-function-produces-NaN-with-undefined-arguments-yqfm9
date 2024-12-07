# JavaScript Function NaN Issue

This repository demonstrates a common issue in JavaScript functions where using `undefined` values can lead to `NaN` results unexpectedly.  The `foo` function is designed to handle `null` values gracefully, but it doesn't properly manage `undefined`. This can cause unexpected behavior in applications if not carefully handled.

## Bug Report

The `foo` function adds two numbers. It's designed to return `null` if either input is `null`. However, if either input is `undefined`, it returns `NaN`.

## Solution

The solution addresses this by explicitly checking for both `null` and `undefined` values. This provides more robust error handling and predictable results.