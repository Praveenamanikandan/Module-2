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
```
n = int(input())

def fact(n):
    if n==1 or n==0:
        return 1
        
    else:
        return n*fact(n-1)
def combination(n,r):
    return fact(n)//(fact(n-r)*fact(r))
for i in range(n):
    print(" "*(n-i-1),end="")
    for j in range(i+1):
        print(combination(i,j),end=" ")
#for j in range((i+1//2)-1,0,-1):
# print(combination(i-1,j-1),end=" ")
    print("")
```
## Output
<img width="564" height="510" alt="image" src="https://github.com/user-attachments/assets/d81e28ba-c504-485f-b63f-0ce5987c6614" />

## Result
The program was exected successfully
