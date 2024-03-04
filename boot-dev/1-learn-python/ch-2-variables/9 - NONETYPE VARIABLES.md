Not all variables have a value. We can declare an "empty" variable by setting it to [None](https://docs.python.org/3/library/constants.html#None).

```python
empty = None
```

The value of `empty` in this instance is `None` until we use the assignment operator, `=`, to give it a value.

## NONE IS NOT A SPECIFIC STRING

Note that the [NoneType](https://docs.python.org/3/library/types.html#types.NoneType) is _not_ the same as a string with a value of "None":

```python
my_none = None # this is a None-type
my_none = "None" # this is a string
```

## ASSIGNMENT

Declare a variable named `enemy` and set it to `None`. Don't change the `print()` function.

```python
# create the empty "enemy" variable here


# don't touch below this line
print(enemy is None)
```

## ANSWER

```python
# create the empty "enemy" variable here
enemy = None

# don't touch below this line
print(enemy is None)
```

[[10 - NONETYPE]]