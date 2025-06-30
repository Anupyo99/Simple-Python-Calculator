# Simple-Python-Calculator
# 🧮 Simple Python Calculator

This is a basic command-line calculator built with Python. It supports addition, subtraction, multiplication, and division.

---

## 🔧 Features
- User input for two numbers
- Menu to select operation
- Division by zero error handling
- Easy to run in any terminal

---

## ▶️ How to Run

1. Make sure Python is installed.
2. Open terminal or VS Code.
3. Run the file:
```bash
python calculator.py

# calculator.py

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    return x / y

print("📱 Simple Python Calculator")
print("Select operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

choice = input("Enter choice (1/2/3/4): ")

try:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == '1':
        print("Result:", add(num1, num2))
    elif choice == '2':
        print("Result:", subtract(num1, num2))
    elif choice == '3':
        print("Result:", multiply(num1, num2))
    elif choice == '4':
        print("Result:", divide(num1, num2))
    else:
        print("Invalid input")
except ValueError:
    print("❌ Please enter valid numbers!")
