Functions allow us to _reuse_ and _organize_ code. For example, say we've written some code that calculates the area of a circle:

```python
radius = 5
area = 3.14 * radius * radius
```

That works! The problem is when we want to calculate the area of _more_ circles, each with its own radius. We could just copy the code and change the variable names like this:

```python
radius = 5
area1 = 3.14 * radius * radius

radius2 = 7
area2 = 3.14 * radius2 * radius2
```

But don't we want to reuse our code? Why would we want to repeat our work? What if we wanted to calculate the area of thousands of circles??? **That's where functions help.**

Instead, we can define a new function called `area_of_circle` using the `def` keyword.

```python
def area_of_circle(r):
    pi = 3.14
    result = pi * r * r
    return result
```

The `area_of_circle` function takes one input and returns one output. The body of the function is indented and contains the code that will be run when the function is called. The `return` keyword tells the function to return the value that follows it as the output of the function.

To ["call"](https://en.wikibooks.org/wiki/Python_Programming/Functions#Function_Calls) this function ("call a function" is a fancy phrase that just means "use a function") we can now pass in any number as the input (in this case, the radius), and capture the output into a new variable:

```python
area = area_of_circle(5)
print(area)
# 78.5
```

`5` goes in as the input, `r`, the result is calculated, and `78.5` comes out as the output. Because the function is already defined, we can use it again and again with different inputs:

```python
area = area_of_circle(6)
print(area)
# 113.04
```

## ASSIGNMENT

We need to calculate the size of a weapon's "attack area". With a `1.0` meter sword, for example, a player can attack in an area of `3.14` square meters around them. You can use the `area_of_circle` function to do that calculation.

Fix the bug on line 13.

The `spear_area` variable should be set to the result of calling the `area_of_circle` function with the given `spear_length` as input.

```python
def area_of_circle(radius):
    pi = 3.14
    area = pi * radius * radius
    return area


sword_length = 1.0
spear_length = 2.0

# don't touch above this line

sword_area = area_of_circle(sword_length)
spear_area = 0

# don't touch below this line

print("Sword length:", sword_length, "meters.")
print("Sword attack area:", sword_area, "square meters")

print("Spear length:", spear_length, "meters.")
print("Spear attack area:", spear_area, "square meters")
```

## ANSWER

```python
def area_of_circle(radius):
    pi = 3.14
    area = pi * radius * radius
    return area


sword_length = 1.0
spear_length = 2.0

# don't touch above this line

sword_area = area_of_circle(sword_length)
spear_area = area_of_circle(spear_length)

# don't touch below this line

print("Sword length:", sword_length, "meters.")
print("Sword attack area:", sword_area, "square meters")

print("Spear length:", spear_length, "meters.")
print("Spear attack area:", spear_area, "square meters")
```

[[2 - FUNCTION REVIEW]]