# EX-21-POINTERS
## AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    double value = 23.65;
    double *ptr = &value;

    *ptr = 25.0;

    printf("Modified value: %.2f\n", value);

    return 0;
}
```
## OUTPUT:	

![image](https://github.com/user-attachments/assets/2afa549d-420e-4ac8-967f-82ed662707b3)










## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 
<hr>

# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
```
#include <stdio.h>

unsigned long long calculateProduct(int n) {
    if (n == 1)
        return 1;
    else
        return n * calculateProduct(n - 1);
}

int main() {
    int n = 12;
    unsigned long long product;

    product = calculateProduct(n);

    printf("Product of first 12 natural numbers: %llu\n", product);

    return 0;
}
```
## OUTPUT:

w![image](https://github.com/user-attachments/assets/78fa125f-1f8a-4ec3-8d60-54bdc6e06b99)
       		
## RESULT:

Thus the program has been executed successfully.
 
 <hr>


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
```c
#include <stdio.h>

int main() {
    int matrix[3][3];
    int i, j, sum;

    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }

    for (i = 0; i < 3; i++) {
        sum = 0;
        for (j = 0; j < 3; j++) {
            sum += matrix[i][j];
        }
        printf("Sum of row %d = %d\n", i + 1, sum);
    }

    return 0;
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/c9b6fe68-0669-4e5c-9838-82d4de516274)

 
 

 ## RESULT
Thus the program has been executed successfully.

<hr>

# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

## Algorithm

1. Input the string and the number of rows for the pyramid.
2. Initialize variables:
   - `i` for the row count (starting from 0).
   - `j` for printing the string in each row.
   - `k` for printing spaces for alignment.
3. Start a loop for `i` from `0` to `rows - 1` (for each row of the pyramid):
   - Print leading spaces to center the pyramid (`rows - i - 1` spaces).
   - Start an inner loop for `j` from `0` to `i`:
     - Print the string followed by a space.
   - Move to the next line.
4. End the program.


## PROGRAM:
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[100];
    int rows;

    scanf("%s", str);
    scanf("%d", &rows);

    for (int i = 0; i < rows; i++) {
        for (int k = 0; k < rows - i - 1; k++) {
            printf("  ");
        }
        for (int j = 0; j <= i; j++) {
            printf("%s ", str);
        }
        printf("\n");
    }

    return 0;
}

```

 ## OUTPUT
![image](https://github.com/user-attachments/assets/9290a727-73b3-4951-b3c9-142aa77664d2)

 

## RESULT

Thus the C program to String process executed successfully
 

 
.<hr>



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int arr[10], n, i;
    int *parr;

    parr = arr;

    scanf("%d", &n);

    for (i = 0; i < n; i++) {
        scanf("%d", parr + i);
    }

    for (i = 0; i < n; i++) {
        printf("%d ", *(parr + i));
    }

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/caf5fc6f-be20-46ad-90f3-a2c4a2e79853)

 

## RESULT
Thus the C program to read and display an array of any 6 integer elements using pointer has been executed
<HR>

