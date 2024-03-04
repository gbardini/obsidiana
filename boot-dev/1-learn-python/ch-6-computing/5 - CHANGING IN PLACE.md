It's fairly common to want to change the value of a variable based on its current value.

```python
player_score = 4
player_score = player_score + 1
# player_score now equals 5
```

```python
player_score = 4
player_score = player_score - 1
# player_score now equals 3
```

Don't let the fact that the expression `player_score = player_score - 1` is not a valid mathematical expression be confusing. _It doesn't matter_, it _is valid code_. It's valid because the way the expression should be read in English is:

> Assign to player_score the old value of player_score minus 1

## ASSIGNMENT

Complete the `update_player_score` function. It should add `increment` to `current_score` and then return the new `current_score`.

## ANSWER

```python
def update_player_score(current_score, increment):
    current_score = current_score + increment
    return current_score
```

[[6 - PLUS EQUALS]]