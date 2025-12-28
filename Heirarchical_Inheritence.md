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
# Base class

class Details:

    def getDetails(self):
        
        self.name = input("Enter name: ")
        
        self.age = int(input("Enter age: "))



class Employee(Details):

    def showEmployee(self):
    
        self.getDetails()
        
        self.emp_id = input("Enter employee id: ")
        
        self.dept = input("Enter department: ")

        
        print("\nEmployee Details")
        
        print(self.name, self.age, self.emp_id, self.dept)




class Patient(Details):

    def showPatient(self):
    
        self.getDetails()
        
        self.pat_id = input("Enter patient id: ")
        
        self.disease = input("Enter disease: ")

        
        print("\nPatient Details")
        
        print(self.name, self.age, self.pat_id, self.disease)


e = Employee()

e.showEmployee()

p = Patient()

p.showPatient()


## Sample Output
<img width="581" height="396" alt="image" src="https://github.com/user-attachments/assets/678b05e6-e343-478d-b296-af1f06740a57" />

## Result
Thus the program executed successfully.
