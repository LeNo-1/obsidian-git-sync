#compSciMain 
## Intro
######  -Python was named after the comedy group "Monty Python"
Python  is good for people learning to code as it is:

- Very Concise **(Little amount of instructions)
- Can be used on different types of computers
- Excellent library of tools
- It is "Open source" meaning it costs nothing to download and can share codes for free

## Errors
###### -Syntax Errors
Syntax errors are errors caused by using the wrong syntax, *i.e. spelling, punctuation and capitalisation*, otherwise the code wont run

Example:
```python
Print(Hello World!)
# This code will not work as it has a capital "P"

print(Hello World!)
# This code will work as it has a lowercase "p"
```

###### -Logic Errors (Bugs)
Logic Errors or "bugs" are errors caused by a mistakes in the code leading to unwanted outputs *i.e. forgotten line of code, instructions in the wrong order or use the wrong operator*

## Variables
|-> In coding variables are used to record and store information.
||| Variables are temporary meaning they only exists while the program ||| runs.

###### Variables <mark style="background: #FF5582A6;">CANNOT</mark> :
- Start with a number *e.g. "1variable = 21"*
- Include spaces *e.g. " myName = DARA"*
- Include special characters such as @,/,- *e.g. "@gmail = mail"*
- Include python keywords *e.g. "print = 1"*

###### Types of Variables
```Python
"Types of Variables"
Integer - int # Whole Numbers
Float - float # Decimal numbers
String - str # Text
Booleen - bool # True or false

type() # Finds the variable type of variable in its brackets 

\"Printing Variables"
# Example
x = 5
y = 7
z = 9
print("The answer is:", x, y, z)

The answer is 5 7 9
```

#### Calculations on Variables

| **Operator** | **Symbol** |     |     |
| ------------ | ---------- | --- | --- |
| *Add*          | +          |     |     |
| *Subtract*     | -          |     |     |
| *Multiply*     | *          |     |     |
| *Divide*       | /          |     |     |
| *Floor divide* | //         |     |     |
| *Modulus*      | %          |     |     |
| *Exponent*     | **         |     |     |
##### Incrementing
->The code x=x+1 is used a lot in programming
||but python provides other ways to do this.

| **Statement** | **Example** | **Equivalent to** |
| :-----------: | :---------: | :---------------: |
|      +=       |    x+=5     |       x=x+5       |
|      -=       |    x-=5     |       x=x-5       |
|       =       |    x*=5     |       x=x*5       |
|      /=       |    x/=5     |       x=x/5       |
|      //=      |    x//=5    |      x=x//5       |
|      %=       |    x%=5     |       x=x%5       |
|      **=      |    x**=5    |      x=x**5       |
## Loops
### While loops
A while loops keeps repeating while a certain condition is true and stops when its is false.
```Python
counter = 0
while counter < 7:
    print(counter)
    counter+=1
print("Im glad that loop is finished")
```
### For Loops
Unlike while loops, for loops are given a specific number of times to repeat.
#### Basic For Loops
```Python
for y in range(1,5):
    print(y)
```


| rang()              | Example                                    | Explanation                                            |
| ------------------- | ------------------------------------------ | ------------------------------------------------------ |
| **One argument**    | ***for y in range(5):<br>print(y)***       | Lists the integers from 0 up to but not including 5.   |
| **Second argument** | ***for y in range(1,5):<br>print(y)***     | Lists integers from 1 up to but not including 5.       |
| **Three arguments** | ***for y in range(1,10,2):<br>print(y)***  | Lists 1 to 9 in steps of 2.                            |
| **Going backwards** | ***for y in range(10,0,-1):<br>print(y)*** | Lists integers from 10 to 1, in steps of 1, backwards. |

### Nested Loops

## Lists
A list can be used to store a collection of data items and to keep them in order if necessary
- A Lists begins and ends with closing square brackets
```Python
colour = ["red", "green", "blue"]
```
