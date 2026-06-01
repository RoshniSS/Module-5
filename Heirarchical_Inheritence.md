# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details:
    def getName(self, name):
        self.name = name

    def getAge(self, age):
        self.age = age


class Employee(Details):
    def getEmployeeDetails(self, emp_id, department):
        self.emp_id = emp_id
        self.department = department

    def display(self):
        print("Employee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.emp_id)
        print("Department:", self.department)


class Patient(Details):
    def getPatientDetails(self, patient_id, disease):
        self.patient_id = patient_id
        self.disease = disease

    def display(self):
        print("Patient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


e = Employee()
e.getName(input("Enter Employee Name: "))
e.getAge(input("Enter Employee Age: "))
e.getEmployeeDetails(input("Enter Employee ID: "), input("Enter Department: "))

p = Patient()
p.getName(input("Enter Patient Name: "))
p.getAge(input("Enter Patient Age: "))
p.getPatientDetails(input("Enter Patient ID: "), input("Enter Disease: "))

e.display()
p.display()
## Sample Output
<img width="1647" height="900" alt="Screenshot 2026-06-01 134628" src="https://github.com/user-attachments/assets/04d6d76c-cfc2-4c79-a074-6c6ccb1f0a27" />

## Result
Thus, the program successfully demonstrated Hierarchical Inheritance using the Employee and Patient classes derived from the Details class.

