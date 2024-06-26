---
title: "Compilation Errors"
date: 2024-06-26
categories:
---

## Example 1

### Code 
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    string name;
    name = get_string("What's your name?\n")
    printf("Hello, %s\n", name);
}
```

### Error Generated 
hello2.c:7:45: error: expected ';' after expression


## Example 2

## Code 
```C
#include <cs50.h>
#include <stdio.h>

int main(void)
{
    string name;
    name = get_string("What's your name?\n");
    printf("Hello, %s\n, name);
}
```

## Error Generated 
error: missing terminating '"' character [-Werror,-Winvalid-pp-token]
    printf("Hello, %s\n, name);