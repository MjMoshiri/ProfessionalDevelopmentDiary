# [Pickaxe Book - Programming Ruby 3.3](https://learning.oreilly.com/library/view/programming-ruby-3-3/9798888650684/)


- **`block_given?`**: Checks if a block is provided to the method. `block_given? ? yield : "No block given"`.
- **`yield` Keyword**: Passes control from the method to the block given. 
- **Procs and Lambdas**:
  - **Proc**: Created with `Proc.new` or `proc`, and called with `.call`.
  - **Stabby Lambda**: Uses `->` syntax. Example: `bo = ->(param) { puts "You called me with #{param}" }`.
- **Splat (`*`)**: Used to handle variable number of arguments. `def varargs(arg1, *rest)`.
- **Double Splat (`**`)**: Used for keyword arguments. `def keywords(arg1:, arg2:)`.
- **Ampersand (`&`)**: Typically used to pass a block to a method. `def my_method(&block)`.
- **Triple Dot (`...`)**: Passes all arguments to another method. `def my_method(...); other_method(...); end`.
- **`<<` Syntax**: Often used for appending elements to a collection. `a = [1, 2, 3]; a << 4`.
- **Redefined Methods**: Ruby issues a warning But, redefines the method if it's defined more than once.
- **Keyword Arguments in Methods**:
  - Defined with names and used with specific keys. Example: `method_with_keywords(city:, state:, zip:)`.
  - Requires either an argument in the call or a default value; otherwise, an `ArgumentError` is raised.
- **!** at the end of a method name typically indicates a method that modifies the receiver.
```ruby
  print "(t)imes or (p)lus: "
  operator = gets
  print "number: "
  number = Integer(gets)
  method = number.method(operator.start_with?("t") ? :* : :+)
  puts (1..10).map(&method).join(", ")
```


### [Enumerators](https://docs.ruby-lang.org/en/master/Enumerator.html)
- **`to_enum`**: Converts an iterable to an Enumerator.
- **`:each_slice`**: Part of the Enumerable module to iterate over a collection in slices. `(1..10).each_slice(3) { |slice| p slice }` prints `[1, 2, 3]`, `[4, 5, 6]`, `[7, 8, 9]`, `[10]`.
- **`Enumerator.produce`**: Creates an Enumerator with a block that generates the next value.
- **`Enumerator::Lazy`**: Allows creating lazy enumerators for potentially infinite series.

```ruby
triangular_numbers = Enumerator.produce([1, 2]) do |number, count|
    [number + count, count + 1]
end
5.times { print triangular_numbers.next.first, " " }
```
**Tags**: `Ruby 3.3`