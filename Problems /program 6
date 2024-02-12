#include <stdio.h>
#include <string.h>
#include <ctype.h>

int isSpecialChar(char ch) {
    return !(isalpha(ch) || isdigit(ch));
}

int isPalindrome(char *str) {
    int left = 0;
    int right = strlen(str) - 1;

    while (left < right) {
        if (isSpecialChar(str[left])) {
            left++;
            continue;
        }
        if (isSpecialChar(str[right])) {
            right--;
            continue;
        }

        if (tolower(str[left]) != tolower(str[right])) {
            return 0;
        }
        left++;
        right--;
    }
    return 1;
}

int main() {
    char str1[] = "malayalam";
    char str2[] = "m@ala $ $ y* a &lam (malayalam)";
    char str3[] = "Something";

    printf("Input: %s\n", str1);
    printf("Output: %s\n", isPalindrome(str1) ? "True" : "False");

    printf("Input: %s\n", str2);
    printf("Output: %s\n", isPalindrome(str2) ? "True" : "False");

    printf("Input: %s\n", str3);
    printf("Output: %s\n", isPalindrome(str3) ? "True" : "False");

    return 0;
}
