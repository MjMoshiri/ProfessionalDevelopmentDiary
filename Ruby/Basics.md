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
- **Stack and Queue Operations**:
  - **`pop`**: Removes the last element.
  - **`shift`**: Removes the first element.
- **`dig` Method**:
  - Accesses nested data safely. Using `dig` prevents exceptions by returning `nil` if the path does not exist.
  - **Example**:
    - `data = { mcu: [{name: "Iron Man", year: 2010, actors: ["Robert Downey Jr.", "Gwyneth Paltrow"]}], starwars: [{name: "A New Hope", year: 1977, actors: ["Mark Hamill", "Carrie Fisher"]}] }`
    - `data[:mcu][0][:actors][1]` # => "Gwyneth Paltrow"
    - `data.dig(:mcu, 0, :actors, 1)` # => "Gwyneth Paltrow"

**Tags**: `Ruby 3.3`
