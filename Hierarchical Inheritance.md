# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
Write a Python program to Get the employee  and patient details & display it using Hierarchical inheritance.

---

### ALGORITHM

1. **Create a Base Class `Person`:**
   - Define attributes:
     - `name`
     - `age`
   - Create a method `display_details()` to display the name and age.

2. **Create Derived Class `Employee`:**
   - Inherits from `Person`.
   - Adds attributes:
     - `employee_id`
     - `department`
   - Override `display_details()` to display employee-specific information along with inherited details.

3. **Create Derived Class `Patient`:**
   - Inherits from `Person`.
   - Adds attributes:
     - `patient_id`
     - `disease`
   - Override `display_details()` to display patient-specific information along with inherited details.

4. **Input Details:**
   - Prompt the user to input employee's name, age, ID, and department.
   - Prompt the user to input patient's name, age, ID, and disease.

5. **Create Objects:**
   - Create an `Employee` object using the entered employee details.
   - Create a `Patient` object using the entered patient details.

6. **Display Details:**
   - Call `display_details()` on each object to show all stored information.



---

### PROGRAM
```
class Details:
    def __init__(self):
        self.__id="<No Id>"
        self.__name="<No Name>"
        self.__gender="<No Gender>"
    def setData(self,id,name,gender):
        self.__id=id
        self.__name=name
        self.__gender=gender
    def showData(self):
        print("Id: ",self.__id)
        print("Name: ", self.__name)
        print("Gender: ", self.__gender)

class Employee(Details): #Inheritance
    def __init__(self):
        self.__company="<No Company>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,comp,dept):
        self.setData(id,name,gender)
        self.__company=comp
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Company: ", self.__company)
        print("Department: ", self.__dept)

class Patient(Details): #Inheritance
    def __init__(self):
        self.__hospital="<No Hospital>"
        self.__dept="<No Dept>"
    def setEmployee(self,id,name,gender,hos,dept):
        self.setData(id,name,gender)
        self.__hospital=hos
        self.__dept=dept
    def showEmployee(self):
        self.showData()
        print("Hospital: ", self.__hospital)
        print("Department: ", self.__dept)

id=int(input())
name=input()
gender=input()
comp=input()
dept=input()
id1=int(input())
nam=input()
gen=input()
hosp=input()
dep=input()

print("Employee Object")
e=Employee()
e.setEmployee(id,name,gender,comp,dept)
e.showEmployee()
print("\nPatient Object")
d = Patient()
d.setEmployee(id1, nam, gen, hosp, dep)
d.showEmployee()


```

### OUTPUT  

![Screenshot (205)](https://github.com/user-attachments/assets/ce6f8ef3-2e0d-4b01-96fa-78ea0f57801d)



### RESULT
Thus, the program to Get the employee  and patient details & display it using Hierarchical inheritance is implemented and executed successfully.

