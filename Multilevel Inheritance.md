


# Exp.No:23 
## Multi-level Inheritance

---

### AIM  
Write a Python program to Get the name, age and salary of a person and display using Multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `salary`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `salary` to `self.salary`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `salary`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `salary`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.salary`.

5. Prompt the user to enter `name` (string), `age` (integer), and `salary` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `salary` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM

```
class Parent:
   def __init__(self,name):
     self.name = name
   def getName(self):
     return self.name
class Child(Parent):
   def __init__(self,name,age):
     Parent.__init__(self,name)
     self.age = age
   def getAge(self):
     return self.age
class Grandchild(Child):
   def __init__(self,name,age,sal):
     Child.__init__(self,name,age)
     self.sal=sal
   def getsal(self):
     return self.sal
name=input()
age=int(input())
sal=int(input())
gc = Grandchild(name,age,sal)
print(gc.getName(), gc.getAge(), gc.getsal())


```

### OUTPUT

![Screenshot (206)](https://github.com/user-attachments/assets/91aa2e25-ec69-473f-b8ec-045710ad978a)


### RESULT
Thus, the program to Get the name, age and salary of a person and display using Multilevel inheritance was implemented and executed successfully.
