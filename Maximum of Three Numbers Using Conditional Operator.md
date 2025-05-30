# # Maximum of Three Numbers Using Conditional Operator

This repository contains a **C program** that determines the **maximum of three integer values** using the **conditional (ternary) operator**.

## 🎯 Aim

To write a C program that finds the maximum between three integers using the **conditional (ternary) operator**.

## 📋 Algorithm

1. Declare integer variables: `a`, `b`, `c`, and `max`.
2. Prompt the user to enter three integer values (`a`, `b`, `c`).
3. Use nested ternary operators to calculate the maximum:
   ```c
   max = (a > b) ? (a > c ? a : c) : (b > c ? b : c);
4. Display the maximum value.

## Program
```
#include <stdio.h>

int main() {
    int a, b, c, max;

    printf("Enter three integers: ");
    scanf("%d %d %d", &a, &b, &c);

    max = (a > b) ? ((a > c) ? a : c) : ((b > c) ? b : c);

    printf("Maximum value is: %d\n", max);

    return 0;
}
```

## Output
Sample Output 1:
Enter three integers: 10 20 15
Maximum value is: 20

Sample Output 2:
Enter three integers: 25 15 30
Maximum value is: 30

## Result
Program was implemented and executed.
