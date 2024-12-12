# Expo Camera Flash Inconsistency

This repository demonstrates a bug in the Expo Camera API where the flash mode is set correctly, but the captured image is consistently underexposed. This issue occurs intermittently, making it difficult to track down and reproduce reliably.

## Bug Report

The primary issue involves using a custom flash mode with the Expo Camera API. Despite correctly setting the flash mode, images are often captured without the flash firing, resulting in poorly lit photos.  The inconsistency makes debugging and finding a consistent solution challenging.

## Steps to Reproduce

1. Clone this repository.
2. Run the app using Expo Go.
3. Attempt to take multiple pictures. Note that some pictures may show proper flash behavior, while others will appear underexposed.

## Expected Behavior

The flash should always fire when a custom flash mode (e.g., `on`) is selected.

## Actual Behavior

The flash fires inconsistently.  Images are often captured without flash activation, regardless of the configured flash mode.

## Solution

The solution file `bugSolution.js` includes some strategies that you can try to improve the flash behavior.
