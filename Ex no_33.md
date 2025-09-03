# EX 33 C program to read a file name from user and create that file using fopen().
## DATE:03/09/2025
## AIM:
To write a C program to read a file name from user and create that file using fopen().

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

<img width="1629" height="680" alt="image" src="https://github.com/user-attachments/assets/ee0c3e49-f14e-4184-aa07-f5465df61ee5" />


## Result:
Thus the program was executed and the output was verified successfully.
