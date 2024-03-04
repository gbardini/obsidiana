## CHALLENGE

You've been working with a biologist who is researching the mating behaviors of fruit bats. They've added some calls to the `main` function that contain invalid syntax.

Fix the biologist's syntax error. Use the proper [delimiter](https://en.wikipedia.org/wiki/Decimal_separator#Digit_grouping) so that the numbers are still easy to parse visually.

The numbers should be:

- 8 million and 3 million
- 10 million and 4.5 million

```python
def main():
    test(8,000,000, 3,000,000)
    test(10,000,000, 4,500,000)


# Don't edit below this line


def calculate_male_ratio(num_fruit_bats, num_male_bats):
    return num_male_bats / num_fruit_bats


def test(num_fruit_bats, num_male_bats):
    ratio = calculate_male_ratio(num_fruit_bats, num_male_bats)
    print(f"{ratio * 100}% of fruit bats are male")
    print("=====================================")


main()
```

## ANSWER

```python
def main():
    test(8e6, 3e6)
    test(10e6, 4.5e5)


# Don't edit below this line


def calculate_male_ratio(num_fruit_bats, num_male_bats):
    return num_male_bats / num_fruit_bats


def test(num_fruit_bats, num_male_bats):
    ratio = calculate_male_ratio(num_fruit_bats, num_male_bats)
    print(f"{ratio * 100}% of fruit bats are male")
    print("=====================================")


main()
```

[[14 - CHALLENGE 2 CONVERTING BINARY]]