
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
int main()
{
    char ch1,ch2,ch3;
    scanf("%c",&ch1);
    scanf("%c",&ch2);
    scanf("%c",&ch3);
    printf("The reverse of %c%c%c is %c%c%c\n",ch1,ch2,ch3,ch3,ch2,ch1);
    return 0;
}
```

## OUTPUT:
![437957528-7ea87db5-9fe6-4aa9-b0fd-01894e62bc4e](https://github.com/user-attachments/assets/69e28ab6-e500-4efa-b41f-21aeec641193)
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

int main()
{
    int A;
    scanf("%d", &A);
    
    if(A >= 0)
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
![437958255-2d9d1c7d-c96b-401c-8f04-2ec3df4fcbd9](https://github.com/user-attachments/assets/9f31fd17-f960-4e50-85f1-8f157082ac15)

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
    float num1, den1, num2, den2, fraction1, fraction2;
    scanf("%f %f", &num1, &den1);
    scanf("%f %f", &num2, &den2);
    fraction1 = num1 / den1;
    fraction2 = num2 / den2;
    float min = (fraction1 < fraction2) ? fraction1 : fraction2;

    printf("Minimum between %f and %f is %.3f\n", min);

    return 0;
}
```


## OUTPUT:
![437960554-50067201-bb87-4a82-bb9e-d1552d52349c](https://github.com/user-attachments/assets/3a5df903-332f-4f10-8eba-3bc7eed4b765)

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

int main()
{
    int A;
    scanf("%d", &A);
    
    if(A == 1)
    {
        
        printf("The input value is equal to 1.\n");
    }
    else
    {
       
        printf("The input value is not equal to 1.\n");
    }

    return 0;
}
```


## OUTPUT:
![437960428-9f830fcc-7414-4f23-b606-bab700e54f21](https://github.com/user-attachments/assets/32856f14-9482-417c-877a-7e8d61a6aa20)

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
#include <string.h>

int main()
{
    int phy,che,ca,total;
    float per;
    char div[10];

   
    scanf("%d%d%d",&phy,&che,&ca);
    total = phy+che+ca;
    per = total/3.0;
    if (per>=60)
	 strcpy(div,"First");
    else if (per<60 && per>=48)
	    strcpy(div,"Second");
	else
	    if (per<48&&per>=36)
		    strcpy(div,"Pass");
	    else
		    strcpy(div,"Fail");

      
       printf("Total Marks = %d\nPercentage = %5.2f\nDivision = %s\n",total,per,div);
       return 0;
}
```

## OUTPUT:
![437961798-67d65316-d094-43a0-86aa-f211567670bb](https://github.com/user-attachments/assets/c1ed4495-b254-4f69-8dee-62d9e1e7dee8)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

