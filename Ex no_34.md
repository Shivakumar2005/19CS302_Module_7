# EX 34 C program to read a file name from user and create that file and insert student roll numbers in to that file.
## DATE:03/09/2025
## AIM:
To write a C program to read a file name from user and create that file and insert student roll numbers in to that file.

## Algorithm
1. Start the program.
2. Read the file name from the user.
3. Open the file in write mode.
4. Read roll numbers from the user and write them into the file. 
5. Close the file and display a success message.  

## Program:
#include <stdio.h>

int main() {
    FILE *fp;
    char filename[50];
    int n, roll;

    printf("Enter file name: ");
    scanf("%s", filename);

    fp = fopen(filename, "w");
    if(fp == NULL) {
        printf("Error creating file!\n");
        return 1;
    }

    printf("Enter number of students: ");
    scanf("%d", &n);

    for(int i = 0; i < n; i++) {
        printf("Enter roll number %d: ", i + 1);
        scanf("%d", &roll);
        fprintf(fp, "%d\n", roll);
    }

    fclose(fp);
    printf("Data written successfully to %s\n", filename);

    return 0;
}


## Output:

<img width="1374" height="634" alt="image" src="https://github.com/user-attachments/assets/458e5e9b-b462-491e-bc7f-9e994258cf30" />


## Result:
Thus the program was executed and the output was verified successfully.
