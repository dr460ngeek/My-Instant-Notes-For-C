# <b><i>IMPORTANT NOTES FOR C </i></b>
## Operators

### There are 5 types of operators in C language

+ Arithmetic Operators
+ Relational Operators
+ Logical Operators
+ Bitwise Operators
+ Assignment Operators

##### Arithmetic Operators

Operators such as :

- "+" Addition
- "-" Subtraction
- "*" Multiplication
- "/" Division
- "%" Modulus

Use cases:
```C
{
    int a = 10 ; // Addition
    float b = 20.25 ;

    printf("The sum of %d and %.f is: %d \n", a, b, a+b); // This will return the answer as it demands to return the sum of float and integer in float.
    
    int c ; // Subtraction
    float d ; 
    
    c = 10;
    d = 5.5;

    printf("The subtraction of %d from %.f is: %d \n", c, d, c-d); // This will return the answer as it demands to return the subtraction of float and integer in float.
    
    int e = 12 ; // Multiplication
    float f = 2.5 ;

    printf("The multiplication of %d and %.2f is: %d \n", e, f, e*f); // This will return the answer as it demands to return the multiplication of float and integer in float.
    
    int g = 10 ; // division
    float h = 2.5 ; 

    printf("The division of %d by %.f is: %.2f \n", g, h, g/h ); // This will return the answer as it demands to return the division of float and integer in float.
    
    int i = 10 ; // Modulus
    /* float j = 2 ;
    printf("The modulus of %d by %f is: %.2f \n", i, j, i % j ); This incorrect because in modulus, you cannot calculate using floats. */
    int j = 6 ;
    printf("The modulus of %d by %d is: %d", i, j, i%j ); // This will return answer as it demands both operands and answers to be an integer.
    
    return 0;
}

```

The points to consider: 
+ The operation between float and integer will always return a float as an answer.
+ The operation between integer and integer will always return a integer as an answer.
+ The operation between float and float will always return a float as an answer.


##### Relational Operators

Operators such as :
- ">" Greater than
- "<" Lesser than
- "==" Is equal to
- "!=" Is not equal to
- ">" Greater than
- "<" Less than
- ">=" Greater than or equal to
- "<=" Less than or equal to

Use cases:
```C
#include <stdio.h>

int main()

{
    // == is equal to
    int a = 2;
    int b = 2;

    printf("'==' example: a == b = %d\n \a", a == b);
    // if a and b are equal to each other then it will print 1. 1 is true while 0 is false.

    printf("'!=' example: a != b = %d\n \a", a != b);
    // if a and b are not equal to each other then it will print 0. 1 is true while 0 is false.

    printf("'>=' example: a >= b = %d\n \a", a >= b);
    // if a is greater than or equals to b then it will print 1. 1 is true while 0 is false.

    printf("'<=' example: a <= b = %d\n \a", a <= b);
    // if a is lesser than or equals to b then it will print 1. 1 is true while 0 is false.

    printf("'>' example: a > b = %d\n \a", a > b);
    // if a is greater than b then it will print 0. 1 is true while 0 is false.

    printf("'<' example: a < b = %d\n \a", a < b);
    // if a is lesser than b then it will print 0. 1 is true while 0 is false.



    return 0;
} 
```
##### Logical & Bitwise Operators

###### Logical 

Operators such as :

- "&&" Both the operands are suppose to be true. Dono!
- "||" One of the operands must be true. Dono me se koi ek!
- "!" If it is true, it prints false. Theek ulta.

Use cases:
```C
#include <stdio.h>

void main()
{
    // Logical operators.
    int a, b;
    printf("Enter the values for a & b respectfully: \n");
    scanf("%d%d", &a, &b);
    
    printf("'&&': (%d && %d) = %d \n", a, b, a && b); 
    // Both of them needs to be true.
    printf("'||': (%d || %d) = %d \n", a, b, a || b); 
    // Anyone of them needs to be true.
    printf("'!': !(%d && %d) = %d \n", a, b, !(a&&b)); 
    // Here, we were suppose to get false but we got true. This is what '!' does as shown in the syntax.
}
```
###### Bitwise

