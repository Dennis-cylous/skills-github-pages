import math

def calculate_circle(radius):
    area = math.pi * radius ** 2
    circumference = 2 * math.pi * radius
    return area, circumference

def calculate_rectangle(length, width):
    area = length * width
    perimeter = 2 * (length + width)
    return area, perimeter

def calculate_square(side):
    area = side ** 2
    perimeter = 4 * side
    return area, perimeter

# Input
radius = float(input("Enter the radius of the circle: "))
length = float(input("Enter the length of the rectangle: "))
width = float(input("Enter the width of the rectangle: "))
side = float(input("Enter the side of the square: "))

# Calculations
circle_area, circle_circumference = calculate_circle(radius)
rectangle_area, rectangle_perimeter = calculate_rectangle(length, width)
square_area, square_perimeter = calculate_square(side)

# Output
print(f"Circle: Area = {circle_area}, Circumference = {circle_circumference}")
print(f"Rectangle: Area = {rectangle_area}, Perimeter = {rectangle_perimeter}")
print(f"Square: Area = {square_area}, Perimeter = {square_perimeter}")
