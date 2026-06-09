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
int countWords(char str[]) {
    int i = 0, count = 0;
    while (str[i] == ' ' || str[i] == '\t' || str[i] == '\n') {
        i++;
    }
    if (str[i] == '\0') 
        return 0;
    count = 1; 
    do {
        if (str[i] == ' ' || str[i] == '\t' || str[i] == '\n') {
            while (str[i] == ' ' || str[i] == '\t' || str[i] == '\n') {
                i++;
            }
            if (str[i] != '\0') {
                count++;
            } else {
                break;
            }
        } else {
            i++;
        }
    } while (str[i] != '\0');
    return count;
}

int main() {
    char a[100];
    printf("Enter a string: ");
    fgets(a, sizeof(a), stdin);  
    int words = countWords(a);
    printf("Total number of words: %d\n", words);
    return 0;
}
```

## Output
<img width="910" height="303" alt="image" src="https://github.com/user-attachments/assets/09625532-3b5f-41de-9527-dd74d591e643" />

## Result
C program to counts the total number of words in a given string using a function is written.
