# Silent Image Load Failure in Expo

This repository demonstrates a common, yet elusive bug in Expo's `Image` component: silent image load failures.  The image fails to load without providing a clear error message, making debugging challenging.  This example shows the problem and a solution.

## Problem

The `Image` component from Expo may fail to load images silently.  No error is thrown, and there are no helpful logs. The image simply doesn't appear.

## Solution

The solution involves using a `try...catch` block to handle potential errors during the image load process, along with more robust error handling within the image source URI.