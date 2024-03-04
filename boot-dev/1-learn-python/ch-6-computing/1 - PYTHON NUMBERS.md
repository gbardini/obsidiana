In Python, numbers without a decimal point are called `Integers` - just like they are in mathematics.

Integers are simply whole numbers, positive or negative. For example, `3` and `-3` are both examples of integers.

Arithmetic can be performed as you might expect:

## ADDITION

```python
2 + 1
# 3
```

## SUBTRACTION

```python
2 - 1
# 1
```

## MULTIPLICATION

```python
2 * 2
# 4
```

## DIVISION

```python
3 / 2
# 1.5 (a float)
```

This one is actually a bit different - division on two integers will actually produce a [float](https://docs.python.org/3/tutorial/floatingpoint.html). A `float` is, as you may have guessed, the number type that allows for decimal values.

## ASSIGNMENT

Complete the missing sections of the `calculate_damage` function.

- Fix the `total_damage` variable so that it contains the sum of all the different weapons' damage values.
- Fix the `average_damage` variable so that it contains the _[average](https://en.wikipedia.org/wiki/Average)_ weapon damage.
main.py
```python
def calculate_damage(sword, arrow, spear, dagger, fire):
    total_damage = 0
    average_damage = 0
    return total_damage, average_damage
```

```python
from main import *

run_cases = [
    (3, 5, 2, 1, 4, (15, 3.0)),
    (5, 5, 5, 5, 5, (25, 5.0)),
]

submit_cases = run_cases + [
    (1, 2, 3, 4, 5, (15, 3.0)),
    (0, 0, 0, 0, 10, (10, 2.0)),
    (0, 0, 0, 0, 0, (0, 0.0)),
    (10, 20, 30, 40, 50, (150, 30.0)),
    (2, 2, 2, 2, 2, (10, 2.0)),
    (1, 1, 1, 1, 1, (5, 1.0)),
]


def test(sword, arrow, spear, dagger, fire, expected_output):
    print("---------------------------------")
    print(f"Inputs: {sword}, {arrow}, {spear}, {dagger}, {fire}")
    print(f"Expecting: {expected_output}")
    result = calculate_damage(sword, arrow, spear, dagger, fire)
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

```python
def calculate_damage(sword, arrow, spear, dagger, fire):
    total_damage = sword + arrow + spear + dagger + fire
    average_damage = total_damage / 5
    return total_damage, average_damage
```

[[2 - NUMBERS REVIEW]]