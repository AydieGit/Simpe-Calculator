print("Simple Calculator")

def add(num1, num2):
  return num1 + num2
def subtrack(num1, num2):
  return num1 - num2
def multiply(num1, num2):
  return num1 * num2
def devide(num1, num2):
  return num1 / num2
#dict of possible functions
operations = {
  "+": add,
  "-":subtrack,
  "*":multiply,
  "/":devide
}


def calculator():
  num1 = float(input("Type first number: "))
  game_status = True
  for operation in operations:
    print(operation)
  while game_status:
    choose_symbol = input("Please choose operation: ")
    num2 = float(input("Type next number: "))
    choose_operation = operations[choose_symbol]
    answer = choose_operation(num1, num2)
    print(f"{num1} {choose_symbol} {num2} = {answer}")
  
    if input(f"Do you wanna continue with this number {answer} ?") == "yes":
      num1 = answer
      
    else:
      game_status = False
      calculator()

calculator()
