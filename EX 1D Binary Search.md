# EX 1D Binary Search
## DATE: 26/02/25
## AIM:
To write a python program to implement the binary search on the given list of characters.

## Algorithm

1. Input and sort the array.  
2. Read the target element `x`.  
3. Use binary search:  
   - Check middle element.  
   - Narrow search to left or right half.  
4. Repeat until found or range is empty.  
5. Print result (index or not found).  

## Program:
```
/*
Program to implement Reverse a String
Developed by: SANTHIYA R
Register Number: 212223230192 
*/
```
```
def binarySearchAppr(arr,l,r, x):
    while l<=r:
        mid=(l+r)//2
        if arr[mid]==x:
            return mid
        elif arr[mid]>x:
            r=mid-1
        else:
            l=mid+1
    return -1
        
arr=[]
n=int(input())
for i in range(n):
    arr.append(input())
arr=sorted(arr)
x=input()
res=binarySearchAppr(arr, 0, len(arr)-1, x)
if res!=-1:
    print("Element is present at index "+str(res))
else:
    print("Element is not present in array")
```

## Output:

![image](https://github.com/user-attachments/assets/20546cc0-6298-4d4a-ad1e-7e2277e4df8c)


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list.
