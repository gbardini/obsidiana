Python is [dynamically typed](https://en.wikipedia.org/wiki/Type_system#Static_and_dynamic_type_checking_in_practice). All this means is that a variable can store any type, and that type can change.

For example, if I make a number variable, I can later change that variable to a string:

This is valid:

```python
speed = 5
speed = "five"
```

## JUST BECAUSE YOU CAN DOESN'T MEAN YOU SHOULD!

In almost all circumstances, it's a _bad idea_ to change the type of a variable. The "proper" thing to do is to just create a new one. For example:

```python
speed = 5
speed_description = "five"

```

## WHAT IF IT WEREN'T DYNAMICALLY TYPED?

Languages that aren't dynamically typed are statically typed, such as Go (which you'll learn in a later course). In a statically typed language, if you try to assign a value to a variable of the wrong type, an error would crash the program.

If Python were statically-typed, the first example from before would crash on the second line, `speed = "five"`. The computer would give an error along the lines of `you can't assign a string value ("five") to a number variable (speed)`
https://www.youtube.com/watch?v=GqXpFycPWLE&embeds_referring_euri=https%3A%2F%2Fwww.boot.dev%2F

Is changing the type of a variable generally a good idea?
R: No

What kind of typing does Python employ?
R: Dynamic

[[12 - MATH WITH STRINGS]]