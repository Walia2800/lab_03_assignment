# lab_03_assignment
# 1 2 3 4 5
## A new line added inside VS code...
class Shape:
    def _init_(self, color):
        self.color = color

    def area(self):
        pass

class Rectangle(Shape):
    def _init_(self, color, length, width):
        super()._init_(color)
        self.length = length
        self.width = width

    def area(self):
        return self.length * self.width

class Circle(Shape):
    def _init_(self, color, radius):
        super()._init_(color)
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius

rect = Rectangle("red", 10, 20)
print("Rectangle area:", rect.area(), " color:", rect.color)

circle = Circle("blue", 5)
print("Circle area:", circle.area(), " color:", circle.color)