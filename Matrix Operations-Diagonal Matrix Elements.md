# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

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
