Exercise:3

Build a simple calculator which can: add, subtract, multiply, divide. Hint: solve by writing a function that takes as argument two numbers and the operation and returns the desired output. Run test for function(2,5,’d’) Output: 0.4

## 🧮 Simple Python Calculator



```python
def calculator(x, y, operation):   ### define calculator for operation
    if operation == 'a':           ### 'a' for add
        return x + y
    elif operation == 's':         ### 's' for subtract
        return x - y
    elif operation == 'm':         ### 'm' for multiply
        return x * y
    elif operation == 'd':         ### 'd' for divide
        if y == 0:                 ### dividing 0 by any number is allowed but any number dividing by 0 is not allowed
            return "Error: divide by zero"
        return x / y
    else:
        return "Invalid operation"
