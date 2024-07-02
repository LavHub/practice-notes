---
title: "Number Programs"
date: 2024-07-01
categories:
---
### These are coding practice problems involving inputs, outputs, while loops, and if else statements

## Positive or Negative
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int num;
    printf("This code will print whether your input is positive or negative\n");
    num = get_int("Enter a number: ");
    if (num < 0){
        printf("This number is negative\n");
    }else{
        printf("This number is positive\n");
    }
}
```

## Maximum Number
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int num1;
    int num2;
    printf("This code will find the max of two numbers\n");
    num1 = get_int("Enter first number: ");
    num2 = get_int("Enter second number: ");
    if (num1 > num2){
        printf("%d is greater than %d.\n", num1, num2);
    }else{
        printf("%d is greater than %d.\n", num2, num1);
    }
}
```

## Even or Odd
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int num;
    printf("This code will display if your number input is even or odd\n");
    num = get_int("Enter a number:");
    if ((num % 2) == 0){
        printf("The number %d is even\n", num);
    }else{
        printf("The number %d is odd\n", num);
    }
}
```

## Print Even
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int num;
    int evenNum;
    printf("This code prints N number of even numbers\n");
    num = get_int("Enter number: ");
    evenNum = 2;
    while ( num > 0){
        printf("%d\n", evenNum);
        num = num - 1;
        evenNum = evenNum + 2;
    }
}
```