Variables are called "variables" because they can hold any value and that value can change (it varies).

For example, the following will print `20`:

```python
acceleration = 10
acceleration = 20
print(acceleration)
```

The line `acceleration = 20` _reassigns_ the value of `acceleration` to 20. It _overwrites_ whatever was being held in the `acceleration` variable before.

## ASSIGNMENT

We need to reduce our hero's health as they take damage in the game.

Before each `print()` function in the provided code, change the value of `player_health` to 100 _less_ than it was before.

```python
player_health = 1000

# reduce by 100 here

print(player_health)

# and here

print(player_health)

# and here

print(player_health)

# and here

print(player_health)
```

## ANSWER


```python
player_health = 1000

# reduce by 100 here
player_health = player_health - 100
print(player_health)

# and here
player_health = player_health - 100
print(player_health)

# and here
player_health = player_health - 100
print(player_health)

# and here
player_health = player_health - 100
print(player_health)
```

[[3 - LET'S DO SOME MATH]]