# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
      class cse:
          def mech(self,radius):
              self.radius = radius
              self.area = 3.14*self.radius*self.radius
              print(f"Area of the circle is {self.area:.2f}")
      radius = int(input("Enter the radius of th circle :"))
      area_circle = cse()
      area_circle.mech(radius)


## Output
<img width="1918" height="547" alt="image" src="https://github.com/user-attachments/assets/58b83267-d953-4b8c-ab29-ec4e1824efc0" />


## Result
Thus, The Python program that calculates the area of a circle based on the radius provided by the user was executed successfully.
