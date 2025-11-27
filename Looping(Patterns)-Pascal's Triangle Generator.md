# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:
     C(n, k) = n!/[k!(n-k)!]
5. Print all rows of Pascal’s Triangle.
6. End the program.
---
## 🧪 Program
```
def fact(n):
    f=1
    for i in range(1,n+1):
        f*=i
    return f
    
r=int(input("rows: "))
print()

for n in range(r):
    print(" " * (r - n), end="")
    for k in range(n + 1):
        value = fact(n) // (fact(k) * fact(n - k))
        print(value, end=" ")
    print()
```
## Sample Output
<img width="197" height="203" alt="image" src="https://github.com/user-attachments/assets/7dd65076-e2bb-447d-a9aa-81dd4999977a" />

## Result
Thus, the program is executed successfully.
