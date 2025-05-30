# Strings: Check If Character Is an Alphabet Using ASCII and If-Else in C

This repository contains a simple **C program** that checks whether the entered character is an **alphabet or not**, using **ASCII values** and an `if-else` statement.

## 🎯 Aim

To write a C program that checks if an input character is an **alphabet** (either uppercase or lowercase) using **ASCII values** and `if-else` statements.

## 📋 Algorithm

1. Declare a variable `ch` of type `char`.
2. Read a character from the user.
3. Use an `if-else` condition to check:
   - If `ch` is between `'A'` and `'Z'` (ASCII 65–90), or
   - If `ch` is between `'a'` and `'z'` (ASCII 97–122).
4. If the condition is true, print `"Alphabet"`.
5. Otherwise, print `"Not an Alphabet"`.

##Program
```
#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    if ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) {
        printf("Alphabet\n");
    } else {
        printf("Not an Alphabet\n");
    }

    return 0;
}
```
## 🧾 Sample Output

Sample Output 1:
Enter a character: G
Alphabet

Sample Output 2:
Enter a character: 5
Not an Alphabet

##Result
Program was implemented and executed.
