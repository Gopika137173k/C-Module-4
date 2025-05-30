# 🔠 Strings: String Comparison in C

## 🎯 Aim
To write a C program that compares two strings character by character and checks whether they are the same.

## 🧠 Algorithm

1. **Start** the program.
2. **Declare** two character arrays `c1` and `c2` of size 100 to store the strings.
   - Also, declare:
     - An integer `i` for indexing.
     - An integer `flag` initialized to `0` to indicate whether strings are different.
3. **Read** the first string `c1` using:
   ```c
   scanf("%[^\n]", c1);
   This reads the entire line including spaces until newline.

4 Read the second string c2 using:
  scanf("%s", c2);
  This reads until the first whitespace character.

5. Compare characters at each index of c1 and c2:

6. Use a loop to check if characters at each position are equal.

7. If c1[i] != c2[i], set flag = 1.

8. After comparison:

If flag == 0, print Strings are same.

9. Else, print Strings are not same.

10. End the program.

## Program
```
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int i = 0, flag = 0;

    printf("Enter the first string: ");
    scanf("%[^\n]", c1);  // Read entire line including spaces until newline

    getchar(); // To consume the leftover newline character

    printf("Enter the second string: ");
    scanf("%s", c2);      // Read until first whitespace

    while (c1[i] != '\0' && c2[i] != '\0') {
        if (c1[i] != c2[i]) {
            flag = 1;
            break;
        }
        i++;
    }

    // If lengths are different, strings are not same
    if (c1[i] != '\0' || c2[i] != '\0') {
        flag = 1;
    }

    if (flag == 0) {
        printf("Strings are same.\n");
    } else {
        printf("Strings are different.\n");
    }

    return 0;
}
```
## Output
Sample Output 1:
Enter the first string: hello world
Enter the second string: hello
Strings are different.

Sample Output 2:
Enter the first string: example
Enter the second string: example
Strings are same.

## Result
Program was implemented and executed.
