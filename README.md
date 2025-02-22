# Expo ImagePicker Crash with Multiple Image Selection

This repository demonstrates a bug in the Expo ImagePicker library where selecting multiple images can lead to application crashes or freezes. The issue is inconsistent and may manifest as a native module error or a runtime exception.

## Bug Description

When using `ImagePicker.launchImageLibraryAsync` with `mediaTypes: ImagePicker.MediaTypeOptions.All` and `selectionLimit: > 1`, selecting multiple images can cause the application to crash or freeze. The error messages are inconsistent and vary depending on the platform and device.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run the app using Expo Go.
4. Select multiple images using the ImagePicker.
5. Observe the crash or freeze.

## Solution

The provided solution involves using the `ImagePicker.showImagePicker` API with handling for a variety of edge cases, including memory and performance optimization, to improve robustness and stability.