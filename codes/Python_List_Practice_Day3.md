Lists in Python

A built-in data type that stores set of values

It can store elements of different types (integer, float, string, etc.)


```python
marks1 = 99.4
marks2 = 87.5
marks3 = 95.2
marks4 = 66.4
marks5 = 45.1

marks = [94.4, 87.5, 95.2, 66.4, 45.1]
print(marks)
print(type(marks))
print(marks[0])
print(marks[1])
```

    [94.4, 87.5, 95.2, 66.4, 45.1]
    <class 'list'>
    94.4
    87.5
    


```python
student = ["karan", 95.4, 17]
print(student)
```

    ['karan', 95.4, 17]
    

Strings --> immutable
Lists --> mutable


```python
student = ["karan", 95.4, 17]
print(student)
```

    ['karan', 95.4, 17]
    


```python
student = ["karan", 95.4, 17]
student[1] = "arjun"
print(student)
```

    ['karan', 'arjun', 17]
    
List Slicing
Similar to String Slicing
List_name[starting_idx:ending_idx #ending idx is not included]


```python
marks = [87, 67, 98, 56, 83]
print(marks[1:4])
```

    [67, 98, 56]
    


```python
marks = [87, 67, 98, 56, 83]
print(marks[-4:-2])
```

    [67, 98]
    

List Methods


```python
list = [2,1,3]
list.append(4) #adds one element at the end []2,1,3,4]
```


```python
list.sort() #sorts in ascending order [1,2,3]
```
list.sort(reverse=True) #sorts in descending order [3,2,1]

```python
list.reverse() #reverses list [3,2,1]
```


```python
list.insert(idx,el) #insert element at index
```


```python
list.remove(1)
```


```python
list.pop(idx)
```


```python
#Example of Append the list
list = [2,1,3]
list.append(4)
print(list)
```

    [2, 1, 3, 4]
    


```python
#example of Sort the list
list = [2,1,3,6,5,9,7]
list.sort()
print(list)
```

    [1, 2, 3, 5, 6, 7, 9]
    


```python
#example of Sort (reverse = True)
list = [2,1,3,6,5,9,7]
list.sort(reverse=True)
print(list)
```

    [9, 7, 6, 5, 3, 2, 1]
    


```python
#example of sort (reverse) the list
list = [2,1,3,6,5,9,7]
list.reverse()
print(list)
```

    [7, 9, 5, 6, 3, 1, 2]
    


```python
#example of list.insert(idx,el) #insert element at index
list = [2,1,3,6,5,9,7]
list.insert(3, 9)
print(list)
```

    [2, 1, 3, 9, 6, 5, 9, 7]
    


```python
#example of list.remove(1) method
list = [2,1,3,6,5,9,7]
list.remove(6)
print(list)
```

    [2, 1, 3, 5, 9, 7]
    


```python
#example of list.pop(idx) method
list = [2,1,3,6,5,9,7]
list.pop(5)
print(list)
```

    [2, 1, 3, 6, 5, 7]
    

Tuples in Python

A built-in datatype that lets us create immutable sequences of values. List if mutable
tup = (87, 64, 33, 95, 76) #tup[0], tup[1]....
tup[0] = 43 #NOT allowed in python

```python
tup = (2,1,3,1)
print(tup[0])
print(tup[1])
tup[0] = 5 #tupple is immutable hence cannot chnage the list
```

    2
    1
    


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[25], line 4
          2 print(tup[0])
          3 print(tup[1])
    ----> 4 tup[0] = 5
    

    TypeError: 'tuple' object does not support item assignment



```python
tup = ()
tup1 = (1,)
tup2 = (1)
tup3 = (1,2,3,4,5)
print(tup3[2:5])
print(tup2)
print(tup)
print(tup1)
print(type(tup1))
print(type(tup2))
print(type(tup))
```

    (3, 4, 5)
    1
    ()
    (1,)
    <class 'tuple'>
    <class 'int'>
    <class 'tuple'>
    

#Tuple Methods

tup = (2,1,3,1)
tup.index(el) #returns index of first occurence tup.index(1) is 1
tup.count(el) #counts total occurrences tup.count(1) is 2

```python
#example of tuple indexing
tup = (2,1,3,4)
print(tup.index(2))
print(tup.index(4))
```

    0
    3
    


```python
#example of tuple count
tup = (2,1,3,1)
print(tup.count(1))
```

    2
    

Q. Write a program to ask the user to enter names of their 3 favorite movies & store them in a list.


```python
list = ["3 Idiots", "Sholey", "Bahubali"]
print(list)
print(type(list))
```

    ['3 Idiots', 'Sholey', 'Bahubali']
    <class 'list'>
    


```python
a = "3 Idiots"
b = "Sholey"
c = "Bahubali"
print(list.append("Ramayan"))
```

    None
    


```python
movies = []
mov1 = input("enter 1st movie:")
mov2 = input("enter 2nd movie:")
mov3 = input("enter 3rd movie:")

movies.append(mov1)
movies.append(mov2)
movies.append(mov3)
print(movies)
```

    enter 1st movie: Sholey
    enter 2nd movie: Bahubali
    enter 3rd movie: 3 Idiots
    

    ['Sholey', 'Bahubali', '3 Idiots']
    


```python
movies = []
mov = input("enter 1st movie:")
movies.append(mov)
mov = input("enter 2nd movie:")
movies.append(mov)
mov = input("enter 3rd movie:")
movies.append(mov)

print(movies)
```

    enter 1st movie: Sholey
    enter 2nd movie: Bahubali
    enter 3rd movie: 3 Idiots
    

    ['Sholey', 'Bahubali', '3 Idiots']
    


```python
movies = []
movies.append(input("enter 1st movie:"))
movies.append(input("enter 2nd movie:"))
movies.append(input("enter 3rd movie:"))

print(movies)
```

    enter 1st movie: Sholey
    enter 2nd movie: Bahubali
    enter 3rd movie: 3 Idiots
    

    ['Sholey', 'Bahubali', '3 Idiots']
    

Q. Write a program to check if a list contains a palindrome of elements. (Hint:use copy() method)

[1,2,3,2,1]                  [1, "abc", "abc", 1]


```python
list1 = [3,2,1]
list2 = [1,2,3]

copy_list1 = list1.copy()
copy_list1.reverse()
print(copy_list1)

if(copy_list1 == list1):
    print("palindrome")
else:
    print("Not palindrome")
```

    [1, 2, 3]
    Not palindrome
    

Q. Write a program to count the number of students with the "A" grade in the following tuple.

["C", "D", "A", "A", "B", "B", "A"]


```python
stu = ["C", "D", "A", "A", "B", "B", "A"]
stu.count("A")
print(stu.count("A"))
```

    3
    

Q. Store the above values in a list & sort them from "A" to "D".


```python
Stu = ["C", "D", "A", "A", "B", "B", "A"]
Stu.sort()
print(Stu)
```

    ['A', 'A', 'A', 'B', 'B', 'C', 'D']
    
