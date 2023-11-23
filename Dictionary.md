# Assignment 05 Part 03
### Dictionary

### 1.Create an empty dictionary and print it.


```python
emp_dictionary = {}
print(emp_dictionary)
type(emp_dictionary)
```

    {}
    




    dict



### 2.Create a dictionary representing a person with keys such as 'name', 'age', and 'city'.


```python
new_dict = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore'
}
print(new_dict)
type(new_dict)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore'}
    




    dict



### 3.Create a dictionary that includes keys with different data types (strings, integers).


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
print(new_dict_1)
type(new_dict_1)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}}
    




    dict



### 4.Access and print the value associated with a specific key.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
print(new_dict_1)
type(new_dict_1)
name_value = new_dict_1['name']
print("value with name:" ,name_value)
city_value = new_dict_1['city']
print("value with city:" ,city_value)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}}
    value with name: kinza
    value with city: Lahore
    

### 5.Use the get() method to access a value, providing a default value if the key is not present.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
print(new_dict_1)
type(new_dict_1)
name_value = new_dict_1.get('name', 'Default Name')
print("value with name:" ,name_value)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}}
    value with name: kinza
    

### 6.Iterate through the keys of a dictionary and print each key.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
print(new_dict_1)
type(new_dict_1)
for key in new_dict_1:
    print(key)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}}
    name
    age
    city
    grades
    

### 7.Add a new key-value pair to a dictionary.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
new_dict_1['gender'] = 'GIRL'
print(new_dict_1)
```

    {'name': 'kinza', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}, 'gender': 'GIRL'}
    

### 8.Modify the value associated with an existing key.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
new_dict_1['name'] = 'kinoo'
print(new_dict_1)
```

    {'name': 'kinoo', 'age': 24, 'city': 'Lahore', 'grades': {'english': 70}}
    

### 9.Remove a specific key-value pair from a dictionary using the pop() method.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
remove = new_dict_1.pop('city')
print(new_dict_1)
```

    {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
    

### 10.Remove a specific key-value pair from a dictionary using the del statement.


```python
new_dict_1 = {
    'name': 'kinza',
    'age' : 24,
    'city' : 'Lahore',
    'grades' : {'english':70}
}
del new_dict_1['age']
print(new_dict_1)
```

    {'name': 'kinza', 'city': 'Lahore', 'grades': {'english': 70}}
    

### 11.Convert a dictionary to a list of keys.


```python
dict_2 = {'name': 'kinza', 'city': 'Lahore', 'grades': {'english': 70}}
keys_list = list(dict_2.keys())
print(keys_list)
```

    ['name', 'city', 'grades']
    

### 12.Convert a dictionary to a list of values.


```python
dict_2 = {'name': 'kinza', 'city': 'Lahore', 'grades': {'english': 70}}
values_list = list(dict_2.values())
print(values_list)
```

    ['kinza', 'Lahore', {'english': 70}]
    

### 13.Convert a list of tuples to a dictionary.


```python
list_of_tuples = [('name' , 'kinza'),('age' , 24)]
dictionary = dict(list_of_tuples)
print(dictionary)
type(dictionary)
```

    {'name': 'kinza', 'age': 24}
    




    dict



### 14.Use the keys() method to get a list of keys in a dictionary.


```python
my_dict = {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
keys = my_dict.keys()
keys_list = list(keys_list)
print(keys_list)
```

    ['name', 'city', 'grades']
    

### 15.Use the values() method to get a list of values in a dictionary.


```python
my_dict = {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
values = my_dict.values()
values_list = list(values_list)
print(values_list)
```

    ['kinza', 'Lahore', {'english': 70}]
    

### 16.Use the items() method to get a list of key-value pairs in a dictionary.


```python
my_dict = {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
items = my_dict.items()
items_list = list(items)
print(items_list)
```

    [('name', 'kinza'), ('age', 24), ('grades', {'english': 70})]
    

### 17.Check if a key is present in a dictionary using the in operator.


```python
my_dict = {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
if 'grades' in my_dict:
    print("The key and value pair of grades is in dictionary")
else: 
    print("The key and value pair of grades is not in dictionary")
```

    The key and value pair of grades is in dictionary
    

### 18.Use the setdefault() method to add a key with a default value if it doesn't exist.


```python
my_dict = {'name': 'kinza', 'age': 24, 'grades': {'english': 70}}
occupation_value = my_dict.setdefault('occupation' , 'programmer')
print(my_dict)
print("value with occupation:" ,occupation_value)

```

    {'name': 'kinza', 'age': 24, 'grades': {'english': 70}, 'occupation': 'programmer'}
    value with occupation: programmer
    

### 19.Merge two dictionaries using the update() method.


```python
dict_1 = {'name' : 'kinza' , 'father' : 'ishaq'}
dict_2 = {'gender' : 'girl' , 'hobby' : 'programming'}
merged = dict_1.update(dict_2)
print("merged dictionary is now:" ,dict_1)
```

    merged dictionary is now: {'name': 'kinza', 'father': 'ishaq', 'gender': 'girl', 'hobby': 'programming'}
    

### 20.Use the clear() method to remove all elements from a dictionary.


```python
new_dict = {'name': 'kinza', 'father': 'ishaq', 'gender': 'girl', 'hobby': 'programming'}
remove = new_dict.clear()
print(new_dict)
```

    {}
    


```python

```
