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
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```python
import math

rows = int(input("Enter number of rows: "))

for n in range(rows):

    # Print spaces
    for space in range(rows - n - 1):
        print(" ", end="")

    # Print values
    for k in range(n + 1):

        value = math.factorial(n) // (
            math.factorial(k) * math.factorial(n - k)
        )

        print(value, end=" ")

    print()
```

## Sample Output
<img width="451" height="202" alt="Screenshot 2026-05-29 185458" src="https://github.com/user-attachments/assets/39562f37-6471-4a8a-a19e-070151c457af" />

## Result
The code was successfully executed  by using python 
