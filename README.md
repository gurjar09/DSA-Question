# 1. Move all zero at the End

```python
l = [1,0,2,0,3,0,5]

pos = 0

for i in range(len(l)) :
    if l[i] != 0 :
        l[pos], l[i] = l[i], l[pos]
        pos += 1

print(l)


#2. Second Largest Element


```python
# Input list
l = [1, 2, 3, 4, 3, 42, 4, 5, 3, 3]

# Initialize with a very small value
first_largest = float('-inf')
second_largest = float('-inf')

for num in l:
    # If current number is greater than the largest
    if num > first_largest:
        second_largest = first_largest
        first_largest = num
    # If number is between first and second largest
    elif num != first_largest and num > second_largest:
        second_largest = num

print(f"First Largest: {first_largest}")
print(f"Second Largest: {second_largest}")
