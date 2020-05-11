# Python-basic
I made a list of all the basic operations of python program. 
The file contains,
1. #### Comment
1. #### data type
1. #### arithmetic operators
1. #### assignment operators
1. #### comparison operators
1. #### logical operators
1. #### variables
1. #### printing anything
1. #### input anything
1. #### if else
1. #### for loop
1. #### function
1. #### list


### Before starting

The extension of python is '.py'. 
Example:

text_file.py

To run a python file you need to open cmd on the same directory of the file and you have to type python 
```
<your_file_name.py>
```

Example:
```
python text_file.py
```

### Comment

Comments starts with a #, and Python will ignore them.

Example:
```python
# This is a comment.
```

### Data type

```
Text Type:	
str # string
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
```

### Arithmetic operators

| Operators  | Name    |  Example  |   
|---|---|---|
|- |Addition|x-y|
|+ |Subtraction|x+y|
|* |Multiplication|x*y|
|/ |Division|x/y|
|% |Modulus|x%y|
|**  |Exponentiation|x**y|

### Assignment operators

| Operators  | Example     |  Same as  |   
|---|---|---|
|= |x=5|x=5|
|+= |x+=5|x=x+5|
|-= |x-=5|x=x-5|
|*\=|x*=5|x=x*5|
|/= |x/=5 |x=x/5|
|%=  |x%=5 |x=x%5|
|**=  |x**=5 |x=x**5|

### Comparison operators

| Operators  | Name    |  Example  |   
|---|---|---|
|== | Equal|x==y |
|!= |Not equal|               x!=y|
|>  |Greater than|            x>y|
|<  |Less than     |          x<y|
|<= |Less than equal|         x<=y|
|>= |Greater than equal|      x>=y|


### Logical operator

|operators|      description|      example|
|---|---|---|
|and                  |Returns True if both statements are true.       |x<5 and x>8|
|or                   |Returns True if one of the statements is true.  |x<5 or x>8 |
|not                   |Reverse the result, returns False if the result is true.   |not(x<5 or x>8)|


### Variables

We don't need to specify variables type in python. Python detects it automatically.

Example:

```python
var1= "My name is Nahib" # Detects as string.

var2= 10 # Detects as int.

var3= 13.434 # Detects as float.

var4= False # Detects as bool.
```

### Printing anything

To print any thing we have to use print(). We have to use "" to show something in it.

Example:

```python
print("hello world")
```

We can also use \n in it to show new line.

Example: 
``` python
print("hello world\nI am the new line")
```

### Input anything

For input any thing we use input(). By python inputs string value.
Example:

```python
print("What is your name?")
name = input()
print("My name is "+ name)
```

We can also use inline command to get input in a single line with the question.
Example:

```python
name = input("Name= ")
print("My name is "+ name)
```

For int and float we need to convert the default string input to int or float.
Example:
```python
var1= int(input("Enter first number: "))
var2= int(input("Enter second number: "))
sum= var1+var2
print("The ans is ", sum) # we have used comma before sum because, we can not concatenate int/float to string.
print("The ans is "+ str(sum)) # we have + before sum because, we can have concatenate int to string using str.
```

Example:
```
 Q. Find area of a circle. Here, r= user defined and pi= 3.14.
```
```python
r= float(input("Value of R= "))
pi= 3.14
print(r*r*pi
```

### if else  

The syntax of if else is:
```python
if expression1:
    statement(s)
elif expression2:
    statement(s)
else:
    statement(s)
```

>Python uses : rather than () and {}. Here spacing  is mandatory. Without spacing the program will not work properly (1 tab).

Example:
```python
a= int(input("Input the value of a: ")) 
b= int(input("Input the value of b: "))

if a>b:
    print(a)
    print("A wins.")

    elif a<b:
        print(b)
        print("B wins.")

    else:
        print("both are equal")
```

### While loop 


The syntax of while loop is: 
```python
while expression:
    statement(s)
```

Example:
```python
i= 1

while i< 7:
    print(i)
    i+=1
```

Example:
```python
i = 1
while i <=6:
    print(i)
    i += 1

print("i is no longer less than 6")
```

### for loop 

Before knowing about for loop we have to understand range() function first. 
The ```range()``` function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and ends at a specified number.
We normally use range for using for loops. The syntax of range is range(start, stop, step).

>Note:(
    start	Optional. An integer number specifying at which position to start. Default is 0
    stop	Required. An integer number specifying at which position to end.
    step	Optional. An integer number specifying the incrementation. Default is 1
    )


for loop syntax:
```python
for s in expression:
    statement(s)
```
Example:
```python
for i in range(20): # it will show value of i from 0 to <20
    print(i)
```


We can also print char of a string using for loop.

Example: 
```python
for i in "Nahib":
    print(i)
```
Example of range:
```python
for n in range(3, 20, 2): # Starts form 3, stops at 19, steps=2
    print(n)
```

### function 

In Python a function is defined using the def keyword.
The syntax of function is:
```python
def functionname( parameters ):
    "function_docstring"
    function_suite
    return [expression]
```

>Note: function must be called.

Example:
```python
# function expression part. 
def hello(): 
    print("Hello world")

    hello() # function is called.
```
This program is called by hello() and it prints the string named "Hello world". It returns noting.

Lets see a function that will receive a string.

Example:
```python
def stringRes(receive): # you can use any thing in parameter. I have used receive.
    print(receive)

stringRes("Hello")
```
Lets return something using string.

Example:
```python
def add(a, b):
     return a+b

x = add(
    int(input("a: ")),
    int(input("b: "))
    )

print(x)
```
### List 

Python does not have built-in support for Arrays, but Python Lists can be used instead.
List is a collection which is ordered and changeable. Allows duplicate members.
List can be anything. It can be number or string.
>List supports negative indexing. -1 means last item of the list -n means nth position item (form the end to begin) in the list.

List syntax:
```python
var_name=  ['elements'] # list starts with []
```
Example:
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12] 

email= ["ab@ab.com", "cd@cd.com"]
```

List starts with 0.

To access list we have to reffer its name. 

Example:
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]

print(List[3]) # shows the element of index 3.

print(List) # will show full list.

print(len(List)) # list length.
```
Example:
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]

for i in List:
    if i%2 ==0:
        print(i) # prints even form list.
```
Some functions of List:
* append():append() is used for adding element at the last of the list.

Example:
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
List.append("ok") # we have added 'ok' at the end of the list.
print(List) 
```

* insert():
    insert() is used to insert element at a specific position.

Example: 
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
List.insert(0, "start") # inserts "start" at position 0
print(List)
List.insert(12, "before 12") # inserts "start" at position 12
print(List)
```
* extend([]):
    extend() is used to add multiple elements at the same time at the end of the list.

Example:
```python
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
List.extend(["I", "am", "in", "a", "list"])
print(List)
```

* remove():
    remove() method removes the specified item (not index) from the list and shows error if the item is not exists.

Example:
```python        
List = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
List.remove(2)
print(List)
```



