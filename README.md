# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: D Vergin Jenifer
RegisterNumber: 23004210
'''
def selection_sort(num):
    n=len(num)
    for i in range(n-1):
        min_index=i
        for j in range(i+1,n):
            if num[j]<num[min_index]:
                min_index=j
        num[i],num[min_index]=num[min_index],num[i]
num=eval(input())
selection_sort(num)
print(num)
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: D Vergin Jenifer
RegisterNumber: 23004210
'''
def insertion_sort(num):
    n=len(num)
    for i in range(1,n):
        key=num[i]
        j=i-1
        while j>=0 and key<num[j]:
            num[j+1]=num[j]
            j-=1
.

.
.;
        num[j+1]=key
num=eval(input())
insertion_sort(num)
print(num)
```

## Output:
![image](https://github.com/VerginJenifer/Sorting-Algorithm/assets/136251012/8c669b9e-e56b-407a-8fef-ceb89754b14c)

![image](https://github.com/VerginJenifer/Sorting-Algorithm/assets/136251012/8aebcca2-0818-4139-801f-0f6d9feb264f)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
