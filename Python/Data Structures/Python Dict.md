## Introduction

Dictionaries are unordered collections of items in Python, storing data in key-value pairs. Keys must be unique and immutable, while values can be of any type.

## Creating Dictionaries

```python
empty_dict = {} 
empty_dict = dict() 
student = {"name": "Krish", "age": 32, "grade": 24}`
```

## Accessing Dictionary Elements

```python
print(student['grade']) 
print(student.get('grade')) 
print(student.get('last_name', "Not Available"))`
```

## Modifying Dictionary Elements

```python

student["age"] = 33 
student["address"] = "India"
del student['grade']` # for deleting the data
```
## Dictionary Methods
```python

keys = student.keys() values = student.values() items = student.items()`
```

## Shallow Copy vs Deep Copy

```python

student_copy = student  # Shallow copy 
student_copy1 = student.copy()  # Deep copy
```
## Iterating Over Dictionaries

```python

for key in student.keys():    
	print(key) for value in student.values():   
	print(value) for key, value in student.items():     
	print(f"{key}:{value}")
```

## Nested Dictionaries

```python
students = {     "student1": {"name": "Krish", "age": 32},    "student2": {"name": "Peter", "age": 35} } 
print(students["student2"]["name"]) for student_id, student_info in students.items():   print(f"{student_id}:{student_info}")    for key, value in student_info.items():        print(f"{key}:{value}")
```

## Dictionary Comprehension

```python

squares = {x: x**2 for x in range(5)} 
evens = {x: x**2 for x in range(10) if x % 2 == 0}
```
## Practical Examples

### Counting Frequency

```python
numbers = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4] 
frequency = {} for number in numbers:    	
	if number in frequency:        
		frequency[number] += 1   
	else:       
		frequency[number] = 1
````

### Merging Dictionaries

```python

dict1 = {"a": 1, "b": 2}
dict2 = {"b": 3, "c": 4} 
merged_dict = {**dict1, **dict2}`
```

## Conclusion

Dictionaries are powerful tools in Python for managing key-value pairs, used in various scenarios like counting word frequency, grouping data, storing configuration settings, managing phonebooks, tracking inventory, and caching results.

--

[[Python Data Structures]] 


