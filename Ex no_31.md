# EX 31 C program to find the smallest among three numbers using Structure.
## DATE:03/09/2025
## AIM:
To write a C program to find the smallest among three numbers using Structure.

## Algorithm
1. Start the program.
2. Define a structure to store three numbers.
3. Read three numbers from the user and store them in the structure.
4. Compare the three numbers using conditional statements. 
5. Display the smallest number.  

## Program:
#include <stdio.h>

struct Numbers {
    int a, b, c;
};

int main() {
    struct Numbers n;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &n.a, &n.b, &n.c);

    if(n.a <= n.b && n.a <= n.c)
        printf("Smallest number is: %d\n", n.a);
    else if(n.b <= n.a && n.b <= n.c)
        printf("Smallest number is: %d\n", n.b);
    else
        printf("Smallest number is: %d\n", n.c);

    return 0;
}


## Output:

<img width="1460" height="671" alt="image" src="https://github.com/user-attachments/assets/9d7b3791-3a60-43a5-adbf-899c51070957" />


## Result:
Thus the program was executed and the output was verified successfully.
