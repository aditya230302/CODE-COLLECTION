# **Introduction**
- Developed by **Guido Van Rossum**
- It is an high level interpreted language.
  - **Interpreted Language** : Where the code is executed line by line by an interpreter, rather than being compiled into machine code all at once (like a compiled language).
  - **High Level Language**  : The language understandable by humans.
  - **Low Level Language**   : The language understandable by machines.
- Python is case sensitive (`a` and `A` both are different)
- Follows `Indentation` (spacing/tabs)
- `#` > comments : notes or lines that are not part of the code.
- `Ctrl + /` : For making multiple lines comment together at once.
- **Why we use Python ?**
  - Simplicity
  - Machine Learning, AI
  - Vast amount of libraries (numpy,pandas,etc)

---
# **Variables**
- Containers that stores information or values.
- It is memory location that stores information.
- We can change the value os the variable, it is not fixed.
```py
# Syntax
variable_name = value

# example
a = 10
print(a)
```
> `print()` command is used to print the value as an output

### **3 Golden Rules for using Variables**
1. Keyword can't be used as the name of variable. Keywords are registered words in python. `Example : in, for, while, if, else, etc.` 
2. Variables can start with letters but can't start with numbers.
3. We can't start with or use special symbols : `@, #, $, *`

### **Ways of assigning a value to a variable**
1. **Static Way**  : When we directly assign the value.
2. **Dynamic Way** : We execute the code and then value is assigned by the user.
```py
# Static way
a = 10

# Dynamic way
a = input()
```
> `input()` by default takes input in string (combination of characters) data type

---
# **Operators**
1. **Arithmatic Operators** : `+`, `-`, `*`, `%`, `/`, `//`
2. **Logical Operators**    : `and`, `or`, `not`
3. **Comparison Operators** : `<`, `>`, `>=`, `<=`, `==`, `!=`
4. **Assignment Operators** : `=`, `+=`, `-=`, `*=`, `/=`

