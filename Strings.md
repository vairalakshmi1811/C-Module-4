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

## Program
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
<img width="914" height="265" alt="image" src="https://github.com/user-attachments/assets/e606e44a-02b3-4221-b937-8e2b25fda6b4" />

## Result
C program that checks if an input character is an **alphabet** (either uppercase or lowercase) using **ASCII values** and if-else statements is written.
