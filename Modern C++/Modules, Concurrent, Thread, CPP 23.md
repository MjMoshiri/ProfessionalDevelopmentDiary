# Chapter 16 to 20 (Final) [C++20 Fundamental](https://learning.oreilly.com/course/c-20-fundamentals-with/9780136875185/)

## C++20 Syntax
- **Jthreads**: Provides a high-level threading facility.
  - **`stop_token`**: Allows thread interruption.
  - **`stop_callback`**: Registers callbacks that are called upon stop requests.
- **`latch`**: A synchronization barrier that allows one-time coordination between threads.
- **`barrier`**: A reusable synchronization barrier.
- **`semaphore`**: Limits the number of threads that can access a resource or pool of resources concurrently. Simplifies the process of managing shared resources.
- **Coroutines**: `co_await`, `co_yield`, `co_return`

## C++23 Syntax
- **`println()` and `print()`**: Functions for simplified output.
- **`ranges::to`**: Converts a range into a container of elements.
- **Other New Ranges Functions**: `contains`, `starts_with`, `ends_with`, ...
- **`views::zip`** and **`views::zip_transform`**: Combine multiple ranges.
- **`enumerate`**: Simplifies the process of iterating over containers with index.
- **`flat_map`** and **`flat_set`** : a container adaptor that gives the functionality of an associative container that contains key-value pairs with unique keys.
- **`stacktrace` header**: Provides utilities for capturing and manipulating stack traces.

## General Syntax and Features
- **`future`** and **`promise`**: Mechanisms for asynchronous computing.
- **`variant`** and **`visit`**: Provides a type-safe union.
- **`mutable`**: Object can be modified even if the function is `const`.
- **`decltype`**: Deduces the type of an expression.
- **`[[nodiscard("with reason")]]`**: Warns when the result of a function is discarded. (e.g. when `string.empty()` is mistakenly called with the purpose of clearing the string.)

## Notes on Language Features
- Learn all about C++ string formatting capabilities inspired by Python at [C++ Format String Syntax](https://en.cppreference.com/w/cpp/utility/format/formatter).
- **Diamond Inheritance**: Utilize virtual inheritance to solve issues with diamond-shaped inheritance hierarchies.
- Avoid the `using` directive in header files to prevent namespace pollution.

**Tags**: `C++20`, `C++23`, `Advanced Programming`, `Software Design`
