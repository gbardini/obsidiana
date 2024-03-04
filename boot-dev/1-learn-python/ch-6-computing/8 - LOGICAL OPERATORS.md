You're probably familiar with the logical operators `and` and `or`.

Logical operators deal with [boolean values](https://en.wikipedia.org/wiki/Boolean_data_type), `True` and `False`.

The logical `and` operator requires that _both_ inputs are `True` to return `True`. The logical `or` operator only requires that _at least one_ input is `True` to return `True`.

For example:

```
True and True == True
True and False == False
False and False == False

True or True == True
True or False == True
False or False == False
```
## PYTHON SYNTAX

```python
print(True and True)
# prints True

print(True or False)
# prints True
```
## NESTING WITH PARENTHESES

We can nest logical expressions using parentheses.

```python
print((True or False) and False)
```

First, we evaluate the expression in the parentheses, `(True or False)`. It evaluates to `True`:

```python
print(True and False)
```

`True and False` evaluates to `False`:

```python
print(False)
```

So, `print((True or False) and False)` prints "False" to the console.

[[9 - BINARY NUMBERS]]