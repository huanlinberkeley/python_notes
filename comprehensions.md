# List Comprehensions
Source: [Python List Comprehensions: Explained Visually](http://treyhunner.com/2015/12/python-list-comprehensions-now-in-color/) by Trey Hunner

### Conditional loop list comprehension

For loop:
```python
numbers = [1, 2, 3, 4, 5]

doubled_odds = []
for n in numbers:
    if n % 2 == 1:
        doubled_odds.append(n * 2)
```

List comprehension:
```python
numbers = [1, 2, 3, 4, 5]

doubled_odds = [n * 2 for n in numbers if n % 2 == 1]
```

Result
```python
double_odds = [2, 6, 10]
```

### Nested loop list comprehension

For loop:
```python
matrix = [[1, 2], [3, 4], [5, 6]]

flattened = []
for row in matrix:
    for n in row:
        flattened.append(n)
```

List comprehension:
```python
matrix = [[1, 2], [3, 4], [5, 6]]

flattened = [n for row in matrix for n in row]
```

Result
```python
flattened = [1, 2, 3, 4, 5, 6]
```

### Set comprehension

For loop:
```python
words = ["Hi", "this", "is", "an", "example"]

first_letters = set()
for w in words:
    first_letters.add(w[0])
```

List comprehension:
```python
words = ["Hi", "this", "is", "an", "example"]

first_letters = {w[0] for w in words}
```

Result
```python
first_letters = {'H', 'i', 'e', 'a', 't'}
```

### Dictionary comprehension

For loop:
```python
original = {'k1':'v1', 'k2':'v2'}

flipped = {}
for key, value in original.items():
    flipped[value] = key
```

List comprehension:
```python
original = {'k1':'v1', 'k2':'v2'}

flipped = {value: key for key, value in original.items()}
```

Result
```python
flipped = {'v1':'k1', 'v2':'k2'}
```

