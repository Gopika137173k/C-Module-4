# Strings: Word Counter in a String (Using Function in C)

## 🎯 Aim
To write a C program that counts the total number of words in a given string using a function.

## 🧠 Algorithm

1. **Declare** a character array `a` of size 100, and variables `i` and `count`, initialized to `0` and `1` respectively.
2. **Read** a string (including spaces) until a newline character is encountered and store it in array `a`.
3. **Use** a `do-while` loop to iterate through each character of the string:
   - **Increment** `count` every time a space `' '`, newline `'\n'`, or tab `'\t'` character is encountered.
4. **Print** the final value of `count`, which represents the total number of words in the string.

## Program
```
#include <stdio.h>

void countWords(char a[]) {
    int i = 0, count = 1;

    do {
        if (a[i] == ' ' || a[i] == '\n' || a[i] == '\t') {
            count++;
        }
        i++;
    } while (a[i] != '\0');

    printf("Total number of words: %d\n", count);
}

int main() {
    char a[100];

    printf("Enter a string: ");
    fgets(a, sizeof(a), stdin);  // Read string including spaces

    countWords(a);

    return 0;
}
```

## Output
Sample Output 1:
Enter a string: Hello world this is C
Total number of words: 5

Sample Output 2:
Enter a string: Counting   words	in this string
Total number of words: 5

## Result
Program was implemented and executed.
