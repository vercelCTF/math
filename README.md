# math
@@ -7,7 +7,6 @@ def add(a, b):
    Adds two numbers.
    """
    return a + b

def subtract(a, b):
    """
    Subtracts the second number from the first.
    """
    return a - b
def multiply(a, b):
    """
    Multiplies two numbers.
    """
    return a * b
def divide(a, b):
    """
    Divides the first number by the second.
    """
    if b == 0:
        raise ValueError("Cannot divide by zero.")
    return a / b
# Advanced Mathematical Functions
def factorial(n):
    """
    Calculates the factorial of a number.
    """
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers.")
    return 1 if n == 0 else n * factorial(n - 1)
def is_prime(n):
    """
    Checks if a number is prime.
    """
    if n <= 1:
        return False
    for i in range(2, int(math.sqrt(n)) + 1):
        if n % i == 0:
            return False
    return True
def fibonacci_sequence(n):
    """
    Generates the first n numbers in the Fibonacci sequence.
    """
    sequence = [0, 1]
    for i in range(2, n):
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]
# Geometry Functions
def area_of_circle(radius):
    """
    Calculates the area of a circle given its radius.
    """
    if radius < 0:
        raise ValueError("Radius cannot be negative.")
    return math.pi * radius ** 2
def area_of_triangle(base, height):
    """
    Calculates the area of a triangle given its base and height.
    """
    return 0.5 * base * height
HIDDEN_TEXT = "a98daeboobo741fb5564"
# Main Execution
if __name__ == "__main__":
    print("Basic Arithmetic:")
    print("5 + 3 =", add(5, 3))
    print("10 - 4 =", subtract(10, 4))
    print("6 * 7 =", multiply(6, 7))
    print("20 / 5 =", divide(20, 5))
    print("\nFactorial and Primality:")
    print("Factorial of 5:", factorial(5))
    print("Is 29 prime?:", is_prime(29))
    print("\nFibonacci Sequence:")
    print("First 10 Fibonacci numbers:", fibonacci_sequence(10))
    print("\nGeometry Calculations:")
    print("Area of a circle with radius 3:", area_of_circle(3))
    print("Area of a triangle with base 5 and height 4:", area_of_triangle(5, 4))
