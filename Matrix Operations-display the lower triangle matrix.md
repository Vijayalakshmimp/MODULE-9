# # ➖ Matrix Operations-display the lower triangle matrix

## 🎯 AIM:
To write a Python program to read a matrix and display the lower triangle Matrix.

---

## 🧠 ALGORITHM:

1. Input n (size of square matrix).
2. Initialize an n × n matrix.
3. For each row, read n integers and store them in the matrix.
4. Print "Matrix:".
5. For each element M[i][j]: If i ≥ j, print M[i][j]. Else, print 0.
6. Move to a new line after each row.

---

## 💻 PROGRAM:
~~~
def read_matrix(n):
    matrix=[[0]*n for row in range(n)]
    for i in range(n):
        lines=list(map(int,input().split()))
        for j in range(n):
            matrix[i][j]=lines[j]
    return matrix
def print_matrix(M):
    print("Matrix:")
    for i in range(len(M)):
        for j in range(len(M[0])):
            if(i>j or i==j):
                print(M[i][j],end=" ")
            else:
                print(0,end=" ")
        print()
~~~

## OUTPUT:
<img width="665" height="413" alt="image" src="https://github.com/user-attachments/assets/eae54260-3fe0-468c-904c-f152f650f5ae" />

## RESULT:
Thus, the program has been executed and verified successfully.
