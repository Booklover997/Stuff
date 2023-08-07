#c 

```c
#include <stdio.h>

void doStuff(int * stuff) {
    *stuff = 1337;
    printf("Within the doStuff() function, the variable stuff has the value: %d\n\n", *stuff);
}

int main() {
    int stuff = 42;
    printf("Within the main function, before doStuff is called, the variable stuff has the value: %d\n\n", stuff);
    doStuff(&stuff);
    printf("Within the main function, after doStuff is called, the variable stuff has the value %d\n\n", stuff);
    return(0);
}
```
This tells the code to change the number at the address of stuff on the [[stack]] instead of creating a new variable in memory which would have a value of 1337 