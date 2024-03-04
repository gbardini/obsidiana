So far we've been working in the global scope. That means that when we define a variable or a function, that name is accessible in _every other place_ in our program, even within other functions.

For example:

```python
pi = 3.14

def get_area_of_circle(radius):
    return pi * radius * radius
```

Because `pi` was declared in the parent "global" scope, it is usable within the `get_area_of_circle()` function.

## ASSIGNMENT

Let's change how we are calculating our player's stats! The only thing we should need to define globally is the character level and then let our functions do the rest!

Declare the variable `player_level` at the top of the global scope and set it to `4`.

```python
# ?


def calculate_health(modifier):
    return player_level * modifier


def calculate_primary_stats(armor_bonus, modifier):
    return armor_bonus + modifier + player_level


# Don't touch below this line

print(f"Character has {calculate_health(10)} max health.")

print(f"Character has {calculate_primary_stats(3, 8)} primary stats.")

```

## ANSWER

```python
# ?
player_level = 4

def calculate_health(modifier):
    return player_level * modifier


def calculate_primary_stats(armor_bonus, modifier):
    return armor_bonus + modifier + player_level


# Don't touch below this line

print(f"Character has {calculate_health(10)} max health.")

print(f"Character has {calculate_primary_stats(3, 8)} primary stats.")

```

[[1 - UNIT TESTS]]