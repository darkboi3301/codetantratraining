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



