# Calculator
This is just a normal menu-driven calculator made using Python. Hope it works for ya!
def add(a, b):
    return a+b 
def subtract(a, b):
    return a-b 
def multiply(a, b):
    return a*b 
def divide(a, b):
    if b == 0: 
        return("No number can be divided by zero") 
    return a / b 
    

while True:
    print("--------MENU--------")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exit")
    
    choice = int(input("Enter your choice"))
    if choice == 5:
        print("Thank you for using this program")
        break
        
    if choice <1 or choice>4: 
        print("Enter from among the options given")
    else:
        num1 = float(input("Enter the first number"))
        num2 = float(input("Enter the second number"))
        
    if choice == 1:
        print("The addition of these numbers is", add(num1, num2))
    if choice == 2:
        print("The subtraction of these numbers is", subtract(num1, num2))
    if choice == 3:
        print("The multiplication of these numbers is", multiply(num1, num2))
    if choice == 4:
        print("The division of these numbers is", divide(num1, num2))
        break
