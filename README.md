# PYTHON PROGRAMMMINDG MODULE 5

### NAME : SANGAMITHRA B
### REGISTER NUMBER : 212224060035

# List Comprehension:Generates all even numbers between 200 and 300
## AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

##  ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

##  PROGRAM:
```
class Program:
    def __init__(self, first,d,last):
        self.first = first
        self.d = d
        self.last=last
    def display(self):
        L=[i for i in range(self.first,self.last+1,self.d)]
        return L


a=int(input())
b=int(input())
c=int(input())
Series = Program(a,b,c+1)
print(Series.display())
```

## OUTPUT:
<img width="129" height="145" alt="image" src="https://github.com/user-attachments/assets/086768d2-20e1-42f8-ad33-a159860e2132" />
<img width="1802" height="113" alt="image" src="https://github.com/user-attachments/assets/65fb5af2-0485-47fc-9505-8f30b9bab09b" />
<img width="1900" height="136" alt="image" src="https://github.com/user-attachments/assets/5cb38b48-067f-48b5-9105-57e621b5bcbc" />

## RESULT:
Thus,the program is executed successfully

# List Comprehension:Transpose of Matrix 

##  AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

##  ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

##  PROGRAM:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M 
    
r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
B=create_matrix(r,c)
print(A)
print(B)
T = [[A[i][j] + B[i][j] for j in range(len(A[0]))] for i in range(len(A))]
print(T)
```

## OUTPUT:
<img width="956" height="827" alt="image" src="https://github.com/user-attachments/assets/e56900d5-175e-4d7f-9b3c-d66179b3ce17" />

## RESULT:
Thus,the program is executed successfully
# Matrix Operations-Diagonal Matrix Elements Printer 

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## Aim

To write a Python program that prints only the diagonal elements of a given matrix.

##  Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

##  Program
```
rows = int(input())
columns = int(input())
matrix = [[0]*columns for row in range(rows)]
for i in range(rows):
    lines = list(map(int, input().split()))
    for j in range(columns):
        matrix[i][j] = lines[j]
print(matrix)
for i in range(rows):
    for j in range(columns):
        if(i==j):
            print(matrix[i][j],end=" ")
        else:
            print(' ',end=" ")
    print()
```

### Output:
<img width="679" height="390" alt="image" src="https://github.com/user-attachments/assets/e6c6fd97-0ed8-4b3c-aab2-7c8d36530bc5" />

## Result
Thus,the program is executed successfully

# #  Matrix Operations-Matrix Subtraction in Python

##  AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

##  ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

##  PROGRAM:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M 
    
def subtract(A,B):
    C=[]
    for i in range(len(A)):
        R=[]
        for j in range(len(A[0])):
            item=A[i][j]-B[i][j]
            R.append(item)
        C.append(R)
    return C
def add(A,B):
    C=[]
    for i in range(len(A)):
        R=[]
        for j in range(len(A[0])):
            item=A[i][j]+B[i][j]
            R.append(item)
        C.append(R)
    return C
r,c=input().split()
A=create_matrix(int(r),int(c))
B=create_matrix(int(r),int(c))
choice= input("Press ADD/SUBTRACT:")
print()
if choice=='ADD':
    C=add(A,B)
elif choice=='SUBTRACT':
    C=subtract(A,B)
else:
    print("Invalid CHoice")
print('A=',A)
print('B=',B)
print('Resultant Matrix:',C)
```

## OUTPUT:
<img width="1117" height="695" alt="image" src="https://github.com/user-attachments/assets/2f2d929d-97a8-4795-9028-72d5624a714b" />

## RESULT:
Thus,the program is executed successfully


#  SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

##  Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

##  Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

##  PROGRAM:
```
class Numbers:
    def __init__(self, N=0):
        self.N = int(input())
    def create_list(self):
        self.L=[]
        for i in range(self.N):
            x=int(input())
            self.L.append(x)
    def sorting(self):
        for i in range(1,len(self.L)):
            key=self.L[i]
            j=i-1
            while j>=0 and key < self.L[j]:
                self.L[j+1]=self.L[j]
                j=j-1
            self.L[j+1]=key
    def print_List(self):
        for i in range(self.N):
            print(self.L[i])
L1=Numbers()
L1. create_list()
print('Before Sorting')
L1.print_List()
L1.sorting()
print('After Sorting')
L1.print_List()
```
## OUTPUT:
<img width="455" height="576" alt="image" src="https://github.com/user-attachments/assets/04c0c242-00b0-4299-8e6f-dd6ed93ab233" />

## RESULT:
Thus,the program is executed successfully




