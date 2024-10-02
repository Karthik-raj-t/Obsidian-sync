

The `map()` function applies a given function to all items in an input list (or any other iterable) and returns a map object (an iterator). This is particularly useful for transforming data in a list comprehensively.

## Basic Usage

```python
### With Regular Functions

def square(x):     
	return x * x 

numbers = [1, 2, 3, 4, 5, 6, 7, 8] 
squared_numbers = list(map(square, numbers)) # Output: [1, 4, 9, 16, 25, 36, 49, 64]

### With Lambda Functions

numbers = [1, 2, 3, 4, 5, 6, 7, 8] 
squared_numbers = list(map(lambda x: x * x, numbers)) # Output: [1, 4, 9, 16, 25, 36, 49, 64]
```

## Advanced Usage

```python
### Multiple Iterables

numbers1 = [1, 2, 3] 
numbers2 = [4, 5, 6] 
added_numbers = list(map(lambda x, y: x + y, numbers1, numbers2)) # Output: [5, 7, 9]`

### Type Conversion

# Convert strings to integers 
str_numbers = ['1', '2', '3', '4', '5'] 
int_numbers = list(map(int, str_numbers)) # Output: [1, 2, 3, 4, 5]`
```

### String Manipulation

```python


words = ['apple', 'banana', 'cherry'] 
upper_words = list(map(str.upper, words)) # Output: ['APPLE', 'BANANA', 'CHERRY']
````

### Working with Dictionaries

```python
def get_name(person):     
	return person['name'] 

people = [     {'name': 'Krish', 'age': 32},    {'name': 'Jack', 'age': 33} ] 
list(map(get_name,people))

names = list(map(get_name, people)) # Output: ['Krish', 'Jack']
```

## Conclusion

The `map()` function is a powerful tool for applying transformations to iterable data structures. It can be used with regular functions, lambda functions, and even multiple iterables, providing a versatile approach to data processing in Python. By understanding and utilizing `map()`, you can write more efficient and readable code.

---

[[Python Built-in Functions]] | [[Functional Programming in Python]] | [[Lambda Functions]]|[[Map Functions]]