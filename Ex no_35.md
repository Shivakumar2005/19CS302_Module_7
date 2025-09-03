# EX 35 C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
## DATE:03/09/2025
## AIM:
To write a C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.

## Algorithm
1. Start the program.
2. Open the file "Hospital.txt" in write mode.
3. Check whether the file is created successfully.
4. If successful, display a message for creation and opening.
5. Close the file and display a message for closing.  

## Program:
#include <stdio.h>

int main() {
    FILE *fp;
    fp = fopen("Hospital.txt", "w");

    if(fp == NULL) {
        printf("Error creating file!\n");
        return 1;
    }

    printf("File 'Hospital.txt' created and opened successfully.\n");

    fclose(fp);
    printf("File closed successfully.\n");

    return 0;
}

## Output:

<img width="1718" height="705" alt="image" src="https://github.com/user-attachments/assets/32434b61-45db-4a0b-ad9a-ffbd986282ba" />


## Result:
Thus the program was executed and the output was verified successfully.
