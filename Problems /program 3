#include <stdio.h>
#include <string.h>

// Function to convert single digit number to word
char *ones(int num) {
    switch (num) {
        case 1: return "One";
        case 2: return "Two";
        case 3: return "Three";
        case 4: return "Four";
        case 5: return "Five";
        case 6: return "Six";
        case 7: return "Seven";
        case 8: return "Eight";
        case 9: return "Nine";
        default: return "";
    }
}

// Function to convert two-digit number to word
char *tens(int num) {
    switch (num) {
        case 10: return "Ten";
        case 11: return "Eleven";
        case 12: return "Twelve";
        case 13: return "Thirteen";
        case 14: return "Fourteen";
        case 15: return "Fifteen";
        case 16: return "Sixteen";
        case 17: return "Seventeen";
        case 18: return "Eighteen";
        case 19: return "Nineteen";
        case 20: return "Twenty";
        case 30: return "Thirty";
        case 40: return "Forty";
        case 50: return "Fifty";
        case 60: return "Sixty";
        case 70: return "Seventy";
        case 80: return "Eighty";
        case 90: return "Ninety";
        default: return "";
    }
}

// Function to convert three-digit number to word
void convertHundreds(int num) {
    if (num >= 100) {
        printf("%s Hundred ", ones(num / 100));
        num %= 100;
    }
    if (num >= 10 && num <= 19) {
        printf("%s ", tens(num));
        return;
    } else if (num >= 20) {
        printf("%s ", tens((num / 10) * 10));
        num %= 10;
    }
    if (num > 0) {
        printf("%s ", ones(num));
    }
}

// Function to convert the given number to words
void numberToWords(int num) {
    if (num == 0) {
        printf("Zero");
        return;
    }
    
    convertHundreds(num);
}

int main() {
    int number;
    printf("Enter a number between 0 and 99999: ");
    scanf("%d", &number);

    if (number < 0 || number > 99999) {
        printf("Input out of range.\n");
        return 1;
    }

    printf("Output: ");
    numberToWords(number);
    printf("\n");

    return 0;
}
