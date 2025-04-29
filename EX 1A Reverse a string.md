# EX 1A Reverse a String
## DATE: 24/02/25
## AIM:
To write a program to create a recursive function to reverse a string.

## Algorithm

1. Take input string from the user.  
2. If the string is empty, return it.  
3. Call `reverse()` on the substring excluding the first character.  
4. Add the first character to the end of the reversed substring.  
5. Return and print the result.  

## Program:
```
/*
Program to implement Reverse a String
Developed by: SANTHIYA R
Register Number: 212223230192
*/
```

```
def reverse(str):
    if len(str)==0:
        return str
    else:
        return(reverse(str[1:])+str[0])
    
str=input()
print(reverse(str))
```

## Output:

![image](https://github.com/user-attachments/assets/80ba9426-d875-4fbc-82df-fa4077209f30)


## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
