# Loops

There are 3 types of loops:

+ do-while loop
+ while loop
+ forloop

### do-while loop:

* It is executed atleast once regardless of the conditions.
* It first executes and then checks the condition.

Syntax:
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