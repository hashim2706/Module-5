# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
Write python code to create a class Triangle and initialiaze the attributes(base and height) using default constructor and calculate the area of the triangle using user defined function.

---

### ALGORITHM

1. **Create a Class:**
   - Define a class named `Triangle`.

2. **Initialize Attributes:**
   - In the default constructor (`__init__` method), initialize two attributes:
     - `base` set to 0
     - `height` set to 0

3. **Define User-Defined Functions:**
   - `set_dimensions(base, height)`:
     - Takes two parameters: `base` and `height`.
     - Assigns them to the class attributes.
   - `calculate_area()`:
     - Calculates the area of the triangle using the formula:
       \[
       \text{Area} = \frac{1}{2} \times \text{base} \times \text{height}
       \]
     - Returns the calculated area.

4. **Input from User:**
   - Create an object of the `Triangle` class.
   - Take input from the user for `base` and `height`.

5. **Set Values and Calculate Area:**
   - Use the `set_dimensions` method to assign user input values.
   - Call the `calculate_area` method to compute and display the area.


---

### PROGRAM

```
class triangle:
    def __init__(self,base,height):
        self.base=base
        self.height=height
    def cal(self):
        self.area=self.base*self.height*.5
    def display(self):
        print(f"Area of triangle: {self.area}")
n1=int(input())
n2=int(input())
obj=triangle(n1,n2)
obj.cal()
obj.display()

```

### OUTPUT

![Screenshot (203)](https://github.com/user-attachments/assets/5504940b-6d10-4224-970f-57875bcc7b0b)

### RESULT
Thus the program to create a class Triangle and initialiaze the attributes(base and height) using default constructor and calculate the area of the triangle using user defined function is implemented amd executed successfully.
