Does not allow for [[Object Oriented Programming]]
C must be compiled used a [[Compiler]] rather than other languages like [[Python]] which allow for interpreters

C is used to make other higher level programming languages such as [[Python]]

C starts in the main function

1. To run c code you must first compile it using [[gcc]]
```
   gcc -o hello hello.c
```

___
Here is some example c code
```c
#include <stdio.h>

int main() {
    puts("Hello Foundations World");
    return(0);
}
```
return 0 indicates the success of the program

# Variables
```c
char variable_1[] = "Hello my first variable";
```
This defines a char array and allows you to store a string

# Printing
[[Puts]] is used for basic printing while [[printf]] is used for more advanced printing

____

# INTS
ints can be [[signed]] or [[unsigned]] 
```c
int value = 10;
value++;
value--;
puts(value)
```
> #### value++ increments and value-- decrements

____

# Comments

```c
//This is a comment
/*This is also a comment
But is a multiline comment
See lots of lines*/

```

---

# Arrays
```c
    char array[] = {'H', 'e', 'l', 'l', 'o', ' ', 'W', 'o', 'r', 'l', 'd'};
```
We use arrays to hold strings
##### Data **CANNOT** be added to an array a new array must be created

# Getting Input
```c
    fgets(data, sizeof data, stdin);
```

###### Argc:
contains the number of [[argument]]s passed into the command when it is run

###### Argv:
contains an array with each of the [[argument]]s passed in when it is run

# Reading From Files
Reading from files is the same as reading from the command line input as stdin is treated as input

# [[Pointers]]
[[Pointers]] allow you change memory on the [[Stack]] 

# [[Malloc]]
[[Malloc]] allows you to change memory on the [[Heap]]






