[[Python Data Structures]]
### Introduction

In this video, we will discuss the tuple data structure in Python. Tuples are ordered collections of items that are immutable.

### Creating Tuples

To create a tuple, we use parentheses `()` instead of square brackets `[]` like in lists.

```python

my_tuple = (1, 2, 3, 4, 5, 6)  # Create a tuple with 6 elements   
print(my_tuple)  # Output: (1, 2, 3, 4, 5, 6)`
```

We can also create a tuple using the `tuple()` function.

```python


my_tuple = tuple([1, 2, 3, 4, 5, 6])  # Convert a list to a tuple  
print(my_tuple)  # Output: (1, 2, 3, 4, 5, 6)`
```

### Accessing Tuple Elements

We can access tuple elements using indexing, just like in lists.

```python

my_tuple = (1, 2, 3, 4, 5, 6)  # Create a tuple  
print(my_tuple[0])  # Access the first element (index 0)   
print(my_tuple[-1])  # Access the last element (index -1)`
```

We can also use slicing to access a range of elements.

```python
my_tuple = (1, 2, 3, 4, 5, 6)  # Create a tuple   \
print(my_tuple[1:4])  # Access elements from index 1 to 3`
```
### Tuple Operations

Tuples support concatenation and repetition.

```python
my_tuple1 = (1, 2, 3)  # Create a tuple  
my_tuple2 = (4, 5, 6)  # Create another tuple  
print(my_tuple1 + my_tuple2)  # Concatenate two tuples 
print(my_tuple1 * 3)  # Repeat a tuple 3 times`
```
### Immutable Nature of Tuples

Tuples are immutable, meaning their elements cannot be changed once assigned.

```python

my_typle = (1, 2, 3)  # Create a tuple 
my_tuple[0] = 10  # Error: 'tuple' object does not support item assignment`
```
### Tuple Methods

Tuples have two built-in methods: `count()` and `index()`.

```python
my_tuple = (1, 2, 3, 2, 4)  # Create a tuple   
print(my_tuple.count(2))  # Count the occurrences of 2 
print(my_tuple.index(3))  # Find the index of 3, return the first index of the value
````

### Packing and Unpacking Tuples

We can pack and unpack tuples using the `*` operator.


```python
my_tuple = (1, 2, 3)  # Create a tuple   
a, b, c = my_tuple  # Unpack the tuple into 3 variables
print(a, b, c)  # Output: 1 2 3`
```

We can also use the `*` operator to unpack a tuple with a variable number of elements.

```python
my_tuple = (1, 2, 3, 4, 5)  # Create a tuple   
a, *b, c = my_tuple  # Unpack the tuple into 3 variables  
print(a, b, c)  # Output: 1 [2, 3, 4] 5`
```

### Nested Tuples

We can create nested tuples by placing tuples inside other tuples.

```python
my_tuple = ((1, 2, 3), (4, 5, 6))  # Create a nested tuple  
print(my_tuple[0])  # Access the first inner tuple  
print(my_tuple[0][1])  # Access the second element of the first inner tuple
````

We can also iterate over nested tuples using a for loop.

```python 
my_tuple = ((1, 2, 3), (4, 5, 6))  # Create a nested tuple  
for sub_tuple in my_tuple:  # Iterate over the inner tuples  
	for item in sub_tuple:  # Iterate over the elements of each inner tuple     
		print(item)  # Print each element
````