# EX 1B Harmonic Sum
## DATE: 25/02/25
## AIM:
To Write a Python program to calculate the harmonic sum of n-1.

## Algorithm

1. Take an integer input `n` from the user.  
2. If `n < 2`, return 1 (base case).  
3. Otherwise, calculate `1/n` and add it to `harmonic(n-1)`.  
4. Repeat step 3 recursively until base case is reached.  
5. Return and print the final harmonic sum. 

## Program:
```
/*
Program to implement Reverse a String
Developed by: SANTHIYA R
Register Number: 212223230192
*/
```
```
def harmonic(n):
    if n<2:
        return 1
    else:
        return 1/n+harmonic(n-1)
        
n=int(input())
print(harmonic(n))
```

## Output:
![image](https://github.com/user-attachments/assets/75b43c51-1cb7-424e-871f-b20f97401215)

## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
