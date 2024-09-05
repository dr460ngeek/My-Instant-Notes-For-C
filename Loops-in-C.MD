# Loops
Does that sound like poop? to me it does but I respect it way more than I respect poops.

There are 3 types of loops:

+ do-while loop
+ while loop
+ for loop

### do-while loop:

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