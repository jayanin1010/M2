# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:

    #include <stdio.h>
    
    int main() {
        int M, N, i;
        printf("Enter the starting value (M): ");
        scanf("%d", &M);
        printf("Enter the ending value (N): ");
        scanf("%d", &N);
    
        for (i = M; i <= N; i++) {
            if (i % 2 == 0) {
                printf("%d ", i);
            }
        }
        printf("\n");
        return 0;
    }


## OUTPUT:

![image](https://github.com/user-attachments/assets/71cbfba5-d740-4b4d-8fab-4c029b5454a7)


## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:


    #include <stdio.h>
    
    int main() {
        int rows, i, j;
    
        printf("Enter the number of rows: ");
        scanf("%d", &rows);
    
        for (i = 1; i <= rows; i++) {
            for (j = 1; j <= i; j++) {
                printf("*");
            }
            printf("\n");
        }
    
        return 0;
    }


## OUTPUT:


![image](https://github.com/user-attachments/assets/f8e3af4c-e208-4b3d-8c9d-31873914b0e3)



## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:

    #include <stdio.h>
    
    void add(int a, int b);
    void subtract(int a, int b);
    
    int main() {
        int num1, num2;
        printf("Enter the first number: ");
        scanf("%d", &num1);
        printf("Enter the second number: ");
        scanf("%d", &num2);
    
        add(num1, num2);
        subtract(num1, num2);
    
        return 0;
    }
    
    void add(int a, int b) {
        int sum = a + b;
        printf("Addition: %d\n", sum);
    }
    
    void subtract(int a, int b) {
        int diff = a - b;
        printf("Subtraction: %d\n", diff);
    }

## OUTPUT:


![image](https://github.com/user-attachments/assets/136292ed-e5ab-4ffd-b86c-5b62a665a98f)




## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:

    #include <stdio.h>
    
    int main() {
        int num, sum = 0, digit, i;
        scanf("%d", &num);
    
        for (i = num; i != 0; i /= 10) {
            digit = i % 10;
            if (digit % 2 != 0) {
                sum += digit;
            }
        }
    
        printf("%d\n", sum);
    
        return 0;
    }


## OUTPUT:

![image](https://github.com/user-attachments/assets/4f294f41-8d2f-45d5-a7fd-055bbcd50a00)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:

    #include <stdio.h>
    
    void fact(int N) {
        int i;
        long long fact = 1;
        for (i = 1; i <= N; i++) {
            fact = fact * i;
        }
        printf("Factorial of %d is: %lld\n", N, fact);
    }
    
    int main() {
        int n;
        printf("Enter a number: ");
        scanf("%d", &n);
        fact(n);
        return 0;
    }

## OUTPUT:

![image](https://github.com/user-attachments/assets/8faf04de-1085-4467-b3f5-671ac9abc05d)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
