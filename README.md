# Unexpected Behavior of removeIf with Concurrent Modification in Kotlin

This repository demonstrates an uncommon issue in Kotlin involving the `removeIf` function on collections. When used improperly, it can lead to unexpected behavior and subtle bugs.

The `bug.kt` file shows a basic example where `removeIf` is used to remove even numbers from a list and a map. Although this appears straightforward, the underlying mechanism can cause issues when handling larger datasets or complex scenarios involving concurrent modifications.

The `bugSolution.kt` file demonstrates safer ways to handle such removals.

## How to Reproduce
1. Clone this repository.
2. Open `bug.kt` and run the code. Observe the output. The output looks correct, but the key is to understand the issues involved.
3. Open `bugSolution.kt` and run the code. Notice the different approaches, which are less prone to subtle errors.