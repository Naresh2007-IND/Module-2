## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```python
num = int(input("Enter a number: "))

original = num
reverse = 0

while num > 0:
    digit = num % 10
    reverse = reverse * 10 + digit
    num = num // 10

if original == reverse:
    print("Palindrome Number")
else:
    print("Not a Palindrome Number")
```
## Output
<img width="251" height="58" alt="Screenshot 2026-05-29 185719" src="https://github.com/user-attachments/assets/88e5512e-e36b-440e-b95d-d050955c2490" />
<img width="310" height="78" alt="Screenshot 2026-05-29 185709" src="https://github.com/user-attachments/assets/72ab5c1d-dabc-4def-b8ad-972ad677ad94" />

## Result
The code was executed successfully by python
