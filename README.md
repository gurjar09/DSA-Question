# DSA-Questions

## 1. Move all zeros to the End

---

### Python Solution

```python
l = [1, 0, 2, 0, 3, 0, 5]

# Track the position to swap non-zero elements
pos = 0

for i in range(len(l)):
    if l[i] != 0:
        # Swap current element with the element at 'pos'
        l[pos], l[i] = l[i], l[pos]
        pos += 1

print(l)
# Output: [1, 2, 3, 5, 0, 0, 0]
```

---

## 2. Second Largest Element

---

### Python Solution

```python
# Input list
l = [1, 2, 3, 4, 3, 42, 4, 5, 3, 3]

# Initialize with negative infinity
first_largest = float('-inf')
second_largest = float('-inf')

for num in l:
    if num > first_largest:
        second_largest = first_largest
        first_largest = num
    elif num != first_largest and num > second_largest:
        second_largest = num

print(f"First Largest: {first_largest}")
print(f"Second Largest: {second_largest}")
```

---

## 3. Remove duplicate from the sorted list/array.

---

```python

# remove duplicate from the sorted list

l = [1,1,2,2,2,3,4,4,5]
dup = None
i = 0
while i < len(l) :
    if dup == l[i] :
        l.pop(l[i])
    else :
        dup = l[i]
        i += 1

print(l)
```
