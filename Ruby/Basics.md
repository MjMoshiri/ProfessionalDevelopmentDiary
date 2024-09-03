# [Pickaxe Book - Programming Ruby 3.3](https://learning.oreilly.com/library/view/programming-ruby-3-3/9798888650684/)

[Ruby Evolution](https://rubyreferences.github.io/rubychanges/evolution.html)


- **Parentheses**: Not mandatory but recommended for methods.
- **`attr_reader`, `attr_accessor`**: Used to define getters and setters.
- **Variables**: Act as references to objects; use `obj.dup` to copy, and `freeze` to make an object immutable.
- **Monkey Patching**: Modifying or extending existing classes.
- **Array Syntax**: Unique array manipulations in Ruby.
  - **Examples**:
    - `a = [1, 3, 5, 7, 9]` #=> `[1, 3, 5, 7, 9]`
    - `a[2, 2] = "cat"` #=> `[1, 3, "cat", 9]`
    - `a[2, 0] = "dog"` #=> `[1, 3, "dog", "cat", 9]`
    - `a[1, 1] = [9, 8, 7]` #=> `[1, 9, 8, 7, "dog", "cat", 9]`
    - `a[0..3] = []` #=> `["dog", "cat", 9]`
    - `a[5..6] = 99, 98` #=> `["dog", "cat", 9, nil, nil, 99, 98]`
    - `a = %w[ant bee cat dog elk]` # => `["ant", "bee", "cat", "dog"]`
    - `a = %i[ant bee cat dog elk]` # => `[:ant, :bee, :cat, :dog]`
- **===** is equal to **include?**.
- **String**:
  - **#{ }**: Used to embed expressions in strings. `puts "2 + 2 = #{2 + 2}"` #=> `2 + 2 = 4`
  - Double-quoted strings allow escape sequences and interpolation.
  - **`<<`**: Appends to a string.
  - **`%q`**: Single-quoted string. e.g., `%q{This is a string}`
  - **`%Q` and `%`**: Double-quoted string. e.g., `%Q{This is a string}` it could be followed by *any* delimiter.
  - **HEREDOC**: Multiline string. e.g., `<<END_OF_STRING`. It can be used with `<<-` to ignore leading whitespace or `<<~` to ignore leading whitespace and indentation.
  - **Encoding**: `# encoding: utf-8`
  - **=~**: Matches a string with a regular expression and returns the index. `puts "cat" =~ /at/` #=> `1`
- **Loops**:
  - **`times`**: `5.times { |i| puts i }`
  - **`upto`**: `1.upto(5)`
  - **`downto`**: `5.downto(1)`
  - **`step`**: `1.step(10, 2)`
  - **`with_index`**: `1.upto(5).with_index { |i, idx| puts "#{i} - #{idx}" }`
  - **`each`**: `a.each { |i| puts i }`
  
- **Stack and Queue Operations**:
  - **`pop`**: Removes the last element.
  - **`shift`**: Removes the first element.
- **`dig` Method**:
  - Accesses nested data safely. Using `dig` prevents exceptions by returning `nil` if the path does not exist.
  - **Example**:
    - `data = { mcu: [{name: "Iron Man", year: 2010, actors: ["Robert Downey Jr.", "Gwyneth Paltrow"]}], starwars: [{name: "A New Hope", year: 1977, actors: ["Mark Hamill", "Carrie Fisher"]}] }`
    - `data[:mcu][0][:actors][1]` # => "Gwyneth Paltrow"
    - `data.dig(:mcu, 0, :actors, 1)` # => "Gwyneth Paltrow"


- **Exceptions**:
  - **`Exception`**: Base class for all exceptions. (`StandardError` is the base class for all exceptions raised by Ruby programs.)
  - **`begin` and `end`**: Used to start and end a block of code.
  - **`kernal.caller`**: Returns the current call stack. e.g., `puts caller[0]`
  - **`rescue`**: Used to handle exceptions.
  - **`ensure`**: Always executed.
  - **`retry`**: Retries the block.
  - **`raise`**: Raises an exception.
  - **`throw` and `catch`**: Used to exit a block of code.

- **FILE**:
  - **`__FILE__`**: Returns the name of the current file.
  - **`__LINE__`**: Returns the current line number.
  - **`__dir__`**: Returns the directory of the current file.
  - **`File.realpath(__FILE__)`**: Returns the absolute path of the current file.
  - You can pass ending character to each_line method. e.g., `File.open("file.txt").each_line("e") { |line| puts line }`
  - `$stdout` and `$stderr` are global variables for standard output and standard error.
**Tags**: `Ruby 3.3`
 