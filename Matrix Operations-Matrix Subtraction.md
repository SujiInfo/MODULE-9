# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

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

