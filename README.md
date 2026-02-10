# 1. Move all zero at the End

```python
l = [1,0,2,0,3,0,5]

pos = 0

for i in range(len(l)) :
    if l[i] != 0 :
        l[pos], l[i] = l[i], l[pos]
        pos += 1

print(l)
