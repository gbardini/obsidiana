When no return value is specified in a function, it will automatically return `None`. For example, maybe it's a function that prints some text to the console, but doesn't explicitly return a value. The following code snippets all return the same value, `None`:

```python
def my_func():
    print("I do nothing")
    return None
```

```python
def my_func():
    print("I do nothing")
    return
```

```python
def my_func():
    print("I do nothing")
```

[[9 - MULTIPLE RETURN VALUES]]