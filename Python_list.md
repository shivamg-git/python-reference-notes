# Python List
---
**Lists are a useful tool for preserving a sequence of data and further iterating over it.**

**Note** - Unlike Sets, list may contain mutable elements.
```python
# Creating a List
List = []
print("Intial blank List: ")
print(List)

# Creating a List with 
# the use of a String
List = ['GeeksForGeeks']
print("\nList with the use of String: ")
print(List)

# Creating a List with
# the use of multiple values
List = ["Geeks", "For", "Geeks"]
print("\nList containing multiple values: ")
print(List[0]) 
print(List[2])

# Creating a Multi-Dimensional List
# (By Nesting a list inside a List)
List = [['Geeks', 'For'] , ['Geeks']]
print("\nMulti-Dimensional List: ")
print(List)

# Creating a List with 
# the use of Numbers
# (Having duplicate values)
List = [1, 2, 4, 4, 3, 3, 3, 6, 5]
print("\nList with the use of Numbers: ")
print(List)

# Creating a List with 
# mixed type of values
# (Having numbers and strings)
List = [1, 2, 'Geeks', 4, 'For', 6, 'Geeks']
print("\nList with the use of Mixed Values: ")
print(List)


#OUTPUT
Intial blank List: 
[]

List with the use of String: 
['GeeksForGeeks']

List containing multiple values: 
Geeks
Geeks

Multi-Dimensional List: 
[['Geeks', 'For'], ['Geeks']]

List with the use of Numbers: 
[1, 2, 4, 4, 3, 3, 3, 6, 5]

List with the use of Mixed Values: 
[1, 2, 'Geeks', 4, 'For', 6, 'Geeks']
```
---
* **Adding Elements to a List**

**Note** - append() and extend() methods can only add elements at the end.


```python
# Creating a List
List = []
print("Intial blank List: ")
print(List)

# Addition of Elements 
# in the List
List.append(1)
List.append(2)
List.append(4)
print("\nList after Addition of Three elements: ")
print(List)

# Adding elements to the List
# using Iterator
for i in range(1, 4):
    List.append(i)
print("\nList after Addition of elements from 1-3: ")
print(List)

# Adding Tuples to the List
List.append((5, 6))
print("\nList after Addition of a Tuple: ")
print(List)

# Addition of List to a List
List2 = ['For', 'Geeks']
List.append(List2)
print("\nList after Addition of a List: ")
print(List)

# Addition of Element at 
# specific Position
# (using Insert Method)
List.insert(3, 12)
List2.insert(0, 'Geeks')
print("\nList after performing Insert Operation: ")
print(List)

# Addition of multiple elements
# to the List at the end
# (using Extend Method)
List.extend([8, 'Geeks', 'Always'])
print("\nList after performing Extend Operation: ")
print(List)

#OUTPUT
Intial blank List: 
[]

List after Addition of Three elements: 
[1, 2, 4]

List after Addition of elements from 1-3: 
[1, 2, 4, 1, 2, 3]

List after Addition of a Tuple: 
[1, 2, 4, 1, 2, 3, (5, 6)]

List after Addition of a List: 
[1, 2, 4, 1, 2, 3, (5, 6), ['For', 'Geeks']]

List after performing Insert Operation: 
[1, 2, 4, 12, 1, 2, 3, (5, 6), ['Geeks', 'For', 'Geeks']]

List after performing Extend Operation: 
[1, 2, 4, 12, 1, 2, 3, (5, 6), ['Geeks', 'For', 'Geeks'], 8, 'Geeks', 'Always']
```
---

* **Accessing elements from the List**
```python
# Creating a List with
# the use of multiple values
List = ["Geeks", "For", "Geeks"]

# accessing a element from the 
# list using index number
print("Accessing a element from the list")
print(List[0]) 
print(List[2])

# Creating a Multi-Dimensional List
# (By Nesting a list inside a List)
List = [['Geeks', 'For'] , ['Geeks']]

# accessing a element from the 
# Multi-Dimensional List using
# index number
print("Acessing a element from a Multi-Dimensional list")
print(List[0][1])
print(List[1][0])


List = [1, 2, 'Geeks', 4, 'For', 6, 'Geeks']

# accessing a element using
# negative indexing
print("Acessing element using negative indexing")

# print the last element of list
print(List[-1])

# print the third last element of list 
print(List[-3])


#OUTPUT
Accessing a element from the list
Geeks
Geeks

Acessing a element from a Multi-Dimensional list
For
Geeks

Acessing element using negative indexing
Geeks
For
```
---
* **Removing Elements from the List**

