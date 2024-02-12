#include <stdio.h>
#include <string.h>

void findMismatchedSubstrings(char *str1, char *str2) {
    int len1 = strlen(str1);
    int len2 = strlen(str2);
    int i = 0, j = 0;

    while (i < len1 && j < len2) {
        if (str1[i] != str2[j]) {
            int start1 = i;
            int start2 = j;

            // Find the end of mismatched substring in str1
            while (i < len1 && str1[i] != str2[j]) {
                i++;
            }

            // Find the end of mismatched substring in str2
            while (j < len2 && str2[j] != str1[start1]) {
                j++;
            }

            // Print the mismatched substring
            printf("%.*s, %.*s\n", i - start1, str1 + start1, j - start2, str2 + start2);
        } else {
            i++;
            j++;
        }
    }
}

int main() {
    char str1[] = "AABBCCDD";
    char str2[] = "ABCDCCAD";

    printf("Input:\n");
    printf("%s, %s\n", str1, str2);

    printf("Output:\n");
    findMismatchedSubstrings(str1, str2);

    return 0;
}
