#simple calculator
print("--- Calculator ---")

try:
    num = float(input("Enter number: "))
except ValueError:
    print("Invalid input,Enter a number.")
    num = 0.0

while True:
    print(f"\nTotal: {num}")
    
    # 2. Get the operator or action
    operator = input("Enter operator (+, -, *, /) \nOr 'c' to clear, 'q' to quit: ").strip().lower()

    # Check for exit or clear commands
    if operator == 'q':
        print(f"Total: {num}")
        print("Goodbye!")
        break
    
    elif operator == 'c':
        # Reset the total
        try:
            num = float(input("Enter new starting number: "))
        except ValueError:
            print("Invalid input. Starting at 0.")
            num = 0.0
        continue

    # Validate operator
    if operator not in ['+', '-', '*', '/']:
        print("Invalid operator. Please try again.")
        continue

    # 3. Get the next number
    try:
        next_number = float(input("Enter next number: "))
    except ValueError:
        print("Invalid number. Please try again.")
        continue

    # 4. Apply the operation to the running total
    if operator == '+':
        num += next_number
    elif operator == '-':
        num -= next_number
    elif operator == '*':
        num *= next_number
    elif operator == '/':
        if next_number == 0:
            print("Error: Cannot divide by zero.")
        else:
            num /= next_number