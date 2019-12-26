
`std::forward_as_tuple()` makes a tuple of references

C++ concurrency primitive hierarchy (3-ways to get future):

`std::async` - the most highlevel (executes somewhere, you can tell where, and returns future)
    |
    V
`std::packaged_task` - if you want to control exactly the place where it will execute, use it
    |
    V
`std::promise` - if you what to control also the what the result is passed (all above are functional objects), use it
