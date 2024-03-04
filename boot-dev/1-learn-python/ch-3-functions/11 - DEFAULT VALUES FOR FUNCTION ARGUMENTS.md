Python has a way to specify a [default](https://docs.python.org/3/glossary.html#term-parameter) value for function arguments. This can be convenient if a function has arguments that are essentially "optional", and you as the function creator want to use a specific default value in case the caller doesn't provide one.

A default value is created by using the assignment (`=`) operator in the function signature.

```python
def get_greeting(email, name="there"):
    print("Hello", name, "welcome! You've registered your email:", email)
```

```python
get_greeting("lane@example.com", "Lane")
# Hello Lane welcome! You've registered your email: lane@example.com
```

```python
get_greeting("lane@example.com")
# Hello there welcome! You've registered your email: lane@example.com
```

If the second parameter is omitted, the default `"there"` value will be used in its place. As you may have guessed, for this structure to work, optional arguments that have defaults specified come _after_ all the required arguments.

## ASSIGNMENT

Complete both the `get_punched` and `get_slashed` functions. They should each take 2 arguments:

- `health`: An integer
- `armor`: An integer

Change the functions so if no `armor` argument is passed, `armor` `default`s to `0`.

Each attack does a different amount of damage. Getting punched does 50 damage. Getting slashed does 100 damage. The armor should absorb some of the attack by subtracting from the damage. The rest of the damage should be applied to the health. Return a single integer, the health left over after the attack.

```python
def get_punched(health, armor):
    # ?


def get_slashed(health, armor):
    # ?


# Don't touch below this line


def test(health, armor):
    print(f"Health: {health}, Armor: {armor}")
    print(f"Health after punch: {get_punched(health, armor)}")
    print("=====================================")
    print(f"Health: {health}, Armor: {armor}")
    print(f"Health after slash: {get_slashed(health, armor)}\n")
    print("=====================================")
    print(f"Health: {health}, Armor: no armor!")
    print(f"Health after slash: {get_slashed(health)}\n")
    print("=====================================")
    print(f"Health: {health}, Armor: no armor!")
    print(f"Health after punch: {get_punched(health)}")
    print("=====================================")


test(400, 5)
test(300, 3)
test(200, 1)
```

## ANSWER

```python
def get_punched(health, armor=0):
        damageTaken = 50 - armor
        totalHealth = health - damageTaken
        return totalHealth

def get_slashed(health, armor=0):
        damageTaken = 100 - armor
        totalHealth = health - damageTaken
        return totalHealth

# Don't touch below this line


def test(health, armor):
        print(f"Health: {health}, Armor: {armor}")
        print(f"Health after punch: {get_punched(health, armor)}")
        print("=====================================")
        print(f"Health: {health}, Armor: {armor}")
        print(f"Health after slash: {get_slashed(health, armor)}\n")
        print("=====================================")
        print(f"Health: {health}, Armor: no armor!")
        print(f"Health after slash: {get_slashed(health)}\n")
        print("=====================================")
        print(f"Health: {health}, Armor: no armor!")
        print(f"Health after punch: {get_punched(health)}")
        print("=====================================")


test(400, 5)
test(300, 3)
test(200, 1)
```

[[12 - PRINTING VS RETURNING]]