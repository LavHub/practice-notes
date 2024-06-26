---
title: "Compilation Errors"
date: 2024-06-26
categories:
---

## Code
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

## Error Generated

hello2.c:7:45: error: expected ';' after expression
    name = get_string("What's your name?\n")
                                            ^
                                            ;
1 error generated.
make: *** [<builtin>: hello2] Error 1

