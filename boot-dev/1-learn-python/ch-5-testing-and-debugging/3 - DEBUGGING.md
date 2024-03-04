When you're working as a professional developer, you'll typically write code on your computer and test it by yourself before it's deployed to users.

That first part of the process is called _debugging_. You write some code, run it, and if it doesn't work, you fix the bugs. You repeat this process until you're confident that your code works as expected.

## RUN VS SUBMIT

At Boot.dev, the `Run` button is for debugging. The `Submit` button mimics the idea of publishing your code for production use.

You should be debugging your code using the `Run` button. You should be adding `print()` statements to your code to make sure it's doing what you think it's doing at different points in the code.

- Write a line to calculate a value
- `print()` the value you calculated
- Run the code
- Did it print what you expected? If not, fix it
- Repeat

You will never lose XP or be penalized on Boot.dev for using the run button. However, there are consequences for submitting broken code, just like there are career consequences for pushing broken code to your users!

## THE SUBMIT BUTTON WILL RUN ADDITIONAL TESTS

When you use the `Run` button, a few tests will run against your code. However, the `Submit` button will run _additional_ tests that you're not able to debug against. That's what keeps it fun and realistic (it's so hard to know what your users will do with your code!).

## ASSIGNMENT

Complete the `take_magic_damage` function. It should return the new `health` after calculating how much magic-type damage the player takes. Here is a description of the arguments:

- `health`: The player's starting health
- `resist`: The player's magic resistance. This reduces the damage they take by a static amount
- `amp`: The attacker's magic amplification. This increases the damage they deal by a multiplier
- `spell_power`: The base damage of the spell

First, calculate the total maximum damage to be inflicted by multiplying the `spell_power` by the `amp`. Then, subtract the `resist` from the total damage to get the actual damage dealt. Apply that damage to the player's health and `return` the new health.

main.py
```python
def take_magic_damage(health, resist, amp, spell_power):
    pass
```

main_test.py
```python
from main import *

run_cases = [
    (100, 5, 2, 20, 65),
    (200, 10, 1, 25, 185),
]

submit_cases = run_cases + [
    (0, 0, 0, 0, 0),
    (1, 1, 1, 1, 1),
    (100, 2, 3, 1, 99),
    (2500, 3, 2, 2, 2499),
]


def test(input1, input2, input3, input4, expected_output):
    print("---------------------------------")
    print(f"Inputs: {input1}, {input2}, {input3}, {input4}")
    print(f"Expecting: {expected_output}")
    result = take_magic_damage(input1, input2, input3, input4)
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
def take_magic_damage(health, resist, amp, spell_power):
    new_health = health - ((spell_power * amp) - resist) 
    return new_health

print(take_magic_damage(100, 10, 1, 25));
```

[[4 - LEARNING EFFECTIVELY]]