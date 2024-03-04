In Python there are several basic [data types](https://en.wikipedia.org/wiki/Data_type).

## STRING TYPE

"Strings" are raw text in coding speak. They are called "strings" because they are a list of characters strung together. Strings are declared in Python by using single quotes or double quotes. That said, for consistency's sake, we prefer double quotes.

```python
name_with_single_quotes = 'boot.dev'
name_with_double_quotes = "boot.dev"
```

## NUMERIC TYPES

Numbers aren't surrounded by quotes when created, but they can have decimals and negative signs.

### INTEGERS ARE NUMBERS WITHOUT A DECIMAL

```python
x = 5
y = -5
```

### A "FLOAT" IS A NUMBER WITH A DECIMAL

```python
x = 5.2
y = -5.2
```

## BOOLEAN TYPE

```python
0 = False
1 = True
```

```python
is_tall = True
```

## ASSIGNMENT

Fix the bugs in the code to move on. `player_health` should be an integer and `player_has_magic` should be a boolean.

```python
player_health = "100"

player_has_magic = "True"

# don't touch below this line
print(f"player_health is a/an {type(player_health)}")
print(f"player_has_magic is a/an {type(player_has_magic)}")
```

## ANSWER

```python
player_health = 100

player_has_magic = True

# don't touch below this line
print(f"player_health is a/an {type(player_health)}")
print(f"player_has_magic is a/an {type(player_has_magic)}")
```

[[8 - F-STRINGS IN PYTHON]]