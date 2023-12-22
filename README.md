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
Developed by: Sanjay sivaramkrishnan M
RegisterNumber: 23013798
'''
def selection_sort(array):
     for i in range (len(array)-1):
          current =i
          for  j in range(i+1,len(array)):
                  if(array[j]<array[current]):
                       current=j
          array[i],array[current]=array[current],array[i]
     return array      
    
list_of_nums = eval(input())
x=selection_sort(list_of_nums)
print(x)




```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: Sanjay sivaraamkrishnan M
RegisterNumber: 23013798
'''
def insertion_sort(a):
    for i in range(1,len(a)):
        j=i
        while a[j-1]>a[j] and j>0:
            a[j],a[j-1]=a[j-1],a[j]
            j-=1
    return a        
    
    
list_of_nums = eval(input())
x=insertion_sort(list_of_nums)
print(x)





```

## Output:
![image](https://github.com/sanjaysivaramakrishnan/Sorting-Algorithm/assets/151629616/00d2326b-48b6-451c-9809-4a72369d86d0)
![image](https://github.com/sanjaysivaramakrishnan/Sorting-Algorithm/assets/151629616/54c636b5-8ac1-4f75-b1e6-8c4e3d0829df)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
