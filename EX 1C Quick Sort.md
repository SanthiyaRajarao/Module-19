# EX 1C Quick Sort
## DATE: 25/02/25
## AIM: 
To write a python to implement Quick sort using the first element as pivot value.

## Algorithm

1. Read `n` integers into a list.  
2. Choose the first element as the pivot. Rearrange elements so that smaller values are to its left and larger to its right.  
3. Swap elements as needed to partition correctly, and place the pivot in its correct sorted position.  
4. Recursively apply quick sort to the left and right sublists around the pivot.  
5. Print the pivot during sorting and the fully sorted array at the end.

## Program:
```
/*
Program to implement Reverse a String
Developed by: SANTHIYA R
Register Number: 212223230192
*/
```
```
def partition(arr,low,high):
    pivot=arr[low]
    i=low+1
    j=high
    
    while True:
        while i<=j and arr[i]<=pivot:
            i+=1
        while i<=j and arr[j]>pivot:
            j-=1
        if i<=j:
            arr[i],arr[j]=arr[j],arr[i]
        else:
            break
    arr[low],arr[j]=arr[j],arr[low]
    return j
    
def quick_sort(arr,low,high):
    if low<high:
        pivot_index=partition(arr,low,high)
        print("Pivot: ",arr[pivot_index])
        quick_sort(arr,low,pivot_index-1)
        quick_sort(arr,pivot_index+1,high)

n=int(input())
arr=[]
for i in range(n):
    arr.append(int(input()))
quick_sort(arr,0,len(arr)-1)
print("Sorted array:",arr)
```
## Output:

![image](https://github.com/user-attachments/assets/38c1810d-da68-44fe-826d-2ae5b28291bd)


## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
