NAME: MANUGUNTA INDU PRIYA
COMPANY: CODTECHIT SOLUTIONS
ID: CT6WDS523
DURATION: JUNE TO AUGUST 2024
OVERVIEW OF THE PROJECT
PROJECT: SIMPLE CALCULATOR
FUNCTIONS
General approach followed in coding a calculator using functions: 
Define Functions: For every arithmetic operation (addition, subtraction, multiplication, and division), create a distinct function. 
OPERATIONS: 
Display Operations: Inform the user of the available arithmetic operations.
# Define the main function
def calculator():
    print("Simple Calculator")
    print("Options:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")
    print("5. Exit")

    while True:
        choice = input("Enter choice (1/2/3/4/5): ")

        if choice == '5':
            print("Exiting the calculator. Goodbye!")
            break

        if choice in ['1', '2', '3', '4']:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

            if choice == '1':
                print(f"{num1} + {num2} = {num1 + num2}")
            elif choice == '2':
                print(f"{num1} - {num2} = {num1 - num2}")
            elif choice == '3':
                print(f"{num1} * {num2} = {num1 * num2}")
            elif choice == '4':
                if num2 != 0:
                    print(f"{num1} / {num2} = {num1 / num2}")
                else:
                    print("Error! Division by zero.")

        else:
            print("Invalid input. Please enter a number between 1 and 5.")

# Run the calculator function
calculator()

