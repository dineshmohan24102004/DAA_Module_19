# EX 1D Linear search
## DATE:
## AIM:
To write a Python program to perform a linear search on a list of elements and check whether a given key element is present or not.



## Algorithm
Start the program.

Read the number of elements n.

Initialize an empty list List.

Read n elements from the user and store them in the list.

Read the search key element key.

Call the function search(List, n) which:

Iterates through the list from index 0 to n-1.

If list[i] == key, return the index i.

If not found after the loop, return -1.

If the function returns -1, display "Not Found".

Otherwise, display "Found".

Stop the program.

## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: Dinesh M
Register Number: 212222040039

global key
def search (list,n):
    for i in range(0,n):
        if(list[i]==key):
            return i
    return -1
n=int(input())
List=[]
for i in range(0,n):
    temp=input()
    List.append(temp)
key=input()
res=search(List,n)
if(res==-1):
    print("Not Found")
else:
    print("Found")
*/
```

## Output:

<img width="1298" height="769" alt="Screenshot 2025-09-07 171446" src="https://github.com/user-attachments/assets/c42f55b3-104d-40f3-873e-958a32d7def2" />


## Result:
The program was successfully executed.
It accepts a list of elements and a key to be searched, and displays whether the key is Found or Not Found.
