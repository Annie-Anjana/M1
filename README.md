
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    char a, b, c;
    printf("Enter first character: ");
    scanf(" %c", &a);

    printf("Enter second character: ");
    scanf(" %c", &b);

    printf("Enter third character: ");
    scanf(" %c", &c);
    printf("Characters in reverse order: %c %c %c\n", c, b, a);

    return 0;
}


```
## OUTPUT:

<img width="804" height="314" alt="Screenshot 2025-11-14 134908" src="https://github.com/user-attachments/assets/3d11de0e-733c-4d33-a8aa-cc94db0df434" />

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```


#include <stdio.h>

int main() {
    int A;
    printf("Enter a value for A: ");
    scanf("%d", &A);
    if (A > 0)
	{
        printf("%d is a positive number.\n", A);
    }
else
	{
        printf("%d is not a positive number.\n", A);
    }

    return 0;
}

```
# OUTPUT:

<img width="811" height="210" alt="Screenshot 2025-11-14 135204" src="https://github.com/user-attachments/assets/205380d7-e259-4f2c-b60e-76f5ddcf923f" />


<img width="813" height="234" alt="Screenshot 2025-11-14 135219" src="https://github.com/user-attachments/assets/3dbf14af-6dfe-456b-94f7-c351080b3e5e" />


# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>

int main() {
    float num1, den1, num2, den2;
    float value1, value2, min;
    printf("Enter numerator and denominator of first fraction: ");
    scanf("%f %f", &num1, &den1);
    printf("Enter numerator and denominator of second fraction: ");
    scanf("%f %f", &num2, &den2);
    value1 = num1 / den1;
    value2 = num2 / den2;
    min = (value1 < value2) ? value1 : value2;
    printf("Minimum value between the two fractions is: %.4f\n", min);

    return 0;
}


```

## OUTPUT:


<img width="812" height="257" alt="Screenshot 2025-11-14 135608" src="https://github.com/user-attachments/assets/355e02a2-3c1c-49b6-ba1e-bd157680fdf0" />


## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.



# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int value;

    // Read input
    printf("Enter a value: ");
    scanf("%d", &value);

    // Check if value equals 1
    if (value == 1) {
        printf("The value is equal to 1.\n");
    } else {
        printf("The value is not equal to 1.\n");
    }

    return 0;
}
```
## OUTPUT:

<img width="818" height="256" alt="Screenshot 2025-11-14 135840" src="https://github.com/user-attachments/assets/5c72023f-2284-4863-9a74-8a1981628296" />

<img width="817" height="243" alt="Screenshot 2025-11-14 135818" src="https://github.com/user-attachments/assets/26a31f6c-a4ee-41cd-b14a-f5f91f9c1966" />


## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include <stdio.h>

int main() {
    int m1, m2, m3;
    float tot, per;
    printf("Enter marks for three subjects: ");
    scanf("%d %d %d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3;
    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60)
            printf("Division = First\n");
        else if (per >= 48)
            printf("Division = Second\n");
        else if (per >= 36)
            printf("Division = Pass\n");
    } 
    else {
        printf("Division = Fail\n");
    }

    return 0;
}
```
## OUTPUT:

<img width="809" height="262" alt="Screenshot 2025-11-14 140039" src="https://github.com/user-attachments/assets/e04f79f2-ed62-45a5-a2dc-2be21edfc08e" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

