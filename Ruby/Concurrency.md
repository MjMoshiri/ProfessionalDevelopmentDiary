# [Pickaxe Book - Programming Ruby 3.3](https://learning.oreilly.com/library/view/programming-ruby-3-3/9798888650684/)


- **GIL**: Global Interpreter Lock (like Python).
- **[Thread](https://docs.ruby-lang.org/en/3.3/Thread.html)**: `priority`, `status`, `abort_on_exception`, `alive?`, `Thread.current[:varName]`
- **system**: `system("echo 'Hello World'")` returns `true` if the command was successful.
- **spawn**: `spawn("echo 'Hello World'")` returns the process ID.
- **IO.popen**: `IO.popen("echo 'Hello World'")` returns an IO object. Check I mean why??? for more info.
- **[Process](https://docs.ruby-lang.org/en/3.3/Process.html)** : `trap`, `wait`, `fork`
- **[Fiber](https://docs.ruby-lang.org/en/3.3/fiber_md.html)**: Coroutine

- **[Ractor](https://docs.ruby-lang.org/en/3.3/ractor_md.html)**: Parallelism in Ruby. (Ruby 3.0) `send`, `receive`, `yield`, `take`, `receive_if`

**Tags**: `Ruby 3.3`, `Concurrency`

