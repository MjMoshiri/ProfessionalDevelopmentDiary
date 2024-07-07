Chapter 9 to 12 [C++20 Fundamental](https://learning.oreilly.com/course/c-20-fundamentals-with/9780136875185/)

## C++20 Syntax
- **Designated Initializers**: `Record record{.first{"mmd"}, .last{"tg"}};` allows for direct initialization of struct members. (Should be in the order of declaration)
- **`<=>` (Spaceship Operator)**: Introduced in `<compare>` header for simplified comprehensive comparisons.


## General Syntax and Features
- **`explicit` keyword**: Enforces that constructors are only used for explicit conversions.
- **`#pragma once`**: Ensures the file is included only once in a single compilation.
- **`friend` keyword**: Allows other classes or functions special access to private and protected members.
- **`final` keyword**: Used to prevent a class from being inherited or a virtual method from being overridden.
- **`<memory>` header**: Manages memory with smart pointers like `unique_ptr`, `shared_ptr`, and `weak_ptr`.
- **Move Constructor**: Allows the resources of a temporary object to be moved rather than copied.
- **`noexcept`**: Specifies that a function does not throw exceptions.
- **Function Try Block**: Allows catching exceptions thrown from within the constructor's initializer list.

## Notes on Language Features
- **Member Initialization Order**: Follows the order of member definition in the class, not the order in the constructor.
- **Virtual Functions and Destructors**: If a class has virtual functions, it is recommended to also have a virtual destructor.
- **Core Guidelines on Memory Management**: Recommend avoiding `new` and `delete` in favor of smart pointers; ownership in `unique_ptr` is transferred when assigning to a new variable, which then assumes ownership.
- **Rule of Five**: If a class needs a custom `destructor`, `copy constructor`, `copy assignment operator`, `move constructor`, or `move assignment operator`, it should define all five.
- **Rule of Zero**: If a class does not need any of the Rule of Five functions, it should not define any of them.
- **Contracts**: Contracts are preconditions, postconditions, and assertions that can be used to specify and check the behavior of functions. [Full Details](https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2023/p2900r3.pdf)
**Tags**: `C++`, `Programming`, `Software Design`
