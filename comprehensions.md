### List Comprehensions
Source: [Python List Comprehensions: Explained Visually](http://treyhunner.com/2015/12/python-list-comprehensions-now-in-color/) by Trey Hunner

From ```for``` loop to ```list comprehension```

```python
numbers = [1, 2, 3, 4, 5]

doubled_odds = []
for n in numbers:
    if n % 2 == 1:
        doubled_odds.append(n * 2)
```

```python
numbers = [1, 2, 3, 4, 5]

doubled_odds = [n * 2 for n in numbers if n % 2 == 1]
```
