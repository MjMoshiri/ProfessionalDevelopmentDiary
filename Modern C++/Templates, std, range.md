# Chapter 13 to 15 [C++20 Fundamental](https://learning.oreilly.com/course/c-20-fundamentals-with/9780136875185/)

## C++20 Syntax
- **`contains()`**: Check if a container has a certain element. (bool)
- **Contiguous Iterator**: Provides direct access to the memory sequence in containers.
- **`ranges::copy`**: Copies elements from one range to another.
- **`ranges::equal_range`**: Finds the range of elements matching a specific value.
- **`ranges::remove`**: Moves elements that should be removed to the end of the range; combine with `erase` for actual removal.
- **`requires` clause**: A way to express constraints on template arguments directly in the function signature.
- **`<concepts>` header**: Provides a set of standard concepts like `std::regular` and `std::totally_ordered`.

## General Syntax and Features
- **`reduce()`**: Similar to `accumulate` but not ordered, enhancing parallelism.
- **`valarray`**: Class designed for more efficient mathematical operations.
- **`list.remove(item)`**: Removes all occurrences of an item; `erase` is used for remove based on iterator.
- **`set.equal_range()`**: Finds the bounds of a sub-range that matches a given value.
- **`extract`** (C++17): Extracts nodes from associative containers.
- **`const_cast`**: Casts away the constness of variables.
- **`std::get<i>(tuple)`**: Accesses the i-th element of a tuple.
- **`consteval`**: Ensures that a function is evaluated at compile time.
- **`if constexpr`** (C++17): Conditional compilation based on constant expressions.

## Notes on Language Features
Useful for understanding the new features and syntax in C++20.
- [C++ Containers Overview](https://en.cppreference.com/w/cpp/container)
- [Named Requirements in C++](https://en.cppreference.com/w/cpp/named_req)
- [C++ Concepts](https://en.cppreference.com/w/cpp/concepts)
- [Plan for C++23 Ranges](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2020/p2214r0.html)

**Tags**: `C++`, `Advanced Programming`, `Software Design`
