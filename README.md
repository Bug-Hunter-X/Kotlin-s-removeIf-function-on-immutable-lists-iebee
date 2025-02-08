# Kotlin's removeIf() function and Immutability

This example demonstrates a common error in Kotlin when using the `removeIf()` function with immutable lists. The `removeIf()` function modifies the list in place, and therefore only works with mutable lists created using `mutableListOf()`.  Attempting to use it on an immutable list (`listOf()`) will result in a compile-time error.

The solution is to either create a mutable list or use other methods appropriate for immutable lists like filtering to create a new list.