All functions _must_ be defined before they're used.

You might think this would make structuring Python code hard because the order of the functions needs to be just right. As it turns out, there's a simple trick that makes it super easy.

Most Python developers solve this problem by defining _all_ the functions in their program first, then finally calling the "entry point" function _last_. Conventionally this "entry point" function is usually called `main` to keep things simple and consistent.

If you follow this pattern you can forget about ordering. All of the functions have been read by the Python interpreter before the first one is called.

```python
def main():
    health = 10
    armor = 5
    add_armor(health, armor)

def add_armor(h, a):
    new_health = h + a
    print_health(new_health)

def print_health(new_health):
    print(f"The player now has {new_health} health")

# call entrypoint last
main()
```

[[6 - FUNCTIONS PRACTICE]]