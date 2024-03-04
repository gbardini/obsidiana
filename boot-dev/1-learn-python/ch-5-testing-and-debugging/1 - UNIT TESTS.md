# UNIT TESTS

Up until this point, all the coding lessons you've completed have been testing you based on your code's _console output_ (what's printed). For example, a lesson might expect your code (in conjunction with the code we provide) to `print` something like:

```bash
Armor: 2
Health: 18
```

If your code prints that _exact_ output, you pass. If it doesn't, you fail.

## A NEW TYPE OF LESSON

Going forward, you'll encounter a new type of lesson: [unit tests](https://en.wikipedia.org/wiki/Unit_testing). A unit test is just an automated program that tests a small "unit" of code. Usually just a function or two. The editor will have tabs: the "main.py" file containing your code, and the "main_test.py" file containing the unit tests.

These new unit-test-style lessons will test your code's _functionality_ rather than its output. Our tests will call functions in your code with different arguments, and expect certain return values. If your code returns the correct values, you pass. If it doesn't, you fail.

There are two reasons for this change:

1. It's more realistic. In the real world, you'll be writing unit tests and running them against your code to make sure it works as expected.
2. You can run and debug your code with `print` statements, and leave those print statements in when you submit. Unlike the output-based lessons, you won't have to remove your `print` statements to pass.

## ASSIGNMENT

Complete the `total_xp` function. It accepts two integers as input:

- `level`
- `xp_to_add`

There are 100 xp per level. `total_xp` should convert the current `level` to xp, then add this current xp to the `xp_to_add` argument and return the player's total xp. For example:

- If a player is level 1 and gains 100 xp, they have 200 total xp.
- If a player is level 2 and gains 250 xp, they have 450 total xp.
- If a player is level 170 and gains 590 xp, they have 17590 total xp.

## TIPS

- The `pass` keyword is a way to tell Python to do nothing. You'll need to replace it with your own code.
- Take a look at the `main_test.py` file at the top of your editor. You can read the tests but you can't edit them.

main.py
```python
def total_xp(level, xp_to_add):
    pass
```

main_test.py
```python
from main import *

run_cases = [
    (1, 200, 300),
    (2, 50, 250),
]

submit_cases = run_cases + [
    (0, 0, 0),
    (0, 200, 200),
    (176, 350, 17950),
    (250, 100, 25100),
]


def test(input1, input2, expected_output):
    print("---------------------------------")
    print(f"Inputs: {input1}, {input2}")
    print(f"Expecting: {expected_output}")
    result = total_xp(input1, input2)
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

## ANSWER
main.py

```python
def total_xp(level, xp_to_add):
    current_xp = level * 100
    return current_xp + xp_to_add
```

[[2 - TWO LESSON TYPES]]