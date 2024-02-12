#include <stdio.h>
#include <string.h>

// Function to check if a number is palindrome
int isPalindrome(int num) {
    int reverse = 0;
    int temp = num;

    while (temp != 0) {
        reverse = reverse * 10 + temp % 10;
        temp /= 10;
    }

    return reverse == num;
}

// Function to find the next palindrome number
int nextPalindrome(int num) {
    do {
        num++;
    } while (!isPalindrome(num));

    return num;
}

int main() {
    int number;

    // Input
    printf("Input: ");
    scanf("%d", &number);

    // Output
    printf("Output: %d\n", nextPalindrome(number));

    return 0;
}
