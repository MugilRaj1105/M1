
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
```
1.Declare three character variables to store the input characters.
2.Use the scanf function to read the characters one by one from the user.
3.Print the characters in reverse order using the printf function.
4.End the program.
```
## PROGRAM:
```
#include <stdio.h>
int main()
{
    char ch,ch1,ch2;
    scanf("%c%c%c",&ch,&ch1,&ch2);
    printf("The reverse of %c%c%c is %c%c%c",ch,ch1,ch2,ch2,ch1,ch);
    return 0;
    
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/3de26c1a-84a5-4f4e-8db7-519e0bfb8b4f)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
```
1.Declare a variable to store the input value A.
2.Use the scanf function to read the value of A from the user.
3.Check if the value of A is greater than zero.
4.If A is greater than zero, print a message indicating that it's a positive number. 
5.Otherwise, print a message indicating that it's not a positive number.
6.End the program.
```
# PROGRAM:
```
#include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if (a>=0)
    {
        printf("Number is positive.");
    }
    else
    {
        printf("Number is negative.");
    }
    return 0;
}
```
# OUTPUT:

![image](https://github.com/user-attachments/assets/749205cb-d2c4-4c0c-ab82-1da8b565074b)

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
```
1.Declare variables to store the two fraction numbers and the result.
2.Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.Use the scanf function to read the numerator and denominator of the first fraction.
4.Repeat steps 2 and 3 to get the second fraction from the user.
5.Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.Print the minimum value.
```
## PROGRAM:
```
#include <stdio.h>

int main() {
    int num1, den1, num2, den2;
    float frac1, frac2, result;

    printf("Enter numerator and denominator of first fraction: ");
    scanf("%d %d", &num1, &den1);

    printf("Enter numerator and denominator of second fraction: ");
    scanf("%d %d", &num2, &den2);

    frac1 = (float)num1 / den1;
    frac2 = (float)num2 / den2;

    result = (frac1 < frac2) ? frac1 : frac2;

    printf("Minimum value = %.4f\n", result);

    return 0;
}

```
## OUTPUT:

![Screenshot 2025-05-30 140410](https://github.com/user-attachments/assets/64766153-3cd0-4791-9ef8-6c59c70b0d3f)

## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
```
1.Declare a variable to store the input value.
2.Use the scanf function to read the input value from the user.
3.Use an if statement to check if the input value is equal to 1.
4.If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.Otherwise, print a message indicating that it's not equal to 1.
6.End the program.
```
## PROGRAM:
```
#include <stdio.h>
int main(){
    int a;
    scanf("%d",&a);
    if(a==1)
       printf("TRUE");
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/7e989890-323c-4121-9a3d-d0759c7ccf4a)

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
```
1.Start
2.Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.Input the marks for three subjects.
4.Calculate total marks: tot = m1 + m2 + m3
5.Calculate percentage: per = tot / 3
6.Display total and percentage.
7.Check if all marks are greater than or equal to 40:
8.If yes:
a.If percentage >= 60: Print “Division = First”
b.Else if percentage >= 48: Print “Division = Second”
c.Else if percentage >= 36: Print “Division = Pass”
9.Else: Print “Division = Fail”
10.End
```
## PROGRAM:
```
#include <stdio.h>

int main() {
    int m1, m2, m3, total;
    float percentage;

    printf("Enter marks of three subjects:\n");
    scanf("%d %d %d", &m1, &m2, &m3);

   
    total = m1 + m2 + m3;
    percentage = total / 3.0;

    
    printf("Total Marks = %d\n", total);
    printf("Percentage = %.2f%%\n", percentage);

   
    if (m1 < 33 || m2 < 33 || m3 < 33) {
        printf("Result: Fail (One or more subjects below 33)\n");
    } else if (percentage >= 60) {
        printf("Result: First Division\n");
    } else if (percentage >= 50) {
        printf("Result: Second Division\n");
    } else if (percentage >= 40) {
        printf("Result: Pass\n");
    } else {
        printf("Result: Fail\n");
    }

    return 0;
}
```

## OUTPUT:

![WhatsApp Image 2025-05-30 at 14 08 05_7dfd2b50](https://github.com/user-attachments/assets/014a4243-8dd9-470f-af63-3f5b7a1f931e)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

