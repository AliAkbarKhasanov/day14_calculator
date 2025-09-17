# 🧮 Calculator (Day 14)

A simple calculator app written in Python.  
It supports basic operations: **addition, subtraction, multiplication, and division**.

---

## 📌 Features
- Add two numbers ➕  
- Subtract two numbers ➖  
- Multiply two numbers ✖️  
- Divide two numbers ➗ (with zero check)  
- Quit option (`q`) to exit the program  

---

## ▶️ Example run
===== CALCULATOR =====
Choose operation: +, -, *, / or q to quit
Enter operation: +
Enter first number: 10
Enter second number: 5
Result: 15.0

python
Copy code

---

## 💻 Code (main part)
```python
while True:
    print("\n===== CALCULATOR =====")
    print("Choose operation: +, -, *, / or q to quit")

    op = input("Enter operation: ")

    if op == "q":
        print("Goodbye!")
        break

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if op == "+":
        print("Result:", num1 + num2)
    elif op == "-":
        print("Result:", num1 - num2)
    elif op == "*":
        print("Result:", num1 * num2)
    elif op == "/":
        if num2 != 0:
            print("Result:", num1 / num2)
        else:
            print("Error: division by zero!")
    else:
        print("Invalid operation. Try again.")
✨ This project is part of my Python learning journey (Day 14).
