EX-11-EMI-CALCULATOR
AIM
To write a program to prepare EMI calculator using function without return type and with arguments.

ALGORITHM
Start the program.
Read principal amount, rate of interest and months.
Pass these values as arguments to function.
Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
Display the result.
Stop the program.
PROGRAM
#include <stdio.h>
#include <math.h>

float emi(float p, float r, int t) {
    r = r / (12 * 100);
    return (p * pow(1 + r, t)) / (pow(1 + r, t) - 1);
}

int main() {
    float p, r;
    int t;
    printf("Enter principal, rate, months: ");
    scanf("%f %f %d", &p, &r, &t);
    printf("EMI = %.2f\n", emi(p, r, t));
    return 0;
}

OUTPUT
image

RESULT
Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully

EX-12-FIBONACCI-SERIES
AIM
To write a C program to generate the Fibonacci series for the value 6.

ALGORITHM
Start the program.
Read number of terms to display.
Add the previous two terms and store it in new term.
Assign 2nd term to 1st term and 3rd term to 2nd term.
Repeat steps 3 and 4 n number of times.
Display the result.
Stop the program.
PROGRAM
#include <stdio.h>

int main() {
    int n, a = 0, b = 1, c, i;
    printf("Enter number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series: ");
    for(i = 1; i <= n; i++) {
        printf("%d ", a);
        c = a + b;
        a = b;
        b = c;
    }
    return 0;
}

OUTPUT
image

RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.

EX-13-ONE-DIMENSIONAL-ARRAY
AIM
To write a C program to read n elements as input and print the last element of the array.

ALGORITHM
Start the program.
Read a variable.
Read the array values n number of times.
Print the last element.
Stop the program.
PROGRAM
#include <stdio.h>

int main() {
    int n, i, arr[100];
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Last element = %d\n", arr[n-1]);
    return 0;
}

OUTPUT
image

RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.

EX-14-POSITIVE-ARRAY-ELEMENTS
AIM
To write a C Program to count total number of positive elements in an array.

ALGORITHM
Start the program.
Read a variable.
Read the array values n number of times.
If the array value can be divided by 2 then increment count by 1.
Display result.
Stop the program.
PROGRAM
#include <stdio.h>

int main() {
    int n, i, x, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d numbers: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &x);
        if(x % 2 == 0)
            count++;
    }

    printf("Count of numbers divisible by 2 = %d\n", count);
    return 0;
}

OUTPUT
image

RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.

EX -15 - Replace All Even Elements With 'E' In One Dimensional Array
Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

Algorithm:
Input the array: Read the size of the array. Input the elements of the array.
Iterate through the array: For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
Replace even elements with 'E': If an element is even, replace that element with the character 'E'.
Output the updated array: Print the updated array after replacements.
Program:
#include <stdio.h>

int main() {
    int n, i, arr[100];
    printf("Enter array size: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Updated array: ");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    return 0;
}

Output:
image

Result:
Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.
