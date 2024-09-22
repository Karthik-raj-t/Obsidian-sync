## Outline
1. Introduction to Dictionaries
2. Creating Dictionaries
3. Accessing Dictionary Elements
4. Modifying Dictionary Elements
5. Dictionary Methods
6. Iterating over Dictionaries
7. Nested Dictionaries
8. Dictionary Comprehension
9. Common Errors

---

## Introduction to Dictionaries
- **Dictionaries**: An unordered collection of items stored as key-value pairs.
  - **Keys**: Must be unique and immutable (cannot be changed once defined).
  - **Values**: Can be of any type and are mutable (can be changed).
  - Keys can include strings, numbers, or tuples.
  - Example:
    ```python
    student = {"name": "Krish", "age": 32, "grade": "A"}
    ```

---

## Creating Dictionaries
1. **Empty Dictionary**:
   - Using curly braces:
     ```python
     empty_dict = {}
     ```
   - Using `dict()`:
     ```python
     empty_dict = dict()
     ```
2. **Dictionary with key-value pairs**:
   - Example:
     ```python
     student = {"name": "Krish", "age": 32, "grade": "A"}
     ```

---

## Accessing Dictionary Elements
1. **Access using key**:
   ```python
   student["grade"]  # Outputs: 'A'
--```
  2.**Using `get()` method**:
	  Safer way to access values (returns `None` if key not found):
	 
```
 student.get("grade")  # Outputs: 'A'
student.get("lastname", "Not available")  # Outputs: 'Not available' else ouput is 'None'
``````


## Modifying Dictionary Elements

- **Dictionaries are mutable**: We can add, update, or delete elements.

1. **Update values**:
    
    ```python
	student["age"] = 33   
	 ```
**Add new key-value pairs**:



