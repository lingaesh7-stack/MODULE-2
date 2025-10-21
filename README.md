# NAME : LINGAESHWAR K
# REGISTER NUMBER : 25016881

# MODULE-2
Module 2 repository
# C Programming Practice Programs – Series, Patterns, Functions, and Loops

This repository contains 5 C programs demonstrating fundamental concepts such as loops, functions, pattern printing, and basic number operations. Each program includes its *Aim, **Algorithm, and placeholders for **Source Code* and *Sample Output*.

---
# C Programming Practice Programs – Loops, Patterns, and Functions

This repository contains 5 C programs demonstrating concepts such as loops, pattern printing, functions, and basic number operations. Each program includes *Aim* and *Algorithm*.

---

## Programs Included
1. Print 1 to n Odd Numbers  
2. Hollow Square Pattern using For Loop  
3. Factorial of a Number using Function (Without Return Type, With Arguments)  
4. Check Palindrome using For Loop  
5. Multiplication Table using Do-While Loop  

---

### 1. Print 1 to n Odd Numbers

*Aim:*

Print all odd numbers from 1 to a user-provided number n.  

*Algorithm:*  

1. Ask the user to input a number n.  
2. Loop from 1 to n.  
3. Check if the current number is odd (num % 2 != 0).  
4. Print the odd numbers.

*source code*

```c
#include<stdio.h>
int main()
{
    int num,i;
    scanf("%d",&num);
    for(i=1;i<=num;i +=2){
        printf("%d ",i);
    }
    return 0;
}
```

*output*

<img width="575" height="160" alt="image" src="https://github.com/user-attachments/assets/2cc1a847-974a-48ed-a56b-2eb453965a0d" />


*Result:*

The program displays all odd numbers from 1 up to the entered number n.

---

# 2. Hollow Square Pattern using For Loop

*Aim:*

Print a hollow square pattern of size n using for loops.  

*Algorithm:*

1. Ask the user to input the size n of the square.  
2. Loop through rows (1 to n) and columns (1 to n).  
3. Print * for the borders (first row, last row, first column, last column).  
4. Print space for inner positions.

*source code*

```c
#include<stdio.h>
int main()
{
    int num,i,j;
    scanf("%d",&num);
    for(i=1;i<=num;i++){
        for(j=1;j<=num;j++){
            if(i==num||i==1||j==1||j==num){
                printf("#");
            }
            else
                printf(" ");
                    }
            printf("\n")
                    }
    return 0;
}
```

*output*

<img width="406" height="253" alt="image" src="https://github.com/user-attachments/assets/b0a92da2-3cce-4d7d-8d96-9f8db9d490c4" />


*Result:*  

The program successfully prints a hollow square pattern of stars (*) with the given size.

---

### 3. Factorial of a Number using Function (Without Return Type, With Arguments)

*Aim:* 

Find the factorial of a given number using a function without return type but with arguments.  

*Algorithm:*

1. Ask the user to input a number n.  
2. Create a function factorial(int n) that calculates the factorial.  
3. Use a loop inside the function to compute factorial.  
4. Print the factorial from within the function.

*source code*

```c
#include<stdio.h>
void fact(int num)
{
    int fact=1,i;
    for(i=1;i<=num;i++)
    {
        fact=fact*i;
    }
    printf("Factorial value is: %d",fact);
    
}
int main()
{
    int n;
    scanf("%d",&n);
    fact(n);
    return 0;
}
```

*output*

<img width="595" height="87" alt="image" src="https://github.com/user-attachments/assets/cf57ce5b-a598-41ea-9480-27f02306ecf9" />



*Result:*  

The program computes and displays the factorial of the entered number using a function with arguments and no return type.

---

### 4. Check Palindrome using For Loop

*Aim:*

Check if the input entered by the user is a palindrome.  

*Algorithm:*  

1. Ask the user to input a number.  
2. Store the input in a variable.  
3. Use a for loop to compare the characters/digits from start and end.  
4. If all characters/digits match, it is a palindrome; else it is not.

*source code*

```c
#include<stdio.h>
int main()
{
    int num,rem;
    int original;
    int reversed=0;
    scanf("%d",&num);
    original = num;
    for(;num!=0;num /= 10){
        rem=num%10;
        reversed = reversed*10+rem;
        
  }
    if(original==reversed){
        printf("Palindrome Number");
    }
        else
    {
        printf("Not a Palindrome Number");
    }
    return 0;
```

    
*output*

<img width="495" height="133" alt="image" src="https://github.com/user-attachments/assets/ce350c0c-3648-48d4-9a4a-6cf52409d323" />



*Result:*  

The program determines and displays whether the given number is a palindrome.



---

### 5. Multiplication Table using Do-While Loop

*Aim:*

Print the multiplication table of a user-provided number using a do-while loop.  

*Algorithm:*  

1. Ask the user to input a number n.  
2. Initialize a counter i = 1.  
3. Use a do-while loop to multiply n by i and print the result.  
4. Increment i until it reaches 10.

*source code*

```c
#include <stdio.h>

int main()
{
 int num,i=1;
 scanf("%d", &num);
 do {
     printf("%d ",num*i);
     i++;
    }
    while(i<=num);
    
     
 return 0;

}
```


*output*

<img width="639" height="139" alt="image" src="https://github.com/user-attachments/assets/453e9fc4-031f-4fb0-ace3-f3170666d1d8" />


*Result:* 

The program prints the complete multiplication table of the user-entered number from 1 to 10 using a do-while loop.
