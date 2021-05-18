# Quadratic-Equation-Solver
# This program provides the roots for a quadratic equation.

def root_one(a, b, c):
    """This function returns the first root of a quadratic equation."""
    return (-b + (b ** 2 - (4 * a * c)) ** 0.5) / (2 * a)


def root_two(a, b, c):
    """This function returns the second root of a quadratic equation."""
    return (-b - (b ** 2 - (4 * a * c)) ** 0.5) / (2 * a)


a = int(input("Insert the 'a' value: "))
b = int(input("Insert the 'b' value: "))
c = int(input("Insert the 'c' value: "))
print()

if (b ** 2 - 4 * a * c) == 0:
    print("Both roots of the equation are equal to", root_one(a, b, c))
else:
    print("Root one = ", root_one(a, b, c))
    print()
    print("Root two = ", root_two(a, b, c))
