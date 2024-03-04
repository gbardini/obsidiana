In Fantasy Quest, a weapon can be enchanted to do bonus damage.

## ASSIGNMENT

Complete the `enchant_and_attack` function. It creates a new "enchanted" name for a weapon and calculates how much damage the enchanted weapon will deal to a victim.

It accepts 3 parameters:

- `player_health`: integer
- `damage`: integer
- `weapon`: string

It should do the following things in the function body:

1. Calculate and store the "enchanted damage" in a new variable. The enchanted damage should be the input `damage` plus `10`.
2. Calculate and store the "new health" in a new variable. The new health should be the input `player_health` minus the enchanted damage.
3. Create a new variable called `enchanted_weapon`. It should be the input `weapon` with the string "enchanted " added to the beginning of it. For example:
    1. `sword` -> `enchanted sword`
    2. `axe` -> `enchanted axe`
4. Return the enchanted weapon and the new health in that order.

```python
def enchant_and_attack(player_health, damage, weapon):
    # ?


# Don't modify below this line


def test(player_health, damage, weapon):
    print("The victim has", player_health, "health.")
    print(weapon, "base damage:", damage, "Enchanting and attacking...")
    enchanted_weapon, new_health = enchant_and_attack(player_health, damage, weapon)
    print("The victim has been attacked with the", enchanted_weapon)
    print("The victim has", new_health, "health remaining.")
    print("=====================================")


def main():
    test(100, 50, "sword")
    test(500, 100, "axe")
    test(1000, 250, "bow")


main()
```

## ANSWER
```python
def enchant_and_attack(player_health, damage, weapon):
        enchanted_damage = damage + 10
        new_health = player_health - enchanted_damage
        enchanted_weapon = "enchanted " + weapon 
        return enchanted_weapon, new_health

# Don't modify below this line


def test(player_health, damage, weapon):
        print("The victim has", player_health, "health.")
        print(weapon, "base damage:", damage, "Enchanting and attacking...")
        enchanted_weapon, new_health = enchant_and_attack(player_health, damage, weapon)
        print("The victim has been attacked with the", enchanted_weapon)
        print("The victim has", new_health, "health remaining.")
        print("=====================================")


def main():
        test(100, 50, "sword")
        test(500, 100, "axe")
        test(1000, 250, "bow")


main()
```

[[1 - SCOPE]]