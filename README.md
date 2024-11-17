# PYTHON-ASSIGNMENT
# Python script to check a variable's data type

# Prompt the user for input
user_input = input("Please enter a value: ")

# Check the type of the input
# Since input() returns a string, we convert it to an integer if possible
try:
    # Attempt to convert the input to an integer
    user_input = int(user_input)
    print(f"The data type of the entered value is: {type(user_input)}")
except ValueError:
    try:
        # Attempt to convert the input to a float
        user_input = float(user_input)
        print(f"The data type of the entered value is: {type(user_input)}")
    except ValueError:
        # If it can't be converted to int or float, it's a string
        print(f"The data type of the entered value is: {type(user_input)}")
