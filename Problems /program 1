#include <stdio.h>
#include <ctype.h>

void printRepeatedChars(char ch, int count) {
    for (int i = 0; i < count; ++i) {
        printf("%c", ch);
    }
}

int main() {
    char input[100];
    printf("Enter input string: ");
    scanf("%s", input);

    int i = 0;
    while (input[i] != '\0') {
        char ch = input[i++];
        int count = 0;
        while (isdigit(input[i])) {
            count = count * 10 + (input[i] - '0');
            i++;
        }
        if (count == 0) {
            count = 1; // If no digit follows, set count to 1
        }
        printRepeatedChars(ch, count);
    }
    printf("\n");

    return 0;
}
