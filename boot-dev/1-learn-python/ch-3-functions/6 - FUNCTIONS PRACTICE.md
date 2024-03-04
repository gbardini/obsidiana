## CONVERSION FORMULA

`celsius = 5/9 * (fahrenheit-32)`

## ASSIGNMENT

In Fantasy Quest, as characters are running around the map they can lose health due to heat exhaustion. The game tracks the temperature in Fahrenheit, but we need to display the temperature in Celsius for players outside the US.

Write a function called `to_celsius` that returns the temperature converted from Fahrenheit to Celsius.

## ANSWER

```python
## Write a function called `to_celsius` that returns the temperature converted from Fahrenheit to Celsius.

def to_celsius(f):
        celsius = (f - 32) / 1.8
        return celsius

def test(x):
        celsius_convert = to_celsius(x)
        print(f"The value of {x} FAHRENHEiT to Celsius is {celsius_convert}")

test(1)
```

[[7 - HOURS TO SECONDS]]