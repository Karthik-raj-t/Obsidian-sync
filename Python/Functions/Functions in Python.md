## Introduction to Functions

**Definition**: A function is a block of code that performs a specific task. Functions help in organizing code, reusing code, and improving readability.

## Defining Functions

Basic syntax:

```python
def function_name(parameters):    
	"""Docstring"""   
	 # Function body    
	 return expression
```

## Why Functions?

Functions allow us to encapsulate logic and reuse it. For example:

```python

def even_or_odd(num):    
"""This function finds even or odd"""    
	if num % 2 == 0:       
		print("the number is even")    
	else:    
	    print("the number is odd")`
```
## Calling Functions

To use a function, we call it by its name and provide any required arguments:

```python
even_or_odd(24)
```

## Function Parameters

Functions can accept multiple parameters:

```python
def add(a, b):    
	return a + b 
	
result = add(2, 4) 
print(result)  # Output: 6
```
## Default Parameters

We can set default values for parameters:

```python

def greet(name="Guest"):    
	print(f"Hello {name} Welcome To the paradise") 
	
greet("Krish")  
# Output: Hello Krish Welcome To the paradise 
greet() 
# Output: Hello Guest Welcome To the paradise
```

## Variable-Length Arguments

### Positional Arguments (*args)

```python

def print_numbers(*args):     
	for number in args:       
		print(number) 
		
print_numbers(1, 2, 3, 4, 5, 6, 7, 8, "Krish")
```

### Keyword Arguments (**kwargs)

```python

def print_details(**kwargs):     
	for key, value in kwargs.items():        
		print(f"{key}:{value}") 

print_details(name="Krish", age="32", country="India")
```

### Combining *args and **kwargs

```python
def print_details(*args, **kwargs):     
	for val in args:        
		print(f" Positional argument :{val}")         
		for key, value in kwargs.items():        
			print(f"{key}:{value}") 
			
print_details(1, 2, 3, 4, "Krish", name="Krish", age="32", country="India")
```

## Return Statement

Functions can return single or multiple values:

```python
def multiply(a, b):     
	return a * b 
	
result = multiply(2, 3) # result = 6 

def multiply_and_return_first(a, b):     
	return a * b, a 
	
result, first = multiply_and_return_first(2, 3)  # result = 6, first = 2
```

----

**Related Links:**

- [[Python Basics]]