**Note** - Remove method in List will only remove the first occurrence of the searched element.

```python
# Creating a List
List = [1, 2, 3, 4, 5, 6, 
        7, 8, 9, 10, 11, 12]
print("Intial List: ")
print(List)

# Removing elements from List
# using Remove() method
List.remove(5)
List.remove(6)
print("\nList after Removal of two elements: ")
print(List)

# Removing elements from List
# using iterator method
for i in range(1, 5):
    List.remove(i)
print("\nList after Removing a range of elements: ")
print(List)

# Removing element from the 
# Set using the pop() method
List.pop()
print("\nList after popping an element: ")
print(List)

# Removing element at a 
# specific location from the 
# Set using the pop() method
List.pop(2)
print("\nList after popping a specific element: ")
print(List)

#OUTPUT
Intial List: 
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]

List after Removal of two elements: 
[1, 2, 3, 4, 7, 8, 9, 10, 11, 12]

List after Removing a range of elements: 
[7, 8, 9, 10, 11, 12]

List after popping an element: 
[7, 8, 9, 10, 11]

List after popping a specific element: 
[7, 8, 10, 11]
```
---
* **Slicing of a List**

**Note** - To print elements of List from rear end, use Negative Indexes.

```python
# Creating a List
List = ['G','E','E','K','S','F',
        'O','R','G','E','E','K','S']
print("Intial List: ")
print(List)

# Print elements of a range
# using Slice operation
Sliced_List = List[3:8]
print("\nSlicing elements in a range 3-8: ")
print(Sliced_List)

# Print elements from beginning
# to a pre-defined point using Slice
Sliced_List = List[:-6]
print("\nElements sliced till 6th element from last: ")
print(Sliced_List)

# Print elements from a 
# pre-defined point to end
Sliced_List = List[5:]
print("\nElements sliced from 5th "
      "element till the end: ")
print(Sliced_List)

# Printing elements from
# beginning till end
Sliced_List = List[:]
print("\nPrinting all elements using slice operation: ")
print(Sliced_List)

# Printing elements in reverse
# using Slice operation
Sliced_List = List[::-1]
print("\nPrinting List in reverse: ")
print(Sliced_List)

#OUTPUT
Intial List: 
['G', 'E', 'E', 'K', 'S', 'F', 'O', 'R', 'G', 'E', 'E', 'K', 'S']

Slicing elements in a range 3-8: 
['K', 'S', 'F', 'O', 'R']

Elements sliced till 6th element from last: 
['G', 'E', 'E', 'K', 'S', 'F', 'O']

Elements sliced from 5th element till the end: 
['F', 'O', 'R', 'G', 'E', 'E', 'K', 'S']

Printing all elements using slice operation: 
['G', 'E', 'E', 'K', 'S', 'F', 'O', 'R', 'G', 'E', 'E', 'K', 'S']

Printing List in reverse: 
['S', 'K', 'E', 'E', 'G', 'R', 'O', 'F', 'S', 'K', 'E', 'E', 'G']
```
---
### List Methods in Python | Set 1 (in, not in, len(), min(), max()...)

#### List methods are discussed in this articles.
1. **"in" operator** :- This operator is used to check if an element is present in the list or not. Returns true if element is present in list else returns false. 

2. **"not in" operator** :- This operator is used to check if an element is not present in the list or not. Returns true if element is not present in list else returns false. 

3. **len()** :- This function returns the length of list.

4. **min()** :- This function returns the minimum element of list.

5. **max()** :- This function returns the maximum element of list.

6. **"+" operator** :- This operator is used to concatenate two lists into a single list.

7. **"*" operator** :- This operator is used to multiply the list "n" times and return the single list.

8. **index(ele, beg, end)** :- This function returns the index of first occurrence of element after beg and before end. 

9. **count()** :- This function counts the number of occurrences of elements in list.

10. **del[a : b]** :- This method deletes all the elements in range starting from index ‘a’ till ‘b’ mentioned in arguments.

11. **pop()** :- This method deletes the element at the position mentioned in its arguments.

12. **insert(a, x)** :- This function inserts an element at the position mentioned in its arguments. It takes 2 arguments, position and element to be added at respective position.

13. **remove()** :- This function is used to delete the first occurrence of number mentioned in its arguments.

14. **sort()** :- This function sorts the list in increasing order.

