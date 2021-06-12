### 1. [Opposite number](https://www.codewars.com/kata/56dec885c54a926dcd001095)
```python
def opposite(number):
    return number - 2 * number
```

### 2. [Even or Odd](https://www.codewars.com/kata/53da3dbb4a5168369a0000fe)
```python
def even_or_odd(number):
    if number % 2 == 0:
        return "Even"
    else: return "Odd"
```

### 3. [Vovel Count](https://www.codewars.com/kata/54ff3102c1bad923760001f3)

```python
def get_count(input_str):
    num_vowels = 0
    for letter in input_str:
        if letter in ["a", "e", "i", "o", "u"]:
            num_vowels += 1
    return num_vowels
```

### 4. [Disemvowel Trolls](https://www.codewars.com/kata/52fba66badcd10859f00097e)

```python
def disemvowel(string_):
    string = "".join(symbol for symbol in list(string_) if symbol not in "aouieAIOUE") 
    return string
```

### 5. [Get the Middle Character](https://www.codewars.com/kata/56747fd5cb988479af000028)

```python
def get_middle(s):
    middle = len(s) // 2
    return s[middle-1:middle+1] if len(s) % 2 == 0 else s[middle]
```

### 6. [All star code challenge](https://www.codewars.com/kata/5863f97fb3a675d9a700003f)

```python
def sum_ppg(playerOne, playerTwo):
    return sum(player["ppg"] for player in [playerOne, playerTwo])
```

### 7. [Who likes it?](https://www.codewars.com/kata/5266876b8f4bf2da9b000362)

```python
def likes(names):
    number_of_names = len(names)
    if number_of_names == 0:
        return "no one likes this"
    elif number_of_names == 1:
        return f"{names[0]} likes this"
    elif number_of_names == 2:
        return f"{names[0]} and {names[1]} like this"
    elif number_of_names == 3:
        return f"{names[0]}, {names[1]} and {names[2]} like this"
    else: 
        others = str(number_of_names-2)
        return f"{names[0]}, {names[1]} and {others} others like this"
```

### 8. [Array.diff](https://www.codewars.com/kata/523f5d21c841566fde000009)

```python
def array_diff(a, b):
    for b_num in b:
        while b_num in a:
            a.pop(a.index(b_num))
    return a
```

### 8. [All star code challenge #22](https://www.codewars.com/kata/5865cff66b5699883f0001aa/)

```python
def to_time(seconds):
    hours = seconds // 3600
    minutes = (seconds - hours * 3600) // 60
    return f"{hours} hour(s) and {minutes} minute(s)"
```


