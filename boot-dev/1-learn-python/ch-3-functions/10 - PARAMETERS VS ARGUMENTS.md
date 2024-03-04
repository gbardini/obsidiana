Parameters are the names used for inputs when _defining_ a function. Arguments are the names of the inputs supplied when a function is _called_.

To reiterate, arguments are the actual values that go into the function, say `42.0`, `"the dark knight"`, or `True`. Parameters are the names we use in the function definition to refer to those values, which at the time of writing the function, could be anything.

That said, it is important to understand that this is all semantics, and frankly developers are really lazy with these definitions. You'll often hear the words arguments and parameters used interchangeably.

```python
# a and b are parameters
def add(a, b):
    return a + b

# 5 and 6 are arguments
sum = add(5, 6)
```

[[11 - DEFAULT VALUES FOR FUNCTION ARGUMENTS]]