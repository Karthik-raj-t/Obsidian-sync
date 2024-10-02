

Lambda functions are small anonymous functions defined using the **lambda** keyword. They can have any number of arguments but only one expression. They are commonly used for short operations or as arguments to higher-order functions.

## Syntax

```python
lambda arguments: expression
```

## Examples

#### Basic Addition
```python

#Regular Function

def addition(a,b):     
	return a+b 
addition(2,3)  # Output: 5

#Lambda Function
addition = lambda a,b: a+b 
addition(5,6)  # Output: 11
```

### Even Number Check

```python
# Regular Function

def even(num):  
	if num % 2 == 0:     
		return True     
even(24)  # Output: True

# Lambda Function

even1 = lambda num: num % 2 == 0 
even1(12)  # Output: True`
```

### Multiple Arguments

```python
# Regular Function

def addition(x,y,z):     
	return x+y+z 
addition(12,13,14)  # Output: 39`

# Lambda Function

addition1 = lambda x,y,z: x+y+z 
addition1(12,13,14)  # Output: 39`
```

## Using Lambda with Higher-Order Functions

### map() Function

The `map()` function applies a given function to all items in an iterable.

```python

numbers = [1,2,3,4,5,6] 
# Using a regular function 
def square(number):     
	return number**2 
square(2)  # Output: 4 
list(map(square,numbers))
# need to write a for loop instead using map function

# Using lambda with map() 
list(map(lambda x: x**2, numbers))  # Output: [1, 4, 9, 16, 25, 36]
```

---

[[Python Functions]] | [[Functional Programming]]|[[Lambda Functions]]