15. **reverse()** :- This function reverses the elements of list.

16. **extend(b)** :- This function is used to extend the list with the elements present in another list. This function takes another list as its argument.

17. **clear()** :- This function is used to erase all the elements of list. After this operation, list becomes empty.

18. **append()**: Used for appending and adding elements to List.It is used to add elements to the last position of List.

19. **sum()** : Calculates sum of all the elements of List.

![String Constants ](https://github.com/spiderOO7/python-reference-notes/blob/master/IMG/51.png "String Constant")

![String Constants ](https://github.com/spiderOO7/python-reference-notes/blob/master/IMG/52.png "String Constant")

![String Constants ](https://github.com/spiderOO7/python-reference-notes/blob/master/IMG/53.png "String Constant")

---
### Sort a List according to the Length of the Elements

The built-in functions include **sort()** and **sorted()** along with the key parameter. We can perform these in two ways. One way is to sort the list by creating a new list and another way is to sort within the given list, saving space.

**The syntax for sorting by creating a new list is:**
```
sorted_list = sorted(unsorted_list, key=len)
```

**The syntax for sorting without creating a new list is:**
```
unsorted_list.sort(key=len)
```
**Working:** These key function of Python's while sorting implemented is known as the decorate-sort-undecorate design pattern. It follows the following steps:

* Each element of the list is temporarily replaced with a “decorated” version that includes the result of the key function applied to the element.

* The list is sorted based upon the natural order of the keys.

* The decorated elements are replaced by the original elements.
---
### Union of two or more Lists

* **Maintaining Repetition**

We can simply use the plus "+" operator inorder to combine two list into one. This will reflect the repetition.

* **Maintaining both Repetition and Order**

To maintain the order of appearance in the new list we need to use the sorted() function, passing the addition of two lists(plus operated, as in the previous problem) as parameters.

* **Without Repetition**

To get rid of all the repetitive elements from the initial list, we use the set() function on both the lists, individually. Then we add them using the "+" operator and pass as a new list.

* **More than two lists**

We can also make an union of more than two lists. This can be done efficiently by using both the set() and union() function, simultaneously, as shown in the below example. This also takes care of the repetition and prevents them.
```python
# Maintained repetition 
def Union(lst1, lst2):
    final_list = lst1 + lst2
    return final_list
# [23, 15, 2, 14, 14, 16, 20, 52, 2, 48, 15, 12, 26, 32, 47, 54]

# Maintained repetition and order 
def Union(lst1, lst2):
    final_list = sorted(lst1 + lst2)
    return final_list
# [2, 2, 12, 14, 14, 15, 15, 16, 20, 23, 26, 32, 47, 48, 52, 54]

# Without repetition 
def Union(lst1, lst2):
    final_list = list(set(lst1) | set(lst2))
    return final_list
# [32, 2, 12, 14, 15, 16, 48, 47, 20, 52, 54, 23, 26]

def Union(lst1, lst2, lst3):
    final_list = list(set().union(lst1, lst2, lst3))
    return final_list
# [32, 64, 2, 4, 5, 6, 9, 12, 14, 15, 16, 48, 47, 78, 20, 52, 54, 23, 25, 26, 59]

# Driver Code
lst1 = [23, 15, 2, 14, 14, 16, 20 ,52]
lst2 = [2, 48, 15, 12, 26, 32, 47, 54]
lst3 = [4, 78, 5, 6, 9, 25, 64, 32, 59]
print(Union(lst1, lst2))
```
---
### Intersection of two lists

**Method 1:** This is the simplest method where we haven't used any built-in functions.
```python
# Python program to illustrate the intersection
# of two lists in most simple way
def intersection(lst1, lst2):
    lst3 = [value for value in lst1 if value in lst2]
    return lst3

# Driver Code
lst1 = [4, 9, 1, 17, 11, 26, 28, 54, 69]
lst2 = [9, 9, 74, 21, 45, 11, 63, 28, 26]
print(intersection(lst1, lst2))

#Output:
[9, 11, 26, 28]
```

**Method 2:** This method includes the use of set() method.

```python
# Python program to illustrate the intersection
# of two lists using set() method
def intersection(lst1, lst2):
    return list(set(lst1) & set(lst2))

# Driver Code
lst1 = [15, 9, 10, 56, 23, 78, 5, 4, 9]
lst2 = [9, 4, 5, 36, 47, 26, 10, 45, 87]
print(intersection(lst1, lst2))

#Output:
[9, 10, 4, 5]
```

**Method 3:** In this method we set() the larger list and then use the built-in function called interscetion() to compute the intersected list. intersection() is a first-class part of set.

```python
# Python program to illustrate the intersection
# of two lists using set() and intersection()
def Intersection(lst1, lst2):
    return set(lst1).intersection(lst2)
    
# Driver Code
lst1 = [ 4, 9, 1, 17, 11, 26, 28, 28, 26, 66, 91]
lst2 = [9, 9, 74, 21, 45, 11, 63]
print(Intersection(lst1, lst2))


#Output:
{9, 11}
```

**Method 4:** By the use of this hybrid method the complexity of the program falls to O(n). This is an efficient way of doing the following program.
```python
# Python program to illustrate the intersection
# of two lists
def intersection(lst1, lst2):

    # Use of hybrid method
    temp = set(lst2)
    lst3 = [value for value in lst1 if value in temp]
    return lst3

# Driver Code
lst1 = [9, 9, 74, 21, 45, 11, 63]
lst2 = [4, 9, 1, 17, 11, 26, 28, 28, 26, 66, 91]
print(intersection(lst1, lst2))


#Output:
[9, 9, 11]
```

**Method 5:** This is the where the intersection is performed over sub-lists inside other lists. Here we have used the concept of filter().<br>
**Working:** The filter part takes each sublist's item and checks to see if it is in the source list. The list comprehension is executed for each sublist in list2.
```python
# Python program to illustrate the intersection
# of two lists, sublists and use of filter()
def intersection(lst1, lst2):
    lst3 = [list(filter(lambda x: x in lst1, sublist)) for sublist in lst2]
    return lst3

# Driver Code
lst1 = [1, 6, 7, 10, 13, 28, 32, 41, 58, 63]
lst2 = [[13, 17, 18, 21, 32], [7, 11, 13, 14, 28], [1, 5, 6, 8, 15, 16]]
print(intersection(lst1, lst2))

#Output:
[[13, 32], [7, 13, 28], [1, 6]]
```
---
## Using List as Stack and Queues in Python
```python
# Python code to demonstrate Implementing 
# stack using list
stack = ["Amar", "Akbar", "Anthony"]
stack.append("Ram")
stack.append("Iqbal")
print(stack)
print(stack.pop())
print(stack)
print(stack.pop())
print(stack)

#OUTPUT
['Amar', 'Akbar', 'Anthony', 'Ram', 'Iqbal']
Iqbal
['Amar', 'Akbar', 'Anthony', 'Ram']
Ram
['Amar', 'Akbar', 'Anthony']
```

```python
# Python code to demonstrate Implementing 
# Queue using deque and list
from collections import deque
queue = deque(["Ram", "Tarun", "Asif", "John"])
print(queue)
queue.append("Akbar")
print(queue)
queue.append("Birbal")
print(queue)
print(queue.popleft())                 
print(queue.popleft())                 
print(queue)

#OUTPUT
deque(['Ram', 'Tarun', 'Asif', 'John'])
deque(['Ram', 'Tarun', 'Asif', 'John', 'Akbar'])
deque(['Ram', 'Tarun', 'Asif', 'John', 'Akbar', 'Birbal'])
Ram
Tarun
deque(['Asif', 'John', 'Akbar', 'Birbal'])
```
---
## Numbers in a list within a given range
* Multiple Line Approach:
```python
# Python program to count the 
# number of numbers in a given range
# using traversal and mutliple line code

def count(list1, l, r):
    c = 0 
    # traverse in the list1
    for x in list1:
        # condition check
        if x>= l and x<= r:
            c+= 1 
    return c
    
# driver code
list1 = [10, 20, 30, 40, 50, 40, 40, 60, 70]
l = 40
r = 80 
print count(list1, l, r)
```
* Single Line Approach:
```python
# Python program to count the 
# number of numbers in a given range

def count(list1, l, r):
    
    # x for x in list1 is same as traversal in the list
    # the if condition checks for the number of numbers in the range 
    # l to r 
    # the return is stored in a list
    # whose length is the answer
    return len(list(x for x in list1 if l <= x <= r))

# driver code
list1 = [10, 20, 30, 40, 50, 40, 40, 60, 70]
l = 40
r = 80 
print count(list1, l, r)
```
---
### Tuples

* Creating a Tuple<br/>
**Note** - Creation of Python tuple without the use of parentheses is known as Tuple Packing.
```python
# Creating an empty tuple
Tuple1 = ()
print("Initial empty Tuple: ")
print (Tuple1)

# Creating a Tuple with 
# the use of Strings
Tuple1 = ('Geeks', 'For')
print("\nTuple with the use of String: ")
print(Tuple1)

# Creating a Tuple with
# the use of list
list1 = [1, 2, 4, 5, 6]
print("\nTuple using List: ")
print(tuple(list1))

# Creating a Tuple
# with the use of loop
Tuple1 = ('Geeks')
n = 5
print("\nTuple with a loop")
for i in range(int(n)):
    Tuple1 = (Tuple1,)
    print(Tuple1)

# Creating a Tuple with the
# use of built-in function
Tuple1 = tuple('Geeks')
print("\nTuple with the use of function: ")
print(Tuple1)

# Creating a Tuple with 
# Mixed Datatypes
Tuple1 = (5, 'Welcome', 7, 'Geeks')
print("\nTuple with Mixed Datatypes: ")
print(Tuple1)

# Creating a Tuple 
# with nested tuples
Tuple1 = (0, 1, 2, 3)
Tuple2 = ('python', 'geek')
Tuple3 = (Tuple1, Tuple2)
print("\nTuple with nested tuples: ")
print(Tuple3)

# Creating a Tuple 
# with repetition
Tuple1 = ('Geeks',) * 3
print("\nTuple with repetition: ")
print(Tuple1)


#OUTPUT
Initial empty Tuple: 
()

Tuple with the use of String: 
('Geeks', 'For')

Tuple using List: 
(1, 2, 4, 5, 6)

Tuple with a loop
('Geeks',)
(('Geeks',),)
((('Geeks',),),)
(((('Geeks',),),),)
((((('Geeks',),),),),)

Tuple with the use of function: 
('G', 'e', 'e', 'k', 's')

Tuple with Mixed Datatypes: 
(5, 'Welcome', 7, 'Geeks')

Tuple with nested tuples: 
((0, 1, 2, 3), ('python', 'geek'))

Tuple with repetition: 
('Geeks', 'Geeks', 'Geeks')
```

* Concatenation of Tuples<br>
**Note**- Only same datatypes can be combined with concatenation, an error arises if a list and a tuple are combined. 

```python
# Concatenaton of tuples
Tuple1 = (0, 1, 2, 3)
Tuple2 = ('Geeks', 'For', 'Geeks')

Tuple3 = Tuple1 + Tuple2

# Printing first Tuple
print("Tuple 1: ")
print(Tuple1)

# Printing Second Tuple
print("\nTuple2: ")
print(Tuple2)

# Printing Final Tuple
print("\nTuples after Concatenaton: ")
print(Tuple3)

##OUTPUT
#Tuple 1: 
#(0, 1, 2, 3)

#Tuple2: 
#('Geeks', 'For', 'Geeks')

#Tuples after Concatenaton: 
#(0, 1, 2, 3, 'Geeks', 'For', 'Geeks')
```

* Slicing of Tuple<br/>
**Note**- Negative Increment values can also be used to reverse the sequence of Tuples

```python
# Slicing of a Tuple
# with Numbers
Tuple1 = tuple('GEEKSFORGEEKS')

# Removing First element
print("Removal of First Element: ")
print(Tuple1[1:])

# Reversing the Tuple 
print("\nTuple after sequence of Element is reversed: ")
print(Tuple1[::-1])

# Printing elements of a Range
print("\nPrinting elements between Range 4-9: ")
print(Tuple1[4:9])

##OUTPUT
#Removal of First Element: 
#('E', 'E', 'K', 'S', 'F', 'O', 'R', 'G', 'E', 'E', 'K', 'S')

#Tuple after sequence of Element is reversed: 
#('S', 'K', 'E', 'E', 'G', 'R', 'O', 'F', 'S', 'K', 'E', 'E', 'G')

#Printing elements between Range 4-9: 
#('S', 'F', 'O', 'R', 'G')
```

* Deleting a Tuple<br>
Tuples are immutable and hence they do not allow deletion of a part of it. Entire tuple gets deleted by the use of del() method.<br>
**Note**- Printing of Tuple after deletion results to an Error.

```python
# Deleting a Tuple

Tuple1 = (0, 1, 2, 3, 4)
del Tuple1

print(Tuple1) # ERROR
```
![String Constants ](https://github.com/spiderOO7/python-reference-notes/blob/master/IMG/54.png "String Constant")
----
