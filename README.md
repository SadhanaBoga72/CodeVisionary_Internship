#CodeVisionary_Internship
#Calculator_using_Python

def add(a,b):
  return a+b
def subtract(a,b):
  return a-b
def multiply(a,b):
  return a*b
def divide(a,b):
  if b==0:
    return "Error! Can't divide."
  else:
    return a/b
def remainder(a,b):
  return a%b

while True:
  try:
    num1=float(input("Enter the first digit - "))
    operator=input("Enter the choice of operator (+,-,*,/,%) or 'q' to quit - ")

    if operator.lower() == 'q':
      print("Calculator exiting.BYE!")
      break

    num2=float(input("Enter the second digit - "))

    if operator == '+':
      print(f"Result:{add(num1,num2)}")
    elif operator == '-':
      print(f"Result:{subtract(num1,num2)}")
    elif operator == '*':
      print(f"Result:{multiply(num1,num2)}")
    elif operator == '/':
      print(f"Result:{divide(num1,num2)}")
    elif operator == '%':
      print(f"Result:{remainder(num1,num2)}")
    else:
      print("Invalid operation!")

   except ValueError:
  print("Invalid input! Enter a valid number.")
  
