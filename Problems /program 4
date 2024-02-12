#include <stdio.h>
#include <string.h>

void compare(const char *str1, const char *str2) {
    int len1 = strlen(str1);
    int len2 = strlen(str2);

    if (len1 != len2) {
        printf("Strings are not of equal length.\n");
        return;
    }

    printf("Output:\n");
    for (int i = 0; i < len1; i++) {
        if (str1[i] != str2[i]) {
            printf("%c, %c\n", str1[i], str2[i]);
        }
    }
}

int main() {
    const char *str1 = "antonyandcleopatra";
    const char *str2 = "antaniandcleapadra";

    printf("Input:\n");
    printf("str1 = \"%s\"\n", str1);
    printf("str2 = \"%s\"\n", str2);

    compare(str1, str2);

    return 0;
}
