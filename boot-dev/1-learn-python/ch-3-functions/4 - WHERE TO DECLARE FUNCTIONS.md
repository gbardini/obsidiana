You've probably noticed that a variable needs to be declared _before_ it's used. For example, the following doesn't work:
```python
print(my_name)
my_name = 'Lane Wagner'
```

It needs to be:

```python
my_name = 'Lane Wagner'
print(my_name)
```

Lines of code execute in _order from top to bottom_, so a variable needs to be created before it can be used. That means that if you define a function, you can not call that function until after the definition.

The `main()` function is a convention used in many programming languages to specify the entry point of an application. By defining a single `main` function, and only calling `main()` at the end of the entire program we ensure that all of our functions are defined _before_ they're called.

## ASSIGNMENT

There is a bug in our program! Fix it.

```python
main()


def main():
    print("Fantasy Quest is booting up...")
    print("Game is running!")
```

## ANSWER

```python
def main():
    print("Fantasy Quest is booting up...")
    print("Game is running!")

main()
```

[[5 - ORDER OF FUNCTIONS]]