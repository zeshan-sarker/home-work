# home-work
home work for today
#include <stdio.h>

int main() {
    double num1, num2, result;
    char op;

    //inputs from user
    printf("Enter first number: ");
    scanf("%lf", &num1);

    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &op);

    printf("Enter second number: ");
    scanf("%lf", &num2);

    // calculation part
    if (op == '+') {
        result = num1 + num2;
        printf("Result: %.2lf\n", result);
    }
    else if (op == '-') {
        result = num1 - num2;
        printf("Result: %.2lf\n", result);
    }
    else if (op == '*') {
        result = num1 * num2;
        printf("Result: %.2lf\n", result);
    }
    else if (op == '/') {
        if (num2 != 0) {
            result = num1 / num2;
            printf("Result: %.2lf\n", result);
        } else {
            printf("Error: Division by zero!\n");
        }
    }
    else {
        printf("Invalid operator.\n");
    }

    return 0;
}
#include <stdio.h>

int main() {
    double num1, num2, result;
    char op;

    printf("Enter first number: ");
    scanf("%lf", &num1);

    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &op);

    printf("Enter second number: ");
    scanf("%lf", &num2);

    switch(op) {
        case '+':
            result = num1 + num2;
            printf("Result: %.2lf\n", result);
            break;
        case '-':
            result = num1 - num2;
            printf("Result: %.2lf\n", result);
            break;
        case '*':
            result = num1 * num2;
            printf("Result: %.2lf\n", result);
            break;
        case '/':
            if(num2 != 0) {
                result = num1 / num2;
                printf("Result: %.2lf\n", result);
            } else {
                printf("Error: Division by zero!\n");
            }
            break;
        default:
            printf("Invalid operator.\n");
            break;
    }

    return 0;
}
