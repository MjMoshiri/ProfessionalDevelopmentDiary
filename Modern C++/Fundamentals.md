First 5 Modules of [C++20 Fundamental](https://learning.oreilly.com/course/c-20-fundamentals-with/9780136875185/) by Paul Deitel.


## General Concepts
- **Preprocessor**: Used for processing directives before actual compilation. e.g., `#include`.
- **Object File**: Compiled but not linked code snippet.
- **Garbage Value**: Uninitialized variable holding random data.

## Syntax and Features
- **println**: Will be added in C++23 for easier printing.
- **`length()` `starts_with()` `ends_with()`**: String functions for string manipulation.
- **`setprecision`**: Manipulator to set the precision of floating-point numbers. (iomanip)
- **`fixed` and `scientific`**: Manipulators to set the output format of floating-point numbers. (iostream)
- **`format` header**: For advanced output formatting. Example usage: `:>20.2f`.
- **`[[fallthrough]];`**: Indicates intentional fall-through in switch cases.
- **`using enum`**: Allows scoped enums to be used without prefix. 
- **`inline` keyword**: Recommends to declare small and time-sensitive functions as inline.
- **`boolalpha`**: Manipulator that returns values as true/false instead of 1/0. (iostream)
- **`static` keyword**: Used to declare variables that retain their values between function calls.
- **`default argument values`**: Typically specified in headers to maintain consistency.
- **Narrowing Conversion**: Causes compilation errors; e.g., `int x{12.0}`.
- **`<numbers>` header**: Provides mathematical constants. 

## Other Topics
- **Boost Library**: Uses types like `cpp_int` and `dec_float_50` for precise calculations.
- **Banker Rounding**: A rounding strategy used in financial calculations.

## Coding Practices
- **Go-style Conditional**: `if(command; condition)` for cleaner control flow.
- **Use single quotes on numbers**: Enhances readability, e.g., `1'000'000`.
- **Block for scoping `{}`**: Encourages declaring variables in the minimal necessary scope.

## Resources
- **[Open-std.org](https://open-std.org)**: Official site for C++ standards.
- **[CppCoreGuidelines](https://github.com/isocpp/CppCoreGuidelines)**: Guidelines for C++ programming.
- **[cppreference.com](https://cppreference.com)**: Specifically the headers section for detailed library information.
- **[Awesome C++](https://awesomecpp.com)**: A curated list of awesome C++ frameworks, libraries, etc.

**Tags**: `C++`, `Programming`, `Coding Standards`
