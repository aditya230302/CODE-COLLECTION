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
