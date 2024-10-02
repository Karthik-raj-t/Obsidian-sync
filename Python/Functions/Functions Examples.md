## Example 1: Temperature Conversion

```python
def convert_temperature(temp, unit):     
"""This function converts temperature between Celsius and Fahrenheit"""    
	if unit == 'C':        
		return temp * 9/5 + 32  # Celsius to Fahrenheit    
	elif unit == "F":       
		return (temp-32)*5/9  # Fahrenheit to Celsius    
	else:        
		return None 

print(convert_temperature(25, 'C'))  # Output: 77.0 
print(convert_temperature(77, 'F'))  # Output: 25.0`
```

## Example 2: Password Strength Checker

```python

def is_strong_password(password):     
"""This function checks if the password is strong or not"""    
	if len(password) < 8:   
		return False    
	if not any(char.isdigit() for char in password):        
		return False    
	if not any(char.islower() for char in password):        
		return False    
	if not any(char.isupper() for char in password):        
		return False    
	if not any(char in '!@#$%^&*()_+' for char in password):        
		return False    
	return True 
	
print(is_strong_password("WeakPwd"))  # Output: False  
print(is_strong_password("Str0ngPwd!"))  # Output: True
```

## Example 3: Calculate the Total Cost Of Items In a Shopping Cart

```python

def calculate_total_cost(cart):     
	total_cost = 0    
	for item in cart:    
		total_cost += item['price'] * item['quantity']    
	return total_cost 

cart = [     {'name': 'Apple', 'price': 0.5, 'quantity': 4},    {'name': 'Banana', 'price': 0.3, 'quantity': 6},    {'name': 'Orange', 'price': 0.7, 'quantity': 3} ] 

total_cost = calculate_total_cost(cart) 
print(total_cost)  # Output: 5.8999999999999995
```

## Example 4: Check If a String Is Palindrome

```python

def is_palindrome(s):     
	s = s.lower().replace(" ", "")    
	return s == s[::-1] 
	
print(is_palindrome("A man a plan a canal Panama"))  # Output: True 
print(is_palindrome("Hello"))  # Output: False
```

## Example 5: Calculate the factorials of a number using recursion

```python

def factorial(n):     
	if n == 0:        
		return 1    
	else:        
		return n * factorial(n-1) 

print(factorial(6))  # Output: 720
```

## Example 6: A Function To Read A File and count the frequency of each word

```python

def count_word_frequency(file_path):     
	word_count = {}    
	with open(file_path, 'r') as file:        
		for line in file:            
			words = line.split()            
				for word in words:                
				word = word.lower().strip('.,!?;:"\'')                
				word_count[word] = word_count.get(word, 0) + 1     
				return word_count 

filepath = 'sample.txt' 
word_frequency = count_word_frequency(filepath) 
print(word_frequency)`
```

## Example 7: Validate Email Address

```python

import re 

def is_valid_email(email):     
"""This function checks if the email is valid."""    
	pattern = r'^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$'    
	return re.match(pattern, email) is not None 
	
print(is_valid_email("test@example.com"))  # Output: True 
print(is_valid_email("invalid-email"))  # Output: False`
```

--

**Related Links:**

- [[Functions in Python]]