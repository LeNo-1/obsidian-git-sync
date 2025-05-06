---
sticker: lucide//code-2
---
*====

**Table of Contents**

1. [Variables and Data Types](#variables-and-data-types)
2. [Operators](#operators)
3. [Control Structures](#control-structures)
4. [Functions](#functions)
5. [Pointers](#pointers)
6. [Arrays and Vectors](#arrays-and-vectors)
7. [Structures and Unions](#structures-and-unions)

**Variables and Data Types**
----------------------------

### Variables
In C, a variable is a name given to a location in memory where a value can be stored.

*   **Declaring variables**: The `int` keyword is used to declare an integer variable.
    ```c
    int x;
    ```
*   **Assigning values**: A value is assigned to a variable using the assignment operator (=).
    ```c
    x = 10;
    ```

### Data Types
C has several built-in data types:

*   **Integers** (`int`): whole numbers, e.g., `1`, `2`, `-3`.
*   **Floating-point numbers** (`float` or `double`): decimal numbers, e.g., `3.14`, `-0.5`.
*   **Characters** (`char`): single characters, e.g., `'a'`.
*   **Boolean** (`bool`): a value that can be either true or false.

### Type Modifiers
Type modifiers are used to specify the size of a variable:

*   `short`: 16-bit integer.
*   `long`: 32-bit or 64-bit integer, depending on the platform.
*   `unsigned`: positive integer only (no negative numbers).
*   `signed`: allows both positive and negative integers.

**Operators**
-------------
### Arithmetic Operators
Arithmetic operators perform mathematical operations:

*   `+` (addition)
*   `-` (subtraction)
*   `\*` (multiplication)
*   `/` (division)

### Comparison Operators
Comparison operators compare values:

-  ` == ` (equal to)
*   `!=` (not equal to)
*   `>` (greater than)
*   `<` (less than)

### Logical Operators

Logical operators evaluate conditions:

*   `&&` (and)
*   `\|\|` (or)
*   `!` (not)

**Control Structures**
----------------------

### Conditional Statements

Conditional statements execute code based on a condition:

*   **If statement**: executes code if the condition is true.
    ```c
    if (x > 10) {
        printf("x is greater than 10\n");
    }
    ```
*   **Switch statement**: selects which case to execute based on the value of an expression.
### Loops
Loops execute code repeatedly:

*   **For loop**: executes code while a condition is true.
    ```c
    for (int i = 0; i < 10; i++) {
        printf("%d\n", i);
    }
    ```
*   **While loop**: executes code while a condition is true.

**Functions**
--------------

### Function Declaration

A function declaration specifies the return type and name of a function, as well as any parameters it takes:

```c
int add(int x, int y) {
    return x + y;
}
```

### Function Call

To call a function, use its name followed by parentheses containing any required arguments:

```c
int result = add(2, 3);
printf("%d\n", result);  // prints 5
```

**Pointers**
------------

A pointer is a variable that stores the memory address of another variable.

### Pointer Declaration

To declare a pointer, use an asterisk (*) before the type:

```c
int *ptr;
```

### Initializing Pointers

Pointers can be initialized with a value using the assignment operator (=):

```c
int x = 10;
int *ptr = &x;  // points to the variable x
printf("%p\n", (void *) ptr);  // prints the memory address of x
```

**Arrays and Vectors**
----------------------

### Array Declaration

An array is a collection of values of the same type stored in contiguous memory locations.

```c
int arr[5];
```

### Accessing Array Elements

Array elements can be accessed using their index (position) within the array:

```c
int x = arr[0];  // accesses the first element of the array
printf("%d\n", x);
```

### Dynamic Memory Allocation

Arrays can also be created dynamically using the `malloc` function from the standard library:

```c
int *arr = malloc(5 * sizeof(int));
```

**Structures and Unions**
-------------------------

### Structures

A structure is a collection of variables of different types stored in contiguous memory locations.

```c
struct Person {
    int age;
    char name[20];
};
```

### Initializing Structures

Structures can be initialized with values:

```c
struct Person person = {30, "John"};
```

### Unions

A union is a collection of variables of different types that occupy the same memory location.

```c
union Color {
    int red;
    char name[20];
};
```

Here are some additional topics that could be added to the Markdown file:

**Pointers (continued)**
-----------------------

### Pointer Arithmetic

You can perform arithmetic operations on pointers to move between elements of an array.

```c
int arr[5];
int *ptr = arr;

printf("%d\n", *ptr);  // prints the first element of the array
ptr++;  // moves to the next element in the array
printf("%d\n", *ptr);  // prints the second element of the array
```

### Pointer Comparison

You can compare two pointers to check if they point to the same location.

```c
int x = 10;
int y = 20;

int *px = &x;
int *py = &y;

if (px == py) {
    printf("px and py point to the same location\n");
} else {
    printf("px and py do not point to the same location\n");
}
```

**Bitwise Operators**
-------------------

### Bitwise AND

The bitwise AND operator (&) performs a binary operation on two integers.

```c
int x = 5;  // binary representation: 101
int y = 3;  // binary representation: 011

int result = x & y;
printf("%d\n", result);  // prints 1 (binary representation: 001)
```

### Bitwise OR

The bitwise OR operator (|) performs a binary operation on two integers.

```c
int x = 5;  // binary representation: 101
int y = 3;  // binary representation: 011

int result = x | y;
printf("%d\n", result);  // prints 7 (binary representation: 111)
```

### Bitwise XOR

The bitwise XOR operator (^) performs a binary operation on two integers.

```c
int x = 5;  // binary representation: 101
int y = 3;  // binary representation: 011

int result = x ^ y;
printf("%d\n", result);  // prints 6 (binary representation: 110)
```

### Bitwise NOT

The bitwise NOT operator (~) performs a unary operation on an integer.

```c
int x = 5;  // binary representation: 101

int result = ~x;
printf("%d\n", result);  // prints -6 (binary representation: 11111010)
```

**Memory Management**
--------------------

### Dynamic Memory Allocation

You can dynamically allocate memory using the `malloc` function.

```c
int *ptr = malloc(sizeof(int));
*ptr = 10;
printf("%d\n", *ptr);  // prints 10
free(ptr);
```

### Automatic Memory Allocation

You can use automatic memory allocation with variables declared inside functions or loops.

```c
{
    int x;
    x = 10;
}

// the variable x is destroyed when it goes out of scope
```

**File Input/Output**
---------------------

### Reading from a File

You can read data from a file using the `fopen` function and reading functions like `fgets` or `fscanf`.

```c
FILE *fp = fopen("example.txt", "r");
if (fp == NULL) {
    printf("Unable to open file\n");
} else {
    char line[100];
    while (fgets(line, sizeof(line), fp) != NULL) {
        printf("%s", line);
    }
    fclose(fp);
}
```

### Writing to a File

You can write data to a file using the `fopen` function and writing functions like `fprintf`.

```c
FILE *fp = fopen("example.txt", "w");
if (fp == NULL) {
    printf("Unable to open file\n");
} else {
    fprintf(fp, "Hello, World!\n");
    fclose(fp);
}
```

**Error Handling**
------------------

### Checking for Errors

You can check if a function call was successful by checking the return value.

```c
FILE *fp = fopen("example.txt", "r");
if (fp == NULL) {
    printf("Unable to open file\n");
} else {
    // do something with the file pointer
}
```

### Using Error Codes

Some functions return error codes that indicate whether the operation was successful or not.

```c
int result = fscanf(fp, "%s", line);
if (result != 1) {
    printf("Error reading from file\n");
} else {
    // do something with the read data
}
```



































































### References