# Unhandled JSON Key Error in Dart

This repository demonstrates a common error in Dart applications when working with JSON responses from APIs. The code assumes the existence of a specific key in the JSON data without proper error handling, leading to runtime exceptions.

## The Bug
The `fetchData` function attempts to access `jsonData['some_key']` without checking if the 'some_key' key actually exists in the `jsonData` map. If the key is missing, a runtime error will occur.

## The Solution
The solution involves checking for the existence of the key before attempting to access it. This can be achieved using the `containsKey` method or optional chaining.

## How to Run
1. Clone the repository.
2. Ensure you have Dart SDK installed.
3. Run `dart bug.dart` to see the error.
4. Run `dart bugSolution.dart` to see the corrected version.