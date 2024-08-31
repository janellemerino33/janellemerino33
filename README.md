def arithmetic_operations(a, b):
    print(f"Operands: a = {a}, b = {b}")
    print("Addition:", a + b)
    print("Subtraction:", a - b)
    print("Multiplication:", a * b)
    print("Division:", a / b)
    
    # Modulus operation is not defined for complex numbers
    if isinstance(a, (int, float)) and isinstance(b, (int, float)):
        print("Modulus:", a % b)
    else:
        print("Modulus: Not defined for complex numbers")
    
    print("Exponentiation:", a ** b)

# Example usage:
print("Integer Operations:")
arithmetic_operations(10, 5)
print()

print("Float Operations:")
arithmetic_operations(10.5, 5.2)
print()

print("Complex Number Operations:")
arithmetic_operations(complex(2, 3), complex(1, 1))
