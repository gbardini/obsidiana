Some new developers get hung up on the difference between `print()` and `return`.

It can be particularly tricky when the test suite we provide prints the output of your functions to the console. This makes it _seem_ like `print()` and `return` are interchangeable, but they are not!

- `print()`:
    1. A function that prints a value to the console.
    2. It does NOT return a value.
- `return`:
    1. A keyword that ends the function execution.
    2. It gives the specified value back to the caller of the function.
    3. It does NOT print anything to the console.

## PRINTING TO DEBUG YOUR CODE

Printing values and running your code in the console is a great way to debug your code. You can see what values are stored in various variables, find your mistakes, and fix them. Add print statements and run your code as you go! It's a great habit to get into to make sure that each line you write is doing what you expect it to do.

In the real world it's rare to leave `print()` statements in your code once you're done debugging. Similarly, you need to remember to remove any `print()` statements from your code before submitting your work for review here on Boot.dev because it will interfere with the test suite!

## ASSIGNMENT

There is a problem in the `get_title` function! It's supposed to calculate the `title` value and `return` it to the caller. Instead, it's barbarically printing the value to the console.

Fix the function so that it returns the `title` value instead of printing it.

```python
def get_title(first_name, last_name, job):
    title = first_name + " " + last_name + " the " + job
    print(title)


# Don't touch below this line


def test(first_name, last_name, job):
    title = get_title(first_name, last_name, job)
    print("First name:", first_name)
    print("Last name:", last_name)
    print("Job:", job)
    print("Title:", title)
    print("=====================================")


test("Frodo", "Baggins", "warrior")
test("Bilbo", "Baggins", "thief")
test("Gandalf", "The Grey", "wizard")
test("Aragorn", "Son of Arathorn", "ranger")
```

## ANSWER

```python
def get_title(first_name, last_name, job):
    title = first_name + " " + last_name + " the " + job
    return title


# Don't touch below this line


def test(first_name, last_name, job):
    title = get_title(first_name, last_name, job)
    print("First name:", first_name)
    print("Last name:", last_name)
    print("Job:", job)
    print("Title:", title)
    print("=====================================")


test("Frodo", "Baggins", "warrior")
test("Bilbo", "Baggins", "thief")
test("Gandalf", "The Grey", "wizard")
test("Aragorn", "Son of Arathorn", "ranger")
```

[[13 - CHALLENGE 1 CURSE]]