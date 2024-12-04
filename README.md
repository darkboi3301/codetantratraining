## INTRODUCTION TO C

> "I DID NOT Listen to anything before this cuz it was yap content imo" - Eeshwar
---

### Structure of C language

* document section
* ink section
* global declaration secftion
* main function
  ```c
  int main() {
      // sample  code
      return 0;
  }
  ```
* subprogram section
  ```c
  int function1(){
    return 0;
  }
  int function1(){
    return 0;
  }
  int function1(){
    return 0;
  }
  int function1(){
    return 0;
  }
  ```
---
> "More Yapping later... "

### Advantages of C
* Readability
* Modularity
* Maintainability
* Resuability
* Error Detection
* Reduced Complexity

> "Some More Yapping & Wrong Info Later..."

> "GOw Throughw Docs MAA" - code tantra

### Header Files in C

Header files in C contain declarations for functions and macros, which can be shared across multiple source files. They help in organizing code and promoting reusability by allowing the same declarations to be used in different parts of a program. Common header files include `stdio.h` for standard input and output functions and `stdlib.h` for general utility functions.

### Functions and macros 
Functions in C are blocks of code that perform a specific task. They help in breaking down a program into smaller, manageable pieces. Functions can be predefined (standard library functions) or user-defined. A function typically has a return type, a name, parameters (optional), and a body. For example:

```c
int add(int a, int b) {
	return a + b;
}
```

Macros in C are preprocessor directives that define constant values or expressions. They are defined using the `#define` directive and are replaced by their values before the compilation process. Macros can make code more readable and easier to maintain. For example:

```c
#define PI 3.14
#define SQUARE(x) ((x) * (x))
```

In the above example, `PI` is a macro for the constant value 3.14, and `SQUARE(x)` is a macro for calculating the square of a number.
### Difference Between Structured and Unstructured


| Feature           | Structured Programming      | Unstructured Programming |
| ----------------- | --------------------------- | ------------------------ |
| Code Organization | Well-organized              | Poorly organized         |
| Flow Control      | Uses loops and conditionals | Uses goto statements     |
| Readability       | High                        | Low                      |
| Maintainability   | Easier to maintain          | Harder to maintain       |
| Debugging         | Easier to debug             | Harder to debug          |
| Reusability       | High                        | Low                      |
| Error Detection   | Easier to detect errors     | Harder to detect errors  |


### Function Implementation

#### Sample Using a Function

Using a function to calculate the sum of two numbers:

```c
#include <stdio.h>

int add(int a, int b) {
  return a + b;
}

int main() {
  int num1 = 5, num2 = 10;
  int sum = add(num1, num2);
  printf("Sum: %d\n", sum);
  return 0;
}
```

#### Sample Without Using a Function

Calculating the sum of two numbers without using a function:

```c
#include <stdio.h>

int main() {
  int num1 = 5, num2 = 10;
  int sum = num1 + num2;
  printf("Sum: %d\n", sum);
  return 0;
}
```


### Hello World in C

A simple C program to print "Hello, World!" to the console:

```c
#include <stdio.h>

int main() {
  printf("Hello, World!\n");
  return 0;
}
```

This program includes the standard input-output header file `stdio.h` and defines the `main` function, which is the entry point of a C program. The `printf` function is used to print the message to the console.


### Hello World with Function

A simple C program to print "Hello, World!" using a function:

```c
#include <stdio.h>

void printHello() {
  printf("Hello, World!\n");
}

int main() {
  printHello();
  return 0;
}
```

In this program, the `printHello` function is defined to print the message "Hello, World!" to the console. The `main` function calls `printHello` to display the message.


> "ONE HOUR and MORE YAPPPING LATER..."

### Types of Variables in C

Variables in C are used to store data that can be manipulated by the program. There are several types of variables in C, each with its own characteristics and usage. The main types of variables are:

1. **Local Variables**:
  - Declared inside a function or block.
  - Accessible only within the function or block where they are declared.
  - Not initialized automatically; must be initialized explicitly.

  ```c
  void function() {
     int localVar = 10; // local variable
     printf("%d\n", localVar);
  }
  ```

2. **Global Variables**:
  - Declared outside of all functions.
  - Accessible from any function within the same file.
  - Initialized automatically to zero if not explicitly initialized.

  ```c
  int globalVar = 20; // global variable

  void function() {
     printf("%d\n", globalVar);
  }
  ```

3. **Static Variables**:
  - Can be local or global.
  - Retain their value between function calls.
  - Local static variables are accessible only within the function where they are declared.
  - Global static variables are accessible only within the file where they are declared.

  ```c
  void function() {
     static int staticVar = 0; // static local variable
     staticVar++;
     printf("%d\n", staticVar);
  }
  ```

  ### Data Types in C

  Data types in C define the type of data that a variable can hold. They determine the size and layout of the variable's memory, the range of values that can be stored, and the set of operations that can be performed on the variable. The primary data types in C are:

  1. **Basic Data Types**:
    - **int**: Used to store integers. Size is typically 4 bytes.
      ```c
      int num = 10;
      ```
    - **float**: Used to store floating-point numbers. Size is typically 4 bytes.
      ```c
      float num = 10.5;
      ```
    - **double**: Used to store double-precision floating-point numbers. Size is typically 8 bytes.
      ```c
      double num = 10.5;
      ```
    - **char**: Used to store single characters. Size is typically 1 byte.
      ```c
      char letter = 'A';
      ```

  2. **Derived Data Types**:
    - **Array**: A collection of elements of the same type.
      ```c
      int arr[5] = {1, 2, 3, 4, 5};
      ```
    - **Pointer**: A variable that stores the memory address of another variable.
      ```c
      int *ptr;
      int num = 10;
      ptr = &num;
      ```
    - **Structure**: A user-defined data type that groups related variables of different types.
      ```c
      struct Person {
       char name[50];
       int age;
      };
      ```

  3. **Enumeration**:
    - A user-defined data type that consists of integral constants.
      ```c
      enum week {Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday};
      ```

  4. **Void**:
    - Represents the absence of type. Commonly used for functions that do not return a value.
      ```c
      void function() {
       // code
      }
      ```

  Understanding these data types is crucial for effective programming in C, as they form the foundation for variable declaration and manipulation.

