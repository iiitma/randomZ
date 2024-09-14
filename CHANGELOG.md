# Changelog

All notable changes to this project will be documented in this file.

## [2.0.0] - 2024-09-14

### Breaking Changes

- **Function Renaming**: 
  - `int()` is now `integer()`
  - `array()` is now `pick()`
  
- **Updated Functionality**: 
  - **`integer(min: number = 0, max: number = 100): number`**: Throws an error if `min` is greater than `max`.
  - **`float(min: number = 0, max: number = 100, precision: number = 2): number`**: Throws an error if `precision` is negative.
  - **`pick<T>(arr: T[]): T | null`**: Returns `null` if the array is empty.
  - **`sample<T>(arr: T[], count: number): T[]`**: Throws an error if `count` exceeds the length of `arr`.

### New Features

- **Enhanced Randomization Methods**:
  - **`integer()`**: Generates a random integer between `min` and `max`.
  - **`float()`**: Generates a random float between `min` and `max` with precision.
  - **`intArray()`**: Generates an array of random integers.
  - **`floatArray()`**: Generates an array of random floats with precision.
  - **`pick()`**: Picks a single random element from an array.
  - **`sample()`**: Picks a specified number of non-repeating elements from an array.
  - **`shuffle()`**: Shuffles the elements in an array.
  - **`string()`**: Generates a random string of specified length.

- **Improved Error Handling**: More precise error messages for invalid inputs.

### Bug Fixes

- **Enhanced Validation**: Added thorough runtime validation to ensure correct inputs.

## [1.1.1] - 2021-06-25

Initial release.