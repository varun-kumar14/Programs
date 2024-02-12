#include <stdio.h>
#include <string.h>

// Function to swap characters at position i and j in the string
void swap(char *x, char *y) {
    char temp = *x;
    *x = *y;
    *y = temp;
}

// Function to generate permutations of the string
void permute(char *str, int start, int end) {
    if (start == end) {
        printf("%s\n", str);
    } else {
        for (int i = start; i <= end; i++) {
            // Swap characters at positions start and i
            swap((str + start), (str + i));
            // Recursively generate permutations for the remaining characters
            permute(str, start + 1, end);
            // Undo the swap to backtrack
            swap((str + start), (str + i));
        }
    }
}

int main() {
    char str[] = "Good";
    int n = strlen(str);
    
    printf("Input: %s\n", str);
    printf("Output:\n");
    permute(str, 0, n - 1);

    return 0;
}
