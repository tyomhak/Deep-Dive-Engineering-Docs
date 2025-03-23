[Solution link](https://github.com/tyomhak/EngineeringDeepDive/tree/main/Cpp/04/hw)

1. Get **volume** of [`multi_array`](4.2%20Multidimensional%20Array.md), by adding`static constexpr int volume`, which will contain the total number of cells in this structure.
2. Access by index to `multi_array`. Implement `multi_array_accessor` template, which will take a multi_array and a variadic pack of indices as arguments, and return the value at the indices.
3. update the `getter` structure for  [tuple](4.3%20Tuple.md), such that we get compile error during index overflow.