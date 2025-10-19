# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>

void calculateEMI(double principal, double rate, int months);

int main() {
    double principal, rate;
    int months;

    printf("Enter principal amount: ");
    scanf("%lf", &principal);
    printf("Enter annual interest rate (in %%): ");
    scanf("%lf", &rate);
    printf("Enter number of months: ");
    scanf("%d", &months);

    calculateEMI(principal, rate, months);

    return 0;
}

void calculateEMI(double principal, double rate, int months) {
    double monthlyRate = rate / (12 * 100); // Convert annual rate to monthly fraction
    double emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) /
          (pow(1 + monthlyRate, months) - 1);

    printf("Your EMI is: %.2lf\n", emi);
}
```


## OUTPUT


<img width="474" height="258" alt="Screenshot 2025-10-19 184708" src="https://github.com/user-attachments/assets/777cd3c7-8110-4d04-a652-9e9b580a8257" />



## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 6; // Number of terms
    int t1 = 0, t2 = 1, nextTerm, i;

    printf("Fibonacci Series for %d terms: ", n);
    printf("%d %d ", t1, t2);

    for(i = 3; i <= n; i++) {
        nextTerm = t1 + t2;
        printf("%d ", nextTerm);
        t1 = t2;
        t2 = nextTerm;
    }

    printf("\n");
    return 0;
}
```

## OUTPUT

<img width="497" height="122" alt="Screenshot 2025-10-19 184810" src="https://github.com/user-attachments/assets/58247b16-bd63-4d4e-af89-fcd30877582d" />







## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];  

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("The last element of the array is: %d\n", arr[n-1]);

    return 0;
}
```

## OUTPUT


<img width="469" height="192" alt="Screenshot 2025-10-19 184936" src="https://github.com/user-attachments/assets/710f34a7-134f-4983-bef4-e82749d662c3" />







## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, i, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < n; i++) {
        if(arr[i] > 0) {  
            count++;
        }
    }

    printf("Total number of positive elements = %d\n", count);
    return 0;
}
```



## OUTPUT



<img width="455" height="211" alt="Screenshot 2025-10-19 185040" src="https://github.com/user-attachments/assets/81dfccf8-ad77-4014-b627-eae07f3c1043" />


## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n, i;
    int arr[100]; 

    printf("Enter the size of the array: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    printf("\n");
    return 0;
}
```


## Output:
 
<img width="455" height="211" alt="Screenshot 2025-10-19 185040" src="https://github.com/user-attachments/assets/542ba4ee-d001-4447-bb96-aa74702988d4" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



