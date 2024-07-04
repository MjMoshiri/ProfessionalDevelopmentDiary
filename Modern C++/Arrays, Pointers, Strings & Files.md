Chapters 6 to 8 [C++20 Fundamental](https://learning.oreilly.com/course/c-20-fundamentals-with/9780136875185/)

## C++20 Features
- **`<ranges>` header**: Lazy generation features like `count_if`, `view::iota`, `view::filter`, and `view::transform`.
- **`<span>` header**: Can receive built-in arrays, vectors, standard arrays, or any contiguous iterable collections. used for passing arrays to functions in safer ways.
- **`to_array`**: Converts aggregate data into a `std::array`.

## General Syntax and Features
- **`string_view`**: Used for read-only string operations.
- **`constexpr`**: Allows variables to be initialized at compile time.
- **`:02d`**: Fills with zeros if the number is smaller than two characters.
- **`|` (Pipeline Operation)**: Used in conjunction with range views for functional style transformations.
- **`ex.what()`**: Used to retrieve a string describing the exception.
- **`int* const` vs. `const int*`**: Differentiates between constant pointer to mutable data and mutable pointer to constant data.
- **Alignment**: `<` for left-aligned and `>` for right-aligned text.
- **`seekg`, `seekp`, `tellg`, `tellp`**: Functions for positioning and querying position in streams.
- **`quoted(name)`**: From C++14, simplifies output of strings that include spaces or special characters.
- **Raw String Literal**: Represents string literals that contain multiple lines or escape characters naturally.

## Notes on Language Features
- **Static Variables**: Initialized to default values if not explicitly set.
- **Argument Deduction in Templates (since C++17)**: Simplifies template usage by automatically determining types.
- **`<numeric>` header functions**: Includes functions like `accumulate` for operations on data sequences.
- **Built-in Arrays**: Limited capabilities, such as no knowledge of their own size, non-assignable, and lack of automatic bounds checking.
- **Pointer Usage**: Should point to a single element rather than an array.
- **String Literal Concatenation**: If only whitespace separates two string literals, the compiler will merge them; useful for multiline strings for better readability.

**Tags**: `C++`, `Programming`, `Coding Standards`
