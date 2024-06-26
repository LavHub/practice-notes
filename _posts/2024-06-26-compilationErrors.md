---
title: "Compilation Errors"
date: 2024-06-26
categories:
---

### Code (Example: 1)
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

### Error Generated (Example: 1)
hello2.c:7:45: error: expected ';' after expression

## Code (Example: 2)
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

## Error Generated (Example: 2)
error: missing terminating '"' character [-Werror,-Winvalid-pp-token]
    printf("Hello, %s\n, name);