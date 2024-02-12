#include <stdio.h>
#include <string.h>

void justifyText(char *text, int length) {
    int words = 1;
    int spaces_needed = length - strlen(text);
    for (int i = 0; text[i] != '\0'; i++) {
        if (text[i] == '_') {
            words++;
        }
    }
    int spaces_per_word = spaces_needed / (words - 1);
    int extra_spaces = spaces_needed % (words - 1);

    printf("Output: ");
    int i = 0;
    while (text[i] != '\0') {
        if (text[i] == '_') {
            printf(" ");
            for (int j = 0; j < spaces_per_word; j++) {
                printf(" ");
            }
            if (extra_spaces > 0) {
                printf(" ");
                extra_spaces--;
            }
        } else {
            printf("%c", text[i]);
        }
        i++;
    }
    printf("\n");
}

int main() {
    char text[] = "Zoho_Corp_Madurai";
    int length = 25;

    printf("Input:\n");
    printf("Text = %s\n", text);
    printf("Padding = %d\n", length);
    
    justifyText(text, length);

    return 0;
}
