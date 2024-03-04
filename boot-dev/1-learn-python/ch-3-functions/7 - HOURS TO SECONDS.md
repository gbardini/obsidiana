## ASSIGNMENT

We need to be able to display the current time to our players. The problem is that the time is stored as a number of hours, but we want to display it as a number of seconds.

Write the `hours_to_seconds` function. It should convert `hours` to `seconds`.

## ANSWER

```python
def hours_to_seconds(h):
        seconds = h * 3600
        return seconds

def test(x):
        seconds = hours_to_seconds(x)
        print(f"{x} Hours to Seconds is: {seconds}")

test(1)
```

[[8 - NONE RETURN]]