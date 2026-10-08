# week8
toolkit_plan.txt
PLP Python Week 8 Toolkit Plan

Tool 1: Simple Calculator
The calculator performs addition, subtraction, multiplication, and division.

Tool 2: To-Do List
The to-do list allows the user to add, remove, and view tasks.

Tool 3: Number Checker
The number checker asks for several numbers and identifies whether each number is even or odd.

Menu Text:
Welcome to My Python Toolkit!
Please choose a tool:
1. Simple Calculator
2. To-Do List
3. Number Checker
4. Quit
Enter your choice:

Concepts Used:

Simple Calculator:
- Input
- Variables
- Conditionals
- F-strings

To-Do List:
- List
- Loop
- Append
- Remove
- Conditionals
- F-strings

Number Checker:
- For loop
- Conditional
- Modulo operator
- F-strings
- print("Welcome to My Python Toolkit!")

while True:
    print("\nPlease choose a tool:")
    print("1. Simple Calculator")
    print("2. To-Do List")
    print("3. Number Checker")
    print("4. Quit")

    choice = input("Enter your choice: ")

    if choice == "1":
        print("You selected Simple Calculator.")

    elif choice == "2":
        print("You selected To-Do List.")

    elif choice == "3":
        print("You selected Number Checker.")

    elif choice == "4":
        print("Thank you for using My Python Toolkit. Goodbye!")
        break

    else:
        print("Sorry, that is not a valid choice. Please try again.")
        Welcome to My Python Toolkit!

Please choose a tool:
1. Simple Calculator
2. To-Do List
3. Number Checker
4. Quit
Enter your choice: 9
Sorry, that is not a valid choice. Please try again.
if choice == "1":
    print("You selected Simple Calculator.")
   if choice == "1":
    # Simple Calculator performs basic mathematical operations.
    num1 = float(input("Enter the first number: "))
    operator = input("Enter +, -, *, or /: ")
    num2 = float(input("Enter the second number: "))

    if operator == "+":
        result = num1 + num2
    elif operator == "-":
        result = num1 - num2
    elif operator == "*":
        result = num1 * num2
    elif operator == "/":
        if num2 != 0:
            result = num1 / num2
        else:
            result = "Cannot divide by zero"
    else:
        result = "Invalid operator"

    print(f"Result: {result}")
   tasks = []
   elif choice == "2":
    print("You selected To-Do List.")
   elif choice == "2":
    # To-Do List allows the user to add, remove, and view tasks.
    while True:
        print("\nTo-Do List")
        print("1. Add task")
        print("2. Remove task")
        print("3. Show tasks")
        print("4. Back to main menu")

        task_choice = input("Choose an option: ")

        if task_choice == "1":
            task = input("Enter a task: ")
            tasks.append(task)
            print(f"Task '{task}' was added.")

        elif task_choice == "2":
            task = input("Enter the task to remove: ")

            if task in tasks:
                tasks.remove(task)
                print(f"Task '{task}' was removed.")
            else:
                print(f"Task '{task}' was not found.")

        elif task_choice == "3":
            if len(tasks) == 0:
                print("Your to-do list is empty.")
            else:
                print("Your tasks:")
                for task in tasks:
                    print(f"- {task}")

        elif task_choice == "4":
            print("Returning to the main menu.")
            break

        else:
            print("Please choose a valid option.")
   elif choice == "3":
    print("You selected Number Checker.")
   print("Welcome to My Python Toolkit!")

tasks = []

while True:
    print("\nPlease choose a tool:")
    print("1. Simple Calculator")
    print("2. To-Do List")
    print("3. Number Checker")
    print("4. Quit")

    choice = input("Enter your choice: ")

    if choice == "1":
        # Simple Calculator performs basic mathematical operations.
        num1 = float(input("Enter the first number: "))
        operator = input("Enter +, -, *, or /: ")
        num2 = float(input("Enter the second number: "))

        if operator == "+":
            result = num1 + num2
        elif operator == "-":
            result = num1 - num2
        elif operator == "*":
            result = num1 * num2
        elif operator == "/":
            if num2 != 0:
                result = num1 / num2
            else:
                result = "Cannot divide by zero"
        else:
            result = "Invalid operator"

        print(f"Result: {result}")

    elif choice == "2":
        # To-Do List allows the user to add, remove, and view tasks.
        while True:
            print("\nTo-Do List")
            print("1. Add task")
            print("2. Remove task")
            print("3. Show tasks")
            print("4. Back to main menu")

            task_choice = input("Choose an option: ")

            if task_choice == "1":
                task = input("Enter a task: ")
                tasks.append(task)
                print(f"Task '{task}' was added.")

            elif task_choice == "2":
                task = input("Enter the task to remove: ")

                if task in tasks:
                    tasks.remove(task)
                    print(f"Task '{task}' was removed.")
                else:
                    print(f"Task '{task}' was not found.")

            elif task_choice == "3":
                if len(tasks) == 0:
                    print("Your to-do list is empty.")
                else:
                    print("Your tasks:")
                    for task in tasks:
                        print(f"- {task}")

            elif task_choice == "4":
                print("Returning to the main menu.")
                break

            else:
                print("Please choose a valid option.")

    elif choice == "3":
        # Number Checker checks whether several numbers are even or odd.
        print("Enter five numbers and I will check them.")

        for i in range(5):
            number = int(input(f"Enter number {i + 1}: "))

            if number % 2 == 0:
                print(f"{number} is even.")
            else:
                print(f"{number} is odd.")

    elif choice == "4":
        print("Thank you for using My Python Toolkit. Goodbye!")
        break

    else:
        print("Sorry, that is not a valid choice. Please try again.")
        
