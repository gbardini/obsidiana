# CURSE

An enemy's weapons can be cursed so that they don't deal as much damage.

## ASSIGNMENT

Complete the `curse` function. It accepts a `weapon_damage` parameter and returns two values:

1. The `lesser_cursed` damage: 50% of the input `weapon_damage`.
2. The `greater_cursed` damage: 25% of the input `weapon_damage`.

A greater curse is more powerful than a lesser curse, so it reduces the damage more.

## TIP

You can multiply a number by a decimal to get a percentage of a number. For example:

30% of 50 is `50 * 0.3`

Ignore the `float` function in the `print` statements. We will introduce [floats](https://en.wikipedia.org/wiki/Floating-point_arithmetic) later.

```python
def curse(weapon_damage):
    # ?


# Don't modify below this line


def test(weapon_damage):
    print("Weapon's base damage:", float(weapon_damage))
    print("Cursing...")
    lesser_cursed, greater_cursed = curse(weapon_damage)
    print("With lesser curse the damage is:", float(lesser_cursed), "damage.")
    print("With greater curse the damage is:", float(greater_cursed), "damage.")
    print("=====================================")


def main():
    test(100)
    test(500)
    test(1000)


main()
```

## ANSWER

```python
def curse(weapon_damage):
        lesser_cursed = weapon_damage * 0.5
        greater_cursed = weapon_damage * 0.25
        return lesser_cursed, greater_cursed

# Don't modify below this line


def test(weapon_damage):
        print("Weapon's base damage:", float(weapon_damage))
        print("Cursing...")
        lesser_cursed, greater_cursed = curse(weapon_damage)
        print("With lesser curse the damage is:", float(lesser_cursed), "damage.")
        print("With greater curse the damage is:", float(greater_cursed), "damage.")
        print("=====================================")


def main():
        test(100)
        test(500)
        test(1000)


main()
```

[[14 - CHALLENGE 2 ENCHANT AND ATTACK]]