### **Arithmatic Operators**
- They are used to do arithmatic operations.
1. `+` : Addition
2. `-` : Subtraction
3. `*` : Multiplication
5. `%` : Remainder (30 % 2 = 0, 30 % 1 = 1)
7. `/` : Float Division (Decimal value as an output : 15/9 = 1.6666666...)
8. `//`: Floor Division (Integer value as an output : 15//9 = 1.0, 15.66//1 = 15.0)

### **Logical Operators**
- They are used to check conditions.
1. `and` : Both conditions must be true.
2. `or`  : Any one condition must be true
3. `not` : Conditions must be false
```py
a = True
b = False
print(a and b) # False
print(a or b)  # True
```

### **Comparison Operators**
- To compare values.
1. `<` : Less than
2. `>` : Greater than
3. `<=`: Less than and equal to
5. `>=`: Greater than and equal to
6. `==`: Equal to
7. `!=`: Not equal to

### **Assignment Operators**
- To assign values.
1. `=` : Assign value equal to
2. `*=`: Multiply with same value and assign (a = 10, b = 2, `a *= b` => `a = a*b` => a = 20)
3. `/=`: Divide with same value and assign (a = 10, b = 2, `a /= b` => `a = a/b` => a = 5.0)
4. `+=`: Add with same value and assign (a = 10, b = 2, `a += b` => `a = a + b` => a = 12)
5. `-=`: Subtract from same value and assign (a = 10, b = 2, `a -= b` => `a = a - b` => a = 8)

---
# **Data Types**
- A data type is an attribute associated with a piece of data that tells a computer system how to interpret its value.
1. **Integer** : 1, 2, 3, 4, etc.
2. **Float**   : decimal values => 1.2, 3.4, 5.6, etc.
3. **String**  : 'Aditya', 'Axel', etc.
4. **Boolean** : `True`, `False`
> There is no character data type in python.
- `type()` function is used to check the data type of a value.
```py
a = 3.2
type(a) # Float
```
### **Type Casting**
- It is the process of converting ine data type to another
```py
a = input()        # String
b = int(input())   # Integer
c = float(input()) # Float
d = int(c)         # Integer
```

---
# **Indexing**
* **Index**    : It is the position of a value (starting from 0)
* **Indexing** : It is the process of excessing or extracting the element at a particular position.
```py
# Syntax
variable_name[index]

# Example
a = 'Aditya'
a[0] # A
a[1] # d
a[2] # i
a[3] # t
a[4] # y
a[5] # a
```
1. **Forward Indexing**  :   0   1  2  3  4  5  6  7  8  9  10
2. **Backward Indexing** : -11 -10 -9 -8 -7 -6 -5 -4 -3 -2  -1

![image](https://github.com/user-attachments/assets/77579852-f3ad-4764-85ee-0f43ddf6e14f)

---

# **Slicing**
- If we have to extract one or more than one element from the collection.
```python
# Syntax
variable_name[start_index_number : end_index_number]
```
> last index number is not included
```py
# Example
a = 'INTELLIPAAT'
a[0:4] # INTE
a[3:6] # ELL
```
> if we are not giving eny start index value it will start from the begining
> if we are not giving any end index value it we go till the end
```py
a[:4]  # INTE
a[7:]  # PAAT
a[:]   # INTELLIPAAT
```
> Slicing will not give error in case we are giving out of bound (extra) indexing, instead it will show blank output.
```py
a[10:15] # T
```

---

# **Step Indexing**
- steps : by how many levels we want to jump the index
```py
# Syntax
variable_name[start : end : steps]

# Example
a = 'INTELLIPAAT'
a[::2]  # ITLIAT
a[::-1] # TAAPILLETNI
```
> `a[::-1]` reverses the string

---

# **Collective and Sequential Data Types**
- String, List, Tuple, Set, Dictionary.

### **1. List**
- Contains different types of data.
- Ordered and mutable
```py
# Syntax
L = []  # Empty List
type(L) # list

# Example
L = [10, 20, 30, 40, 2.3, 4.5, 'suraj', 'python', 'apple']
# List Indexing
L[0]  # 10
# Reverse Indexing
L[-1] # 'apple'
# Slicing
L[:4] # [10, 20, 30, 40]

# Changing a value un list
L[1] = 200          # [10, 200, 30, 40, 2.3, 4.5, 'suraj', 'python', 'apple']
L[1:3] = ['f', 'g'] # [10, 'f', 'g', 40, 2.3, 4.5, 'suraj', 'python', 'apple']
```
- **append(value)** : accepts one argument and insert it at the end of the list
```py
L.append('virat') # [10, 'f', 'g', 40, 2.3, 4.5, 'suraj', 'python', 'apple', 'virat']
```
- **insert(index_number, value)** : insert value at the mentioned index number, and shift the original value at that place by 1 position to left.
```py
# Syntax
list.insert(index_number, value)

# Example
l = [1, 2, 3]
l.insert(1, 'apple') # [1, 'apple', 2, 3]
```
- **extend(list)** : add 2 lists together to make 1 list.
```py
l1 = [1, 'suraj', 2, 3, 4]
l2 = [2.3, 3.4, 4.5]
l1.extend(l2) # [1, 'suraj', 2, 3, 4, 2.3, 3.4, 4.5]
# l1 + l2 is same as l1.extend(l2)
```
- **remove(value)** : Just to delete the value from the list
```py
L.remove('suraj')
print(L) # [10, 20, 30, 40, 2.3, 4.5, 'python', 'apple']
```
- **pop(index)** : remove as well return the value and it accepts index number
```py
L.pop(1) # 'apple'
```
- **clear()** : Delete all the values of the list.
```py
L.clear()
```
- **del** : delete list.
```py
del L1
```

### **2. Tuple**
- Collection of hetrogenous data types.
- Ordered data types.
- Immutable : we can't update the values of tuples directly.
```py
# Syntax
t = ()
type(t) # tuple

# len() : helps to get the no. of elements
len(t)
# Example
t = (1,2,3)
t[2] # 3
t[2] = 789 # Error
```
- If we need to update the value of a tuple we first convert it to list
```py
convert_tuple_to_list = list(t)
convert_tuple_to_list[2] = 987
t = tuple(convert_tuple_to_list)
t # (1,2,987)
```
- Combining two tuples
```py
t1 = (1,2,3)
t = t + t1
t # (1,2,987,1,2,3)
```

### **3. Set**
- Collection of hetrogenous data types
- Unordered : will not have index values
- mutable data type : can be changed
- don't have duplicates
```py
# Syntax
S = {1,2,3,4.4,5.5,'suraj','python'}
type(S) # set

# Slicing
S[3] # Error
```
- **add(value)** : to add value
```py
S.add(100)
S.add('S')
S # {1,100,2,3,4.4,5.5,'python','S','suraj'}
```
- **remove(value) : To remove value
```py
S.remove(100)
```
- **union(set)** : To join all the values of 2 sets without duplicates
```py
S1 = {1,2,3,4,5,6,7}
S2 = {1,2,3,4,9,10,11}
S1.union(S2) # {1,2,3,4,5,6,7,9,10,11}
```

### **4. Dictionary**
- key   : User defined index value
- value : Value that we want to share
```py
# Syntax
D = { key1 : value1,
      key2 : value2,...}
# Empty dictionary
d = {} 
type(d) # dict

# Example
d = {'name'   : 'suraj',
     'age'    : 30,
     'weight' : 78}
d['age']  # 30
d['name'] #'suraj'
```
- **values()**
```py
h = {'name' : ['suraj', 'adi', 'kunal'],
     'age'  : [23,34,45]}
h.values() # dict_values([['suraj','adi','kunal'],[23,34,45]])
```
- **Keys()**
```py
h.keys() # dict_keys(['name','age'])
```
- **items()**
```py
h.items() # dict_items([('name',['suraj','adi','kunal']), ('age', [23,34,45])])
```

---

# **Coditional Statements / Loops**
### **1. if-else**
```py
# Syntax
if(condition): # if condition is true
  task 1 code
else : # if condition is false
  task 2 code
```

### **2. More than one if-else loop : elif/else if**
```py
if(condition1):
  code
elif(condition2): # else if
  code
.
.
.
else : # final when all above conditions are false
  code
```

### **3. for loop**
- It works with range
```py
# Example
for i in range(10): # last element of range is not considered
  print(i) # 0 1 2 3 4 5 6 7 8 9
```

### **4. while loop**
- works with condition
```py
# Syntax
while(condition):
  code
  increment/decrement

# Example : write a program to write/print the table of any number
num = int(input("enter the number : "))
i = 1
while(i<=10):
  print(f"{num}*{i} = {num*i}")
  i = i+1
```

---

# **User Defined Functions**
- **def** : keyword, which we use to create a function
```py
# Syntax
def function_name(parameters):
  code

# calling function
function_name(parameters by user)
```
---

# **Lambda Function**
- nameless function, so we need to store them in a variable
- one line function
```py
# Example
adder = lambda a,b,c : a+b+c
square = a : a*a

# Calling Lambda Function
adder(1,2,3) # 6
square(3) # 9
```

---

# **OOPs : Object Oriented Programming**
- It is a concept or an approach where everything is represented in the form of classes and objects.
- **Classes** :
  - Collection of objects.
  - It contains the blueprint of the program.
- **Object** :
  - Objects are the instance of the class
  - instance : It represents a concrete realization of the class and has its own unique state
- There are 4 main pillars of OOPs:
1. **Inheritance**   : Passing the properties from parent to child
2. **Polymorphism**  : Multiple Forms
3. **Abstraction**   : Showing only information relevant to the user, all the information that is not required by the user is hidden.
4. **Encapsulation** : To bundle data and methods into easy to use units.
```py
# Syntax
class class_name:
  code

object_name = class_name()

# Example
class number:
  a = 10
  b = 20

obj1 = number()
obj1.b # 20
obj1.a # 10
```
- Each class can have multiple objects but that might create a bit of confusion.
- We can access both variables and function of a class using object

- **self** :
  - It is a special paramter that gives refrence to the current instance.
  - Without self paramter it will show `TypeError : classfunc1.func1() takes 0 positional arguments but 1 was given`
  - We will get an error because when we call a function, the function by default takes an argument that is the refence of object to class to access the function.
```py
class classfunc1:
  def func1(self):
    print("Hello")

Obj2 = classfunc1()
Obj2.func1() # "Hello"
```
- Whenever we call a function, an object reference will always be passed, that is 1 more argument, so we need self keyword.
- If we only call object, it will show memory refrence.
```py
obj2 # <main_.classfunc1 at 0x1d76...>
```

- **__init__** :
  - 
