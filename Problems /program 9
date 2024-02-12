#include <stdio.h>
#include <string.h>
#include <ctype.h>

void countVowels(char *str) {
    int vowels[5] = {0}; // Array to store counts of 'a', 'e', 'i', 'o', 'u'
    
    for (int i = 0; str[i] != '\0'; i++) {
        char ch = tolower(str[i]);
        switch (ch) {
            case 'a':
                vowels[0]++;
                break;
            case 'e':
                vowels[1]++;
                break;
            case 'i':
                vowels[2]++;
                break;
            case 'o':
                vowels[3]++;
                break;
            case 'u':
                vowels[4]++;
                break;
        }
    }

    printf("Output:\n");
    printf("a:%d\n", vowels[0]);
    printf("e:%d\n", vowels[1]);
    printf("i:%d\n", vowels[2]);
    printf("o:%d\n", vowels[3]);
    printf("u:%d\n", vowels[4]);
}

int main() {
    char str[] = "India";

    printf("Input: %s\n", str);

    countVowels(str);

    return 0;
}
