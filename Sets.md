# Assignment 5 Part 2
## Sets

### 1.Create an empty set and print it.


```python
set = {}
print(set)
```

    {}
    

### 2.Create a set of your favorite colors and print it.


```python
colors = {'red' , 'black' , 'purple' , 'voilet'}
print(colors)
```

    {'purple', 'black', 'red', 'voilet'}
    

### 3.Create a set that includes a mix of data types (integers, strings, floats).


```python
set_2 = {1,2, ('red' , 'black')}
print(set_2)
type(set_2)
```

    {1, 2, ('red', 'black')}
    




    set



### 4.Access the elements of a set using a loop and print each element.


```python
new_set = {1, 2, 3, 4, 5}
for element in new_set:
    print(element)

```

    1
    2
    3
    4
    5
    

### 5.Add a new element to a set using the add() method.


```python
numbers = {5,6,7,8,9}
adding = numbers.add(10)
print(numbers)
```

    {5, 6, 7, 8, 9, 10}
    

### 6.Add multiple elements to a set using the update() method.


```python
numbers = {5,6,7,8,9}
updating = numbers.update({10})
print(numbers)
```

    {5, 6, 7, 8, 9, 10}
    

### 7.Remove and return an arbitrary element from a set using the pop() method.


```python
numbers = {5,6,7,8,9}
removed = numbers.pop()
print(numbers)
print(removed)
print(f"Updated set: {numbers}")
```

    {6, 7, 8, 9}
    5
    Updated set: {6, 7, 8, 9}
    

### 8.Remove a specific element from a set using the remove() method.


```python
numbers = {5,6,7,8,9}
element_to_remove = 8
print(numbers)
print(element_to_remove)
print(f"Updated set: {numbers}")
```

    {5, 6, 7, 8, 9}
    8
    Updated set: {5, 6, 7, 8, 9}
    

### 9.Remove a specific element from a set using the discard() method.


```python
numbers = {5,6,7,8,9}
element_to_remove = 9
numbers.discard(element_to_remove)
print(numbers)
print(element_to_remove)
print(f"Updated set: {numbers}")
```

    {5, 6, 7, 8}
    9
    Updated set: {5, 6, 7, 8}
    

### 10.Convert a string to a set of unique characters.


```python
name = "kinza ishaq"
unique_characters = set(name)
print(unique_characters)
```

    {'a', 's', 'z', 'q', 'i', 'k', 'h', ' ', 'n'}
    

### 11.Convert a set of characters to a string.


```python
characters = {'k' , 'i' , 'n' , 'z' , 'a'}
converting = ''.join(characters)
print(converting)
type(converting)
```

    zkain
    




    str



### 12.Use the clear() method to remove all elements from a set.


```python
characters = {'k' , 'i' , 'n' , 'z' , 'a'}
removed = characters.clear()
print(characters)
```

    set()
    

### 13.Use the copy() method to create a shallow copy of a set.


```python
characters = {'k' , 'i' , 'n' , 'z' , 'a'}
copied = characters.copy()
print("characters:" ,characters)
print("copied:" ,copied)
```

    characters: {'z', 'k', 'a', 'i', 'n'}
    copied: {'z', 'k', 'a', 'i', 'n'}
    

### 14.Use the difference() method to find the difference between two sets.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
diff = set_A.difference(set_B)
print(diff)
```

    {1, 2, 3}
    

### 15.Create two sets and find their union.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
union = set_A | set_B
print(union)
```

    {1, 2, 3, 4, 5, 6, 7, 8}
    

### 16.Create two sets and find their intersection.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
intersection = set_A.intersection(set_B)
print(intersection)
```

    {4, 5}
    

### 17.Create two sets and find their difference.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
minus = set_A - set_B
print(minus)
```

    {1, 2, 3}
    

### 18.Create two sets and find their symmetric difference.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
symmetric_difference = set_A.symmetric_difference(set_B)
print(symmetric_difference)

```

    {1, 2, 3, 6, 7, 8}
    

### 19.Check if one set is a subset of another.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
set_subset = set_A <= set_B
print(set_subset)
```

    False
    

### 20.Check if one set is a superset of another.


```python
set_A = {1,2,3,4,5}
set_B = {4,5,6,7,8}
set_superset = set_A >= set_B
print(set_superset)
```

    False
    

### 21.Check if two sets are disjoint (have no common elements).


```python
set_A = {1,2,3}
set_B = {4,5,6,7,8}
set_disjoint = set_A.isdisjoint(set_B)
print(set_disjoint)
```

    True
    


```python

```
