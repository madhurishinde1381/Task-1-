**TASK 1 PYTHON DEVELOPER**

Task 1: Build a Calculator CLI App

Objective: Create a command-line calculator supporting basic operations (+, -, *, /).

Deliverable: Python script (calculator.py).
Implemented Python Code (calculator.py):


def add(a, b):
 return a + b
def subtract(a, b):
 return a - b
def multiply(a, b):
 return a * b
def divide(a, b):
 if b == 0:
 return "Error! Division by zero."
 return a / b
def calculator():
 while True:
 print("\n--- Simple CLI Calculator ---")
 print("1. Add")
 print("2. Subtract")
 print("3. Multiply")
 print("4. Divide")
 print("5. Exit")
 choice = input("Enter choice (1-5): ")
 if choice == "5":
 print("Exiting... Goodbye!")
 break
 if choice in ["1", "2", "3", "4"]:
 try:
 num1 = float(input("Enter first number: "))
 num2 = float(input("Enter second number: "))
 except ValueError:
 print("Invalid input! Please enter numbers only.")
 continue
 if choice == "1":
 print(f"Result: {add(num1, num2)}")
 elif choice == "2":
 print(f"Result: {subtract(num1, num2)}")
 elif choice == "3":
 print(f"Result: {multiply(num1, num2)}")
 elif choice == "4":
 print(f"Result: {divide(num1, num2)}")
 else:
 print("Invalid choice! Please try again.")
if __name__ == "__main__":
 calculator()
