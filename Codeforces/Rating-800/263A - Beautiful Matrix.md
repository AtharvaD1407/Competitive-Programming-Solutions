# Python
```python
rowNo, colNo = 0, 0

for i in range(1, 6):
    row = list(map(int, input().split()))
    if 1 in row:
        rowNo = i
        colNo = row.index(1) + 1
        break

moves = abs(rowNo - 3) + abs(colNo - 3)

print(moves)
```

<hr>

# C++
```c++
```
