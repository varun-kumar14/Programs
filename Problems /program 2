#include <stdio.h>
#include <string.h>

void compressString(char *input) {
    int len = strlen(input);
    if (len == 0)
        return;

    int count = 1;
    for (int i = 0; i < len; i++) {
        if (input[i] == input[i + 1]) {
            count++;
        } else {
            printf("%c%d", input[i], count);
            count = 1;
        }
    }
}

int main() {
    char input[100];
    printf("Enter input string: ");
    scanf("%s", input);

    printf("Compressed string: ");
    compressString(input);
    printf("\n");

    return 0;
}
