# EX 1B Merge Sort
## DATE:
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
Start the program.

Input the size of the array n and read n elements into the array.

Implement the function merge(arr, l, m, r):

Divide the array into two temporary subarrays L and R.

Compare elements of both subarrays and merge them back into the original array in sorted order.

Implement the recursive function mergeSort(arr, l, r):

If l < r, find the middle index m.

Recursively call mergeSort for the two halves of the array.

Merge the two sorted halves using the merge function.

Display the given (unsorted) array.

Apply mergeSort on the array.

Display the sorted array.

Stop.

## Program:
```
/*
Program to implement Merge Sort
Developed by: Dinesh M
Register Number: 212222040039

def merge(arr,l,m,r):
    n1=m-l+1
    n2=r-m
    L=[0]*(n1)
    R=[0]*(n2)
    for i in range(0,n1):
        L[i]=arr[l+i]
    for j in range(0,n2):
        R[j]=arr[m+1+j]
    
    i=0
    j=0
    k=l
    
    while i<n1 and j<n2:
        if(L[i]<=R[j]):
            arr[k]=L[i]
            i+=1
        else:
            arr[k]=R[j]
            j+=1
        k+=1
    while i<n1:
        arr[k]=L[i]
        i+=1
        k+=1
    while j<n2:
        arr[k]=R[j]
        j+=1
        k+=1
def mergeSort(arr,l,r):
    if l<r:
        m=l+(r-l)//2
        mergeSort(arr,m+1,r)
        merge(arr,l,m,r)
        
arr=[]
n=int(input())
for i in range(n):
    arr.append(int(input()))
print("Given array is")
for i in range(n):
    print(arr[i],end=' ')
mergeSort(arr,0,n-1)
print("\n\nSorted array is")
for i in range(n):
    print(arr[i],end=' ')


*/
```

## Output:

<img width="1084" height="468" alt="image" src="https://github.com/user-attachments/assets/5e1a8ed8-bc27-4fb5-abdf-5ca4d94722ad" />


## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
