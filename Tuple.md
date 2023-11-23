# Assignment 5 Part(1) 
## Tuple

### 1.Create an empty tuple and print it. 


```python
empt_tup = ()
print(empt_tup)
```

    ()
    

### 2.Create a tuple of your favorite fruits and print it.


```python
fruits = ('guava' , 'grapes' , 'plum')
print(fruits)
```

    ('guava', 'grapes', 'plum')
    


```python
type(fruits)
```




    tuple



### 3.Create a tuple that includes a mix of data types (integers, strings, floats).


```python
mix_data = (23, 23.5 , ('a' , 'b' , 'c'))
print(mix_data)
```

    (23, 23.5, ('a', 'b', 'c'))
    


```python
type(mix_data)
```




    tuple



### 4.Access the first element of a tuple.


```python
first = fruits[0]
print(first)
```

    guava
    

### 5.Access the last element of a tuple.


```python
last = fruits[2]
print(last)
```

    plum
    

### 6.Access the second and third elements of a tuple.


```python
tuple_data = (1,2,3,4,5)
print(tuple_data)
second = tuple_data[1]
print(second)
third = tuple_data[2]
print(third)
```

    (1, 2, 3, 4, 5)
    2
    3
    

### 7.Slice a tuple to extract the first three elements.


```python
tuple_data = (1,2,3,4,5)
extract = tuple_data[:3]
print(extract)
```

    (1, 2, 3)
    

### 8.Slice a tuple to extract the last three elements.


```python
tuple_data = (1,2,3,4,5,6,7,8,9,10)
extracting = tuple_data[-3:]
print(extracting)
```

    (8, 9, 10)
    

### 9.Slice a tuple to get every second element.


```python
tuple_data = (1,2,3,4,5,6,7,8,9,10)
get = tuple_data[1::2]
print(get)
```

    (2, 4, 6, 8, 10)
    

### 10.Reverse a tuple using slicing.


```python
tuple_data = (1,2,3,4,5,6,7,8,9,10)
reverse = tuple_data[::-1]
print(reverse)
```

    (10, 9, 8, 7, 6, 5, 4, 3, 2, 1)
    

### 11.Create two tuples and concatenate them.


```python
tuple_1 = ('a' , 'b' , 'c' )
tuple_2 = (1,2,3)
concatenate = (tuple_1 + tuple_2)
print(concatenate)
```

    ('a', 'b', 'c', 1, 2, 3)
    

### 12.Repeat a tuple multiple times using the repetition operator.


```python
tuple_1 = ('a' , 'b' , 'c' )
repeat = tuple_1*5
print(repeat)
```

    ('a', 'b', 'c', 'a', 'b', 'c', 'a', 'b', 'c', 'a', 'b', 'c', 'a', 'b', 'c')
    

### 13.Find the index of a specific element in a tuple using the index() method.


```python
tuple_1 = ('a' , 'b' , 'c' )
indexing = tuple_1.index('b')
print(indexing)
```

    1
    

### 14.Count the number of occurrences of a specific element in a tuple using the count() method.


```python
data = (1,2,3,3,3,3,3,4,5,6,7,8,9,10)
print(data)
counting = data.count(3)
print(counting)
```

    (1, 2, 3, 3, 3, 3, 3, 4, 5, 6, 7, 8, 9, 10)
    5
    

### 15.Sort a tuple of numbers in ascending order.


```python
numbers = (6,9,0,1,6,9,6,2,5,8)
print(numbers)
sorting = sorted(numbers)
print(sorting)
```

    (6, 9, 0, 1, 6, 9, 6, 2, 5, 8)
    [0, 1, 2, 5, 6, 6, 6, 8, 9, 9]
    

### 16.Sort a tuple of strings in alphabetical order.


```python
fruits = ('guava' , 'grapes' , 'plum' , 'apple' , 'mango')
print(fruits)
sorting = sorted(fruits)
print(sorting)
```

    ('guava', 'grapes', 'plum', 'apple', 'mango')
    ['apple', 'grapes', 'guava', 'mango', 'plum']
    

### 17.Sort a tuple of tuples based on the second element of each inner tuple.


```python
multi_tuples = ((9, 4), (1, 6), (0, 3))
sorted_tuple = tuple(sorted(multi_tuples, key=lambda x: x[1]))
print(sorted_tuple)

```

    ((0, 3), (9, 4), (1, 6))
    

### 18.Compare two tuples to see if they are equal in both value and identity.


```python
tup_1 = (1,2,3,4,5)
tup_2 = (1,3,5,7)
equal = tup_1==tup_2
print(equal)
identity = tup_1 is tup_2
print(identity)
```

    False
    False
    

### 19. Create a shallow copy of a tuple and observe the effects of modifying one of the tuples.


```python
Orig_Tup = ([5,8,3], 'i', 'z', 'k')
shallow_copy = tuple(Orig_Tup)
print(Orig_Tup)
print(shallow_copy)
Orig_Tup[0][0] = 45
print("\nAfter Modification:")
print("Orig_Tup:", Orig_Tup)
print("shallow_copy:", shallow_copy)
```

    ([5, 8, 3], 'i', 'z', 'k')
    ([5, 8, 3], 'i', 'z', 'k')
    
    After Modification:
    Orig_Tup: ([45, 8, 3], 'i', 'z', 'k')
    shallow_copy: ([45, 8, 3], 'i', 'z', 'k')
    

### 20.Create a deep copy of a nested tuple and observe the effects of modifying one of the tuples.


```python
import copy
original_tuple = (1, 2, [3, 4, [5, 6]])
deep_copy_tuple = copy.deepcopy(original_tuple)
print("Original Tuple:", original_tuple)
print("Deep Copy Tuple:", deep_copy_tuple)
original_tuple[2][2][0] = 99
print("\nAfter Modification:")
print("Original Tuple:", original_tuple)
print("Deep Copy Tuple:", deep_copy_tuple)

```

    Original Tuple: (1, 2, [3, 4, [5, 6]])
    Deep Copy Tuple: (1, 2, [3, 4, [5, 6]])
    
    After Modification:
    Original Tuple: (1, 2, [3, 4, [99, 6]])
    Deep Copy Tuple: (1, 2, [3, 4, [5, 6]])
    

### 21.Pickle a tuple and save it to a file.


```python
import pickle
new_tuple = ([3] , 'kinza')
with open('new_tuple.pkl', 'wb') as file:
    pickle.dump(new_tuple, file)
print("Tuple pickled and saved to 'new_tuple.pkl'")
```

    Tuple pickled and saved to 'new_tuple.pkl'
    

### 22.Unpickle a tuple from a file and display its content.


```python
import pickle
with open('new_tuple.pkl', 'rb') as file:
    loaded_tuple = pickle.load(file)
print("Tuple loaded from '_tuple.pkl':", loaded_tuple)

```

    Tuple loaded from '_tuple.pkl': ([3], 'kinza')
    


```python

```
