# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

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


