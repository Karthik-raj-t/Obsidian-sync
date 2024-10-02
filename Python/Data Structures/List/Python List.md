[[Python Data Structures]]
## 1. Introduction to Lists

- Lists are ordered, mutable collections of items
- Can contain different data types

## 2. Structure

- Notebook organized into sections covering various aspects of lists

## 3. Creating Lists

```python

lst = []  # Empty list 
mixed_list = [1, "Hello", 3.14, True]  # Mixed data types`
```

## 4. Accessing List Elements

```python

fruits[0]   # First element
fruits[-1]  # Last element 
fruits[1:]  # Slicing from second element to end 
fruits[1:3] # Slicing from second to third element`
```

## 5. Modifying List Elements

`
```python

fruits[1] = "watermelon"  # Change single element 
fruits[1:] = "watermelon" # Replace multiple elements
```

## 6. List Methods

- `append()`: Adds item to end
- `insert()`: Adds item at specific index
- `remove()`: Removes first occurrence of item
- `pop()`: Removes and returns last element
- `index()`: Finds index of item
- `count()`: Counts occurrences of item
- `sort()`: Sorts list in ascending order
- `reverse()`: Reverses list order
- `clear()`: Removes all items

```python
# Start with a sample list
fruits = ["apple", "banana", "cherry", "date", "banana"]

# append(): Adds item to end
fruits.append("elderberry")
print(fruits)  # ["apple", "banana", "cherry", "date", "banana", "elderberry"]

# insert(): Adds item at specific index
fruits.insert(1, "blueberry")
print(fruits)  # ["apple", "blueberry", "banana", "cherry", "date", "banana", "elderberry"]

# remove(): Removes first occurrence of item
fruits.remove("banana")
print(fruits)  # ["apple", "blueberry", "cherry", "date", "banana", "elderberry"]

# pop(): Removes and returns last element
last_fruit = fruits.pop()
print(last_fruit)  # "elderberry"
print(fruits)  # ["apple", "blueberry", "cherry", "date", "banana"]

# index(): Finds index of item
cherry_index = fruits.index("cherry")
print(cherry_index)  # 2

# count(): Counts occurrences of item
banana_count = fruits.count("banana")
print(banana_count)  # 1

# sort(): Sorts list in ascending order
fruits.sort()
print(fruits)  # ["apple", "banana", "blueberry", "cherry", "date"]

# reverse(): Reverses list order
fruits.reverse()
print(fruits)  # ["date", "cherry", "blueberry", "banana", "apple"]

# clear(): Removes all items
fruits.clear()
print(fruits)  # []
```
## 7. Slicing Lists

- Various slicing techniques demonstrated

## 8. Iterating Over Lists

```python
for item in list:     # process item for index, item in enumerate(list):     # process index and item`
```

## 9. List Comprehensions

- Basic syntax: `[expression for item in iterable]`
- With condition: `[expression for item in iterable if condition]`
- Nested: `[expression for item1 in iterable1 for item2 in iterable2]`

## 10. Examples of List Comprehensions

```python

squares = [x**2 for x in range(10)] 
even_numbers = [num for num in range(10) if num % 2 == 0] 
pairs = [[i, j] for i in list1 for j in list2] 
word_lengths = [len(word) for word in words]`
```

## 11. Conclusion

- Emphasizes the power and conciseness of list comprehensions
- Encourages their use for cleaner and more efficient code

The notebook provides a comprehensive overview of Python lists, covering creation, manipulation, methods, iteration, and advanced concepts like list comprehensions. It includes both explanations and code examples for each topic.