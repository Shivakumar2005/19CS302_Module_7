# EX 32 C program to display Hardware details such as price, product name and price using structure.
## DATE:
## AIM:
To write a C program to display Hardware details such as price, product name and price using structure.

## Algorithm
1. Start the program.
2. Define a structure with members for product name and price.
3. Declare a structure variable.
4. Read the hardware details from the user.
5. Display the entered hardware details. 

## Program:
#include <stdio.h>

struct Hardware {
    char name[50];
    float price;
};

int main() {
    struct Hardware h;
    printf("Enter product name: ");
    scanf("%s", h.name);
    printf("Enter price: ");
    scanf("%f", &h.price);

    printf("\nHardware Details:\n");
    printf("Product Name: %s\n", h.name);
    printf("Price: %.2f\n", h.price);

    return 0;
}


## Output:

<img width="1390" height="677" alt="image" src="https://github.com/user-attachments/assets/c8cb5a0e-5739-4ebd-a6a5-2cc09f57216c" />


## Result:
Thus the program was executed and the output was verified successfully.
