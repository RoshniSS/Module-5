# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
class Student:
    def __init__(self,name):
        self.name = name

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.name)

name=input()
obj = Student(name)
obj.show()

## Output
<img width="1418" height="427" alt="Screenshot 2026-06-01 133834" src="https://github.com/user-attachments/assets/a6a652a8-91fe-4d0b-8547-8390eef26941" />

## Result
Thus, the program successfully used a non-parameterized constructor to display a welcome message with the student's name.
