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
Add code here
class Details:
   
    def __init__(self, name, age):
        self.name = name
        self.age = age

class Employee(Details):
    
    def __init__(self, name, age, emp_id):
        super().__init__(name, age)
        self.emp_id = emp_id

    def show_employee(self):
        print("Employee:", self.name, self.age, self.emp_id)

class Patient(Details):
    
    def __init__(self, name, age, disease):
        super().__init__(name, age)
        self.disease = disease

    def show_patient(self):
        print("Patient:", self.name, self.age, self.disease)

# Input
ename = input()

eage = int(input())

eid = input()

pname = input()

page = int(input())

disease = input()

# Objects
e = Employee(ename, eage, eid)

p = Patient(pname, page, disease)
## Sample Output
<img width="375" height="347" alt="image" src="https://github.com/user-attachments/assets/9e065e52-e676-494d-a7b7-71a593de1f0b" />

