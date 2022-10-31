# Python W2 - Assignment 01 (Mandatory)

### 1. String Manipulation (Total marks 1)

Match the following string methods with the respective output in the below options

Here,
 `string= "this is old python course"`

| Statement | Output |
| --- | --- |
| (a) string.count("is") | (1) True |
| (b) string.replace("old", "new") | (2) 12 |
| (c) string.index("python") | (3) 'this is new python course' |
| (d) string.startswith("this") | (4) 2 |
| (e) string.isalnum() | (5) False |
| (g) string.strip("this is old") | (6) 'python course' |

#YOUR ANSWER HERE
(a) string.count("is")--------> (4)2
(b) string.replace("old", "new")--------> (3)'this is new python course' 
(c) string.index("python")-----------> (2)12
(d) string.startswith("this")---------> (1)True	
(e) string.isalnum()------------>(5) False
(g) string.strip("this is old")--------->	(6)'python course'


```python
string="this is old python course"
```


```python
string.count("is")
```




    2




```python
string.replace("old","new")
```




    'this is new python course'




```python
string.index("python")
```




    12




```python
string.startswith("this")
```




    True




```python
string.isalnum()
```




    False




```python
string.strip('this is old')
```




    'python course'



### 2. Nested Conditions (Total marks 1)





```python

x = int(input())
y = int(input())
z = int(input())

#Block-1 Start

if x > 0 or y> 0 or z > 0:
    if (x > 0 and y> 0) or (y> 0 and z> 0) or (z> 0 and x > 0):
        if x > 0 and y> 0 and z > 0:
            print('P3')
        else:
            print('P2')
    else:
        print('P1')

#Block-1 End


# Block-2 Start

if x <0 or y<0 or z < 0:
    if (x < 0 and y< 0) or (y< 0 and z< 0) or (z< 0 and x < 0):
            if x < 0 and y< 0 and z < 0:
                print('N3')
            else:
                print('N2')
    else:
        print('N1')


#Block-2 End
```

What will be the output for the below input of x,y and z?

x= -1
y= 4
z= 1

#YOUR ANSWER HERE
Output of Block1-----------> P2
Output of Block2-----------> N1


**Block1**


```python
x = int(input("x:"))
y = int(input("y:"))
z = int(input("z:"))

if x > 0 or y> 0 or z > 0:
    if (x > 0 and y> 0) or (y> 0 and z> 0) or (z> 0 and x > 0):
        if x > 0 and y> 0 and z > 0:
            print('P3')
        else:
            print('P2')
    else:
        print('P1')
```

    x:-1
    y:4
    z:1
    P2
    

**Block2**


```python
x = int(input("x:"))
y = int(input("y:"))
z = int(input("z:"))

if x <0 or y<0 or z < 0:
    if (x < 0 and y< 0) or (y< 0 and z< 0) or (z< 0 and x < 0):
            if x < 0 and y< 0 and z < 0:
                print('N3')
            else:
                print('N2')
    else:
        print('N1')
```

    x:-1
    y:4
    z:1
    N1
    

### 3. String slicing (Total marks 2)



```python
a = int(input())

b= int(input())

c= int(input())

d = int(input())

e = int(input())

print(s[-a:-len(s):-3])

print (s[::-b])

print (s[c:0:-3])

print (s[len(s): - d:-3])

print (s[:e:-3])
```

Consider that the string `s='abcdefghijklmnopqrstuvwxyz'`\
For what user input of a, b, c, d and e (where 0 <= a,b,c,d,e< len(s) ) does the above code-snippet print following output?\
It is a Numerical Answer Type (NAT) question. Enter your input value separated by, without any space like: 7,15,0,4,0

`zwtqnkheb`

`zwtqnkheb`

`zwtqnkheb`

`zwtqnkheb`

`zwtqnkheb`

#YOUR ANSWER HERE

To get the desired result "zwtqnkheb"  of all, inputs have to take----------> a=1, b=3, c=26, d=0, e=0


```python

s='abcdefghijklmnopqrstuvwxyz'
a = int(input("a="))

b= int(input("b="))

c= int(input("c="))

d = int(input("d="))

e = int(input("e="))

print(s[-a:-len(s):-3])

print (s[::-b])

print (s[c:0:-3])

print (s[len(s): - d:-3])

print (s[:e:-3])
```

    a=1
    b=3
    c=26
    d=0
    e=0
    zwtqnkheb
    zwtqnkheb
    zwtqnkheb
    zwtqnkheb
    zwtqnkheb
    

### 4. Code Brackets (Total marks 2)

Consider the program in the code cell below;


```python
match= False
if s.count('(') == s.count(')'):
    if s.count('{') == s.count('}'):
        if s.count('[') == s.count(']'):
            match = True
```

If s = "abcd(efgh(ijkl}{{}))" what will be the value of match at the end of execution and justification?

1. False, the number of opening and closing brackets are only considered
2. False, the position of opening and closing brackets are not considered.
3. True, the number of opening and closing brackets are only considered
4. True, the number and position of opening and closing brackets are considered.


#YOUR ANSWER HERE
Ans: 3.True, the number of opening and closing brackets are only considered


```python
s="abcd(efgh(ijkl}{{}))"
match= False
if s.count('(') == s.count(')'):
    if s.count('{') == s.count('}'):
        if s.count('[') == s.count(']'):
            match = True
print(match)
```

    True
    

## Programming Questions

Instructions:
- Enter your solution in the cell block below only. Double click to edit.
- Do not edit anything else apart from 'YOUR ANSWER HERE' for your solution


```python
#YOUR ANSWER7 HERE
```

### 5. Accept a sentence as input and find the number of words in it. Assume that the sentence has no punctuation marks (Total marks 2)


Example:

what a shot - 3 words

this is a chair - 4 words


```python
#YOUR ANSWER HERE
sen="python is platform independent language"
num=len(sen.split(' '))
print("The number of words in this sentence is:",num)
```

    The number of words in this sentence is: 5
    

### 6. Sandwich number (Total marks 2)

A three digit number is called a sandwich number if the difference between its first and last digit is equal to its middle digit. Accept a three digit number as input and print “sandwich” if the number is a sandwich number. Print “plain” if the number is not a sandwich number. For example, 123 and 853 are sandwich numbers.


```python
#YOUR ANSWER HERE
a=int(input("Put a number you want to check="))

#print("value of a=",a)
b=(a%10)
c=(a//10)
d=(c%10)
e=(c//10)
f=(e%10)
if(d==b-e or d==e-b):
 print("sandwich")
else:
  print("plain")
```

    Put a number you want to check=358
    sandwich
    
