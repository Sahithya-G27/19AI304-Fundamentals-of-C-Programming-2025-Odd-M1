# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 13/11/2025 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int a = 25;
    float b = 12.5;
    char c = 'A';
    char str[] = "Hello, C Programming";

    printf("Integer literal value   : %d\n", a);
    printf("Float literal value     : %.2f\n", b);
    printf("Character literal value : %c\n", c);
    printf("String literal value    : %s\n", str);

    return 0;
}

```

# Output:
<img width="1461" height="577" alt="image" src="https://github.com/user-attachments/assets/6fff34a4-0070-4548-9434-eb73b0e60d0d" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 13/11/2025
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>
#define PI 3.14

int main() 
{
    const int MAX = 100;

    printf("Value of macro constant PI = %.2f\n", PI);
    printf("Value of constant variable MAX = %d\n", MAX);

    return 0;
}
```

# Output:
<img width="1211" height="451" alt="image" src="https://github.com/user-attachments/assets/e72cccca-0979-4fdc-9fe1-a561d8b66d43" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 13/11/2025
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int a = 10;
    float b = 5.25f;
    double c = 123.456789;
    char d = 'C';

    printf("Integer value   : %d\n", a);
    printf("Float value     : %.2f\n", b);
    printf("Double value    : %.6lf\n", c);
    printf("Character value : %c\n", d);

    return 0;
}
```
# Output:
<img width="1222" height="558" alt="image" src="https://github.com/user-attachments/assets/50e04e52-7c5f-4702-9ada-505bf82d3422" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 13/11/2025
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter two integers:\n");
    scanf("%d %d", &a, &b);
    printf("\n--- Arithmetic Operations ---\n");
    printf("Addition        = %d\n", a + b);
    printf("Subtraction     = %d\n", a - b);
    printf("Multiplication  = %d\n", a * b);

    if (b != 0)
     {
        printf("Division        = %d\n", a / b);
        printf("Remainder       = %d\n", a % b);
    } else 
    {
        printf("Division and Remainder not possible (division by zero)\n");
    }
    printf("\n--- Bitwise Operations ---\n");
    printf("Bitwise AND     = %d\n", a & b);
    printf("Bitwise OR      = %d\n", a | b);
    printf("Bitwise XOR     = %d\n", a ^ b);
    printf("Left Shift (a<<1)  = %d\n", a << 1);
    printf("Right Shift (a>>1) = %d\n", a >> 1);
    printf("Bitwise NOT of a  = %d\n", ~a);

    return 0;
}
```

# Output:

<img width="1197" height="647" alt="image" src="https://github.com/user-attachments/assets/eb2a8d2b-13a0-4f6d-bb79-fb3af639beac" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 13/11/2025
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
#include <ctype.h>
int main() {
    char ch;
    printf("Enter a character: ");
    scanf("%c", &ch);

    (isdigit(ch)) ? 
        printf("The character is a Digit.\n") :
    (isalpha(ch)) ?
        ((ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
          ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U') ?
            printf("The character is a Vowel.\n") :
            printf("The character is a Consonant.\n")) :
        printf("The character is a Special Symbol.\n");

    return 0;
}
```
# Output:

<img width="1307" height="597" alt="image" src="https://github.com/user-attachments/assets/96f325f2-29ae-4549-824d-48254bead6d0" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


