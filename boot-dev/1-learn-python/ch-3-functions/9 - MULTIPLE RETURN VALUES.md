In Python, we can return more than one value from a function.

First, we can return multiple values on one line by separating them with commas.

```python
# returns email, age, and status of the user
def get_user():
    return "name@domain.com", 21, "active"
```

Second, when we _call_ this function, we need to assign all the returned values to an equal number of variables by separating them with commas. The values will be assigned according to the order they are returned.

```python
# sets email, age, and status to values returned from get_user() function
email, age, status = get_user()
print(email, age, status)
# name@domain.com 21 active
```

## ASSIGNMENT

Complete the `become_warrior` function. It accepts 3 inputs:

- `first_name`: string
- `last_name`: string
- `power`: integer

It should return 2 values:

1. First, a string of this format: "`first_name` `last_name` the warrior"
2. Second, the `power` input after adding `1` to it.

For example:

```python
title, power = become_warrior("Aang", "Airbender", 100)
print(title)
# "Aang Airbender the warrior"
print(power)
# 101
```

## TIP

You can use the `+` operator to [concatenate](https://en.wikipedia.org/wiki/Concatenation#:~:text=In%20formal%20language%20theory%20and,concatenation%20is%20a%20primitive%20notion.) strings together. For example:

```python
first_name = "Aang"
last_name = "Airbender"
full_name = first_name + " " + last_name
print(full_name)
# "Aang Airbender"
```

```python
def become_warrior(first_name, last_name, power):
    # ?


# Don't edit below this line


def main():
    test("Frodo", "Baggins", 5)
    test("Bilbo", "Baggins", 10)
    test("Gandalf", "The Grey", 9000)


def test(first_name, last_name, power):
    title_string, power = become_warrior(first_name, last_name, power)
    print(title_string, "has a power level of:", power)


main()
```

## ANSWER

```python
def become_warrior(first_name, last_name, power):
        title = first_name + " " + last_name + " the warrior"
        totalPower = power + 1
        return title, totalPower

# Don't edit below this line


def main():
    test("Frodo", "Baggins", 5)
    test("Bilbo", "Baggins", 10)
    test("Gandalf", "The Grey", 9000)


def test(first_name, last_name, power):
    title_string, power = become_warrior(first_name, last_name, power)
    print(title_string, "has a power level of:", power)


main()
```

[[10 - PARAMETERS VS ARGUMENTS]]