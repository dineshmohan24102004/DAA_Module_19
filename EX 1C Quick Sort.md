# EX 1C Quick Sort

## AIM:
To write a Python program to sort a list of elements using the Quick Sort algorithm.

## Algorithm
Start the program.

Input the number of elements n and read the elements into the list arr.

Implement the function partition(alist, start, end):

Select the first element as the pivot.

Initialize two pointers i (from left) and j (from right).

Move i forward until an element greater than the pivot is found.

Move j backward until an element smaller than the pivot is found.

If i <= j, swap the elements at i and j.

If i > j, swap the pivot with alist[j] and return the pivot position.

Implement the function quickSort(alist, start, end):

If the array has more than one element, partition the array.

Recursively apply quickSort to the left and right subarrays divided by the pivot.

Call quickSort(arr, 0, n) to sort the list.

Display the sorted array.

Stop.

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: Dinesh M
Register Number:212222040039

def quickSort(alist, start, end):  
    if end - start > 1:      
        p = partition(alist, start, end)       
        quickSort(alist, start, p)       
        quickSort(alist, p + 1, end) 
def partition(alist, start, end):   
    pivot = alist[start]   
    i = start + 1   
    j = end - 1    
    #print("Pivot: ",pivot)   
    while True:       
        while (i <= j and alist[i] <= pivot):            
            i = i + 1       
        while (i <= j and alist[j] >= pivot):       
            j = j - 1        
        if i <= j:           
            alist[i], alist[j] = alist[j], alist[i]       
        else:            
            alist[start], alist[j] = alist[j], alist[start]          
            return j
arr = []
n=int(input())
for i in range(n):   
    arr.append(str(input()))
quickSort(arr, 0, n)
print("Sorted array is:")
for i in arr:  
    print(i)
*/
```

## Output:
<img width="1275" height="783" alt="Screenshot 2025-09-07 171131" src="https://github.com/user-attachments/assets/8d8b0e09-c1b3-43b1-acda-6b9113ee8543" />



## Result:
The program successfully sorts the given list of elements in ascending order using the Quick Sort technique.
