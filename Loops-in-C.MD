# Loops
Does that sound like poop? to me it does but I respect it way more than I respect poops.

There are 3 types of loops:

+ do-while loop
+ while loop
+ for loop

### do-while loop:

* It's an Exit controlled loop.
* It first executes and then checks the condition.
* It is executed atleast once regardless of the conditions.

Syntax:
```C
do {
    // code to be executed
} while(/*condition*/);
```
Use case:
```C
#include <stdio.h>

int main()
{
    int num, index = 0;
    printf("Enter a number\n");
    scanf("%d", &num);
    do
    {
        printf("%d\n", index + 1);
        index = index + 1;
    } while (index < num);

    return 0;
}

```

### while loop:

* It's an Entry Controlled loop.
* Unlike do-while loop, It checks condition and then executes loops.
* There is no semicolon in the syntax of while loop unlike do-while loop.

Syntax:
```C
while(/*conditon*/) {
// code to be executed.
}
```
Use Case:
```C
while(i<=30) {
    printf("%d", i++);
}
```

### for loop:

* It's an Entry Controlled loop.
* Similar to while loop. For-loop has the ability to assign the value for it's iteration and increment/decrement the value of it. 

Syntax:
```C
for( /* initialization */ ; /* check/test expression */ ; /* updation */)
{    
     // body consisting of multiple statements
}
```
Use Case:
```C
for (int i = 1; i <= 10; i++){
    printf("It should print this text 10 times. \n ");
}
```