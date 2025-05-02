# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```
class student:
    def __init__(self,name):
        print("Inside Constructor")
        print("Object initialized")
        self.name=name
    def display(self):
        print(f"Hello, my name is {self.name}")
    def __del__(self):
        print("Inside destructor")
        print("Object destroyed")
n1=input()
obj=student('Emma')
obj.display()
del obj

```

### OUTPUT

![Screenshot (204)](https://github.com/user-attachments/assets/0a9c0aac-6af8-4f79-b3d8-5ef7a56f65d4)


### RESULT
Thus, the program To create a Python class `Student` with a destructor is implemented amd executed successfully.
