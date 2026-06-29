# Day 1


## Q1. Calculate sum of first N natural numbers

> **Logic:** *Loop from 1 to N, adding each value. Alternatively: sum = n(n+1)/2.*

**C Code:**
```c
#include <stdio.h>

int main() {

    int n, sum = 0;

    printf("Enter N: ");

    scanf("%d", &n);

    for (int i = 1; i <= n; i++)

        sum += i;

    printf("Sum = %d\n", sum);

    return 0;

}
```


## Q2. Print multiplication table of a given number

> **Logic:** *Loop from 1 to 10 and print ni each iteration.*

**C Code:**
```c
#include <stdio.h>

int main() {

    int n;

    printf("Enter number: ");

    scanf("%d", &n);

    for (int i = 1; i <= 10; i++)

        printf("%d x %d = %d\n", n, i, n * i);

    return 0;

}
```


## Q3. Find factorial of a number

> **Logic:** *Multiply from 2 to n. Use long long for large values.*

**C Code:**
```c
#include <stdio.h>

int main() {

    int n;

    long long fact = 1;

    printf("Enter n: ");

    scanf("%d", &n);

    for (int i = 2; i <= n; i++)

        fact *= i;

    printf("Factorial = %lld\n", fact);

    return 0;

}
```


## Q4. Count digits in a number

> **Logic:** *Divide by 10 repeatedly and count iterations until n becomes 0.*

**C Code:**
```c
#include <stdio.h>

int main() {

    int n, count = 0;

    printf("Enter number: ");

    scanf("%d", &n);

    if (n == 0) { printf("Digits = 1\n"); return 0; }

    if (n < 0) n = -n;

    while (n > 0) { n /= 10; count++; }

    printf("Digits = %d\n", count);

    return 0;

}
```
