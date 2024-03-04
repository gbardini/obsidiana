You can create a string with dynamic values by using `f-strings` in Python. It's a beautiful syntax that I wish more programming languages used.

```python
num_bananas = 10
print(f"You have {num_bananas} bananas")
# You have 10 bananas
```

- The opening quotes must be preceded by an `f`.
- Any variables within curly brackets have their values "interpolated" (injected) into the string.

## ASSIGNMENT

Fix the bug on line 7. Use an f-string to inject the dynamic values into the string:

- Replace `NAME` with the value of the `name` variable
- Replace `RACE` with the value of the `race` variable
- Replace `AGE` with the value of the `age` variable

Do _not_ "hard-code" the values into the string. For example, this is _not_ the solution we're looking for (even though it happens to work in this case):

```python
print("Yarl is a dwarf who is 37 years old.")
```

The problem with hard coding is that it doesn't work with values that change. What if we had multiple characters?

## TIP

**Punctuation matters!** Make sure your output matches the expected output exactly.

```python
name = "Yarl"
age = 37
race = "dwarf"

# Don't edit above this line

print("NAME is a RACE who is AGE years old.")
```

## ANSWER

```python
name = "Yarl"
age = 37
race = "dwarf"

# Don't edit above this line

print(f"{name} is a {race} who is {age} years old.")
```

[[9 - NONETYPE VARIABLES]]