It converts the integeral operands into binary and checks if it's true or not.

- "&" AND. 
-  "|" OR.
- "^" XOR or Exclusive OR.
- "~" is the binary one's complement operators. ___Not so important as of now___
- "<<" is the binary left shift operators. ___Not so important as of now___
- ">>" is the binary right shift operators. ___Not so important as of now___
```C
#include <stdio.h>
void main()
{
    // Bitwise operator. 
    int c, d;
    printf("Enter the value of 'c': \n");
    scanf("%d", &c);
    printf("Enter the value of 'd': \n");
    scanf("%d", &d);
    // It converts the integeral operands into binary and checks if it's true or not.


    printf("'&': %d & %d = %d \n", c, d, c==d & c<d); 
    printf("'|': %d | %d = %d \n", c, d, c==d | c==d); 
    printf("'^': %d ^ %d = %d \n", c, d, c==d ^ c==d); 
    
/*--------------------------------------------------------------------------------------------------------------*/
}
```
### Operators Precedence 

|Category      |Operators                         |Associativity |
|--------------|----------------------------------|--------------|
|Postfix       |() [] -> . ++ - -                 |Left to right |
|Unary         |+ - ! ~ ++ - - (type)* & sizeof   |Right to left |
|Multiplicative|* / %                             |Left to right |
|Additive	   |+ -	                              |Left to right |
|Shift         |<< >>	                          |Left to right |
|Relational	   |< <= > >=	                      |Left to right |
|Equality	   |== !=                             |Left to right |
|Bitwise AND   |&                                 |Left to right |
|Bitwise XOR   |^	                              |Left to right |
|Bitwise OR	   | "|"	                          |Left to right |
|Logical AND   |&&	                              |Left to right |
|Logical OR	   | "||"	                          |Left to right |
|Conditional   | ?:	                              |Right to left |
|Assignment	   | = += -= *= /= %=>>= <<= &= ^= |= |Right to left |
|Comma	       |,	                              |Left to right |


## Format Specifiers & Escape Sequences

### Format Specifier & Constants

#### Format specifier

|S no.|Specifiers     | Type      |
|-----|---------------|-----------|
|1.   |%d             |Integer    |
|2.   |%f             |Float      |
|3.   |%c             |Character  |
|4.   |%l             |Long       |
|5.   |%lf            |Double     |
|6.   |%Lf            |Long Double|

>Float (%f) is an interesting one:

```C


{
    int a = 1.3333 ;
    printf("%f",a);
    printf("%.2f", a) // Prints only two decimal points(.).
    printf("%10.f |",a); /* Prints the float according to accuracy of the number given after %.
    Since the number is in (+), it will leave excessive spaces before the float number while printing*/
    printf("%-10.f |",a); /* Prints the float according to accuracy of the number given after %.
    Since the number is in (-), it will leave excessive spaces after the float number while printing*/
}

```

#### Constants

Points to be noted!
+ Constants are immutable.
+ Constants can be pre-processed as well with "#define".

```C
#include <stdio.h>
void main()
{
    const float a = 4.33 ;
    a = 2.22 ; 
    printf("%f", a); /* Will show an error because  a's value has
    become immutable as we assigned it as constant before. */
}
```
Pre-processed Constants:
```C
#include <stdio.h>
#define PI 3.14

{
    printf("%f", PI);
}
```

### Escape Sequences

|Escape Sequence              |Description                        |
|-----------------------------|-----------------------------------|
|\t                           |Inserts a tab                      |
|\b                           |Inserts a backspace                |
|\n                           |Inserts a newline.                 |
|\r                           |Inserts a carriage return.         |
|\f                           |Inserts a form feed.               |
|\’                           |Inserts a single quote character.  |
|\”                           |Inserts a double quote character.  |
|\\\                          |Inserts a backslash character.     |
