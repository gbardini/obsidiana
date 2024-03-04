A stack trace (or "traceback") is a scary-looking error message that the Python interpreter prints to the console when it encounters certain problems. Stack traces are most common (at least for you right now) when you're trying to run invalid Python code.

You need to get used to figuring out scary error messages as a programmer. We might as well start now.

## ASSIGNMENT

Go ahead and run the code in its current state. You should see something like this:

```
PythonError: Traceback (most recent call last):
  File "<exec>", line 5, in <module>
  File "<string>", line 1, in <module>
  File "/home/pyodide/main.py", line 3
    msg = f"You have {strength} strength, {wisdom} wisdom, and {dexterity} dexterity for a total of {total} stats.
                                                                                                                  ^
IndentationError: unindent does not match any outer indentation level
```


1. `PythonError: Traceback (most recent call last):`

This is a standard header that's just letting us know that a Python traceback is what we're looking at.

2. `File "<exec>", line 5, in <module>` and `File "<string>", line 1, in <module>`

This is the start of the "trace". These strange `"<exec>"` and `"<string>"` files don't really exist, the Python interpreter is letting us know about them because they have to do with how your code is executed in a virtual browser-based environment.

3. `File "/home/pyodide/main.py", line 3`

Now we're getting to the real meat of the error message! The purpose of a "trace" is to show us the path that the Python interpreter took through our code before it encountered the error, which can help us figure out what went wrong.

In this case, the interpreter was executing the code in the `main.py` file, and it got to line 3 before it encountered the error.

4. `msg = f"You have {strength} strength, {wisdom} wisdom, and {dexterity} dexterity for a total of {total} stats.`

This is the line of code that caused the error.

5. `IndentationError: unindent does not match any outer indentation level`

This is the type of error that was raised. In this case, it's an `IndentationError`, which means that the Python interpreter was expecting a certain amount of indentation (whitespace at the beginning of the line) but it didn't get what it was expecting.

**Don't be fooled!** The proper amount of indentation in Python is 4 spaces (or one `<tab>` stroke). In this case, line 2 is actually indented 6 spaces, which is why the interpreter is confused. Fix line 2.

Run the code again. You should see another error, this time the last few lines are something like:

```
msg = f"You have {strength} strength, {wisdom} wisdom, and {dexterity} dexterity for a total of {total} stats.
                                                                                                 ^
SyntaxError: unterminated string literal (detected at line 3)
```

Now we have a `SyntaxError`, which is just a more general type of error related to invalid code. Take a close look at line 3 and fix the problem.

```python
def create_stats_message(strength, wisdom, dexterity):
      total = strength + wisdom + dexterity
    msg = f"You have {strength} strength, {wisdom} wisdom, and {dexterity} dexterity for a total of {total} stats.
    return msg

```

```python
from main import *

run_cases = [
    (1, 2, 3, "You have 1 strength, 2 wisdom, and 3 dexterity for a total of 6 stats."),
    (2, 4, 2, "You have 2 strength, 4 wisdom, and 2 dexterity for a total of 8 stats."),
]

submit_cases = run_cases + [
    (
        10,
        50,
        100,
        "You have 10 strength, 50 wisdom, and 100 dexterity for a total of 160 stats.",
    ),
    (0, 0, 0, "You have 0 strength, 0 wisdom, and 0 dexterity for a total of 0 stats."),
    (1, 1, 1, "You have 1 strength, 1 wisdom, and 1 dexterity for a total of 3 stats."),
]


def test(input1, input2, input3, expected_output):
    print("---------------------------------")
    print(f"Inputs: {input1}, {input2}, {input3}")
    print(f"Expecting: {expected_output}")
    result = create_stats_message(input1, input2, input3)
    print(f"Actual: {result}")
    if result == expected_output:
        print("Pass")
        return True
    print("Fail")
    return False


def main():
    passed = 0
    failed = 0
    for test_case in test_cases:
        correct = test(*test_case)
        if correct:
            passed += 1
        else:
            failed += 1
    if failed == 0:
        print("============= PASS ==============")
    else:
        print("============= FAIL ==============")
    print(f"{passed} passed, {failed} failed")


test_cases = submit_cases
if "__RUN__" in globals():
    test_cases = run_cases

main()
```