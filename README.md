#include <stdio.h>

int main() {
    int ch;
    float a, b;

    printf("1.Add 2.Sub 3.Mul 4.Div \nEnter choice:");
    scanf("%d", &ch);
    printf("Enter two numbers:");
    scanf("%f %f", &a, &b);

    switch (ch) {
        case 1: printf("Sum=%.2f", a + b); break;
        case 2: printf("Diff=%.2f", a - b); break;
        case 3: printf("Product=%.2f", a * b); break;
        case 4: printf("Quotient=%.2f", b != 0 ? a / b : 0); break;
        default: printf("Invalid choice");
    }

    return 0;
}
