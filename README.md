# python1
2.1 python function(argument types...)

A function is a bloke of code which only runs when it is called

how to create a function? in python a function is defined using the def keyword:

how to calling a function? to call a function name followed by parenthesis

Arguments in python is information can be passed in to functions as arguments

```jsx
#creating a function
def myfun():
     print("Hello world")
#function calling
myfun() 
    #output
Hello world

```

```jsx
#functionArgument/parameter
der comp_prog(lang):
     print(lang +"programming")
comp_prog("c++")
comp_prog("java")
comp_prog("pyhton")
#output
c++ programming
java programming
pyhton programming

```

```python
# crate a function that add two number and return sum
def add (num1,num2)
     print(num1+num2)
add(10,8)
#output is
18

```

2.2 python anonymous function lambda

```python
#symple lambda function
x=lambda y:y+20
print(x(15))
#the output is 35

#multiple three number and return result
 mul=lambda x,y,z:x*y*z
print(mul(5,6,7))
#the output is 210

#lambda inside a function
def multiple(k):
     return lambda x:x*k
product=multiple(3) #the k value
print(product(7))# the x value
print(product(10))
#yhe output is 7*3=21
                10*3=30 ....etc  

```

function lambda

```jsx
#simple lambda function
x=lambda y:y+20
print(x(15))
#multiple three numbers and result
mul=lambda x,y,z:x*y*z
print(mul(5,6,7))
#lambda inside a function
def multiple(k):
    return lambda x:x*k
product=multiple(3)
print(product(3))
```

map() function in python

map() function takes another function and a sequence of iterables as parameters and retuns the output after execution the function to each item in the sequence

```python
#Map
def add(a):
    return a+a
numbers=(4,6,8,9)
out=map(add,numbers)
print(out)
add=list(out)
print(add)

#output
(8,12,16,9)

numbers=(4,6,8,9)
out=map(lambda a:a*a,numbers)
print(out)
mul=list(out)
print(mul)

#output
[16,36,64,81]

```

filter() function in python

python filter() function provide filtereds elements. the function also takes another function and a sequence of iterables as parameterss.the filter function returnd a sequence for which function returns true

```python
def fil(a):
    if a>5:
        return a
out=filter(fil,(1,4,7,3,9))
print(list(out)) 
y=filter(lambda a:(a>5),(1,4,7,3,9))
print(list(y))

#output
[7,9]
[7,9]

```

reduce() function in python

python reduce() function provides a single value on exexcution . this function also takes another function and a sequence of iterables as parameters. the function tools module must be used to improt this function

> syntax:reduce(function,iterables)
> 

```python

```

```python
from functools import reduce
reduce(lambda a,b:a+b,[10,35,50,20])

reduce(lambda a,b:a*b,[9,7,23,4])
```
