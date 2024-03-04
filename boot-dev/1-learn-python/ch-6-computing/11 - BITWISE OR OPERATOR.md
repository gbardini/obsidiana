As you may have guessed, the bitwise `OR` operator is similar to the bitwise `AND` operator in that it works on binary rather than boolean values. However, the bitwise `OR` operator `OR`s the bits together. Here's an example:

- `0101` is 5
- `0111` is 7

```
0101
|
0111
=
0111
```

A `1` in binary is the same as `True`, while `0` is `False`. So a bitwise operation is just a bunch of logical operations that are completed in tandem. When two binary numbers are `OR`ed together, the result has a `1` in any place where _either_ of the input numbers has a `1` in that place.

`|` is the bitwise `OR` operator in Python. `5 | 7 = 7` and `5 | 2 = 7` as well!

```
0101 = 5
|
0010 = 2
=
0111 = 7
```
## HOW PERMISSIONS WORK WITH PARTIES AND GUILDS

A "party" is a team of 2-4 players who are online at the same time and fighting together. A "guild" is a larger group of players, sometimes 50 or 60, who share a common purpose.

We've been asked to add some more functionality to the "guild permissions" system. When players from a guild are in a party together, they should _all_ gain _all_ of the guild permissions of all the other members of the party!

For example, if Jack has the "create" permission, and Jill has the "delete" permission, then when they are in a party together, Jack and Jill should both have the "create" and "delete" permissions.

## ASSIGNMENT

Complete the `calculate_party_perms` function. It should return a binary number that represents the permissions of _all_ the members of the party (Glorfindel, Galadriel, Elendil and Elrond).

Use bitwise `OR` operations to calculate the [superset](https://www.youtube.com/watch?v=1wsF9GpGd00) of all the permissions.

## ANSWER

```python
def calculate_party_perms(glorfindel, galadriel, elendil, elrond):
    return glorfindel | galadriel | elendil | elrond
```

[[12 - NOT]]