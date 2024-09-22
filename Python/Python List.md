[python]
#### **List Function**
- **`append(item)`**: Adds an item to the end of the list.
- **`insert(index, item)`**: Inserts an item at a specific index.
- **`remove(item)`**: Removes the first occurrence of an item.
- **`pop()`**: Removes and returns the last item.
- **`index(item)`**: Returns the index of the first occurrence of an item.
- **`count(item)`**: Returns the number of times an item appears in the list.
#### **List Slicing:**

- **Basic Slicing**:
    
    - `numbers[2:5]`: Extracts elements from index 2 to 4 (end index not included).
    - `numbers[:5]`: Extracts from the beginning to index 4.
    - `numbers[5:]`: Extracts from index 5 to the end of the list.
- **Step Slicing (Double Colon)**:
    
    - `numbers[::2]`: Extracts elements starting from index 0, taking every second element.
    - `numbers[::-1]`: Reverses the list by taking every element from the end to the beginning.
- **Negative Step**:
    
    - `numbers[::-2]`: Extracts every second element from the end of the list.**

####  **Iterating Over List **

	Basic
		[expression for item in iterable]
		Example: `[x**2 for x in range(10)]` gives the square of numbers from 0 to 9.
		
	With Conditional Logic:
		[expression for item in iterable if condition]
		Example: `[x for x in range(10) if x % 2 == 0]` extracts even numbers.
		
	Nested List Comprehension:
		[(i, j) for i in list1 for j in list2]
		Example: Pairs elements from two lists, like `[(1, 'a'), (1, 'b'), (2, 'a'), ..]`.
		
	Using enumerate : 
		for index, element in enumerate(numbers): print(index, element)
