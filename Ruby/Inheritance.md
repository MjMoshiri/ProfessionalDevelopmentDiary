# [Pickaxe Book - Programming Ruby 3.3](https://learning.oreilly.com/library/view/programming-ruby-3-3/9798888650684/)

A Ruby class can only have one direct parent, which makes it a single-inheritance language. However, it can include the functionality of any number of mixins, providing a multiple-inheritance-like capability without the complexity.

- **Mixins (Modules)**:
  - Mixins are like partial class definitions that can be included in multiple classes.
  - They provide a way to share code among multiple classes without using classical inheritance.
    - Common Modules: Enumerable (needs `each`), Comparable (needs `<=>`)
- **include, extend, prepend**:
  - `include`: Adds instance methods from the module to the class.
  - `extend`: Adds module's methods to the class itself.
  - `prepend`: Adds module's methods to the front of the method lookup chain.

- **Lookup Chain**:
  - When a method is called on an object, Ruby looks for the method in the prepended modules first, then in the class itself, and finally in the included modules. if the method is not found, it repeats the process in the parent class till it reaches the top of the inheritance chain.
    - **method_missing, NameError**:
    - `method_missing`: Called when a method is invoked on an object and it does not exist.
    - `NameError`: Raised when a constant or method is not found and no `method_missing` is defined.

- **super**:
  - When called inside a method, Ruby looks for a method with the same name one step up the inheritance chain.

### Practical Example

```ruby
module Log
  def execute
    puts "logging"
    super
  end
end

module Caller
  def execute
    puts "calling"
    super
  end
end

class Parent
  def execute
    puts "parenting"
  end
end

class Child < Parent
  prepend Log
  include Caller

  def execute
    puts "childing"
    super
  end
end

puts Child.new.execute

# Output:
# logging
# childing
# calling
# parenting
```
