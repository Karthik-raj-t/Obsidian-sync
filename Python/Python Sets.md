
[python]
- **Definition of Sets**:
    
    - Built-in data structure in Python.
    - Stores unique items, unordered, and does **not allow duplicates.**
    - Useful for membership tests, eliminating duplicates, and performing set operations (union, intersection, etc.).
- **Creating Sets**:
    
    - Use curly braces **`{}`** for defining a set.
    - For an empty set, use **`set()`**.
	    **my_set = {'a','b','c','d'}**
- **Key Properties**:
    
    - Duplicate elements are automatically ignored.
    - Sets are unordered, meaning elements do not follow a specific order.
### **Basic Set Operations**
- **Adding and Removing Elements**:
    
    - Add elements using `set_name.add()`.
    - Remove elements using `set_name.remove()`. Raises a KeyError if the element doesn’t exist.
    - Use `set_name.discard()` to remove an element without raising an error.
    - Use `set_name.pop()` to remove and return a random element (First-In-First-Out behavior).
    - `set_name.clear()` removes all elements from the set.
- **Set Membership Test**:
    
    - Use `in` to check if an element exists in the set. 
       `print (10 in set_name)
    - Returns `True` if the element is found, otherwise `False`.
- 
####  **Mathematical Set Operations**:
    
    **Union**: Combines all elements from two sets (set1.union(set2)).
- **Intersection**: Returns common elements from two sets (`set1.intersection(set2)`).
- **Intersection Update**: Updates set1 with common elements (`set1.intersection_update(set2)`).
- **Difference**: Elements in set1 that are not in set2 (`set1.difference(set2)`).
- **Difference Update**: Removes common elements from set1 (`set1.difference_update(set2)`).
- **Symmetric Difference**: Combines unique elements from both sets while removing common elements (`set1.symmetric_difference(set2)`).

####  **Subset Superset**:
##### Subset Operations

- **Subset (`issubset`)**: Determines if all elements of one set are present in another set.
    - Syntax: `set1.issubset(set2)`
    - Returns `True` if `set1` is a subset of `set2`, meaning all elements of `set1` are contained within `set2`.
    
##### Superset Operations

- **Superset (`issuperset`)**: Checks if a set contains all elements of another set.
    
    - Syntax: `set1.issuperset(set2)`
    - Returns `True` if `set1` is a superset of `set2`, meaning all elements of `set2` are contained in `set1`.
- 