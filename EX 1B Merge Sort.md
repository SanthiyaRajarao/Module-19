# EX 1B Merge Sort
## DATE: 25/02/25
## AIM:
To Write a python program for the implementation of merge sort on the given list of float values.

## Algorithm

1. Read `n` elements into an array.  
2. Recursively split the array into two halves until each has one element.  
3. Sort each half by recursive calls to `mergesort()`.  
4. Combine the sorted halves by comparing and inserting elements into the original array.  
5. Print the original and sorted arrays.

## Program:
```
/*
Program to implement Reverse a String
Developed by: SANTHIYA R
Register Number: 212223230192
*/
```
```
def mergesort(arr):
    if len(arr)>1:
        mid=len(arr)//2
        l=arr[:mid]
        r=arr[mid:]
        mergesort(l)
        mergesort(r)
        i=j=k=0
        while i<len(l) and j<len(r):
            if l[i]<r[j]:
               arr[k]=l[i]
               i+=1
            else:
               arr[k]=r[j]
               j+=1
            k+=1
        while i<len(l):
            arr[k]=l[i]
            i+=1
            k+=1
        while j<len(r):
            arr[k]=r[j]
            j+=1
            k+=1
    
def printlist(arr):
        for i in range(len(arr)):
            print(arr[i],end=" ")
        print()
        
n=int(input())
arr=[]
for i in range(n):
    element=float(input())
    arr.append(element)
    
print("Given array is",end="\n")
printlist(arr)
mergesort(arr)
print("Sorted array is",end="\n")
printlist(arr)
        
```
## Output:

![image](https://github.com/user-attachments/assets/52506282-2250-40fb-a2e4-e23a3cdd21cf)


## Result:
The program successfully sorts the values using merge sort. When the user provides an input values, the output displays in the sorted way.
