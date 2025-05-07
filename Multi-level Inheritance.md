# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Start the Program
2. Define the Parent class:
-Create a constructor __init__ that accepts one parameter: name.
-Initialize instance variable self.name.
-Define a method getName() that returns self.name.
3. Define the Child class inheriting from Parent:
-Create a constructor __init__ that accepts two parameters: name and age.
-Call the Parent class constructor to initialize name.
-Initialize instance variable self.age.
-Define a method getAge() that returns self.age.
4. Define the Grandchild class inheriting from Child:
-Create a constructor __init__ that accepts three parameters: name, age, and id.
-Call the Child class constructor to initialize name and age.
-Initialize instance variable self.id.
-Define a method getid() that returns self.id.
5. Accept user input:
-Read a string input for name.
-Read an integer input for age.
-Read an integer input for id.
6. Create an object gc of class Grandchild using the input values.
7. Display output:
-Call gc.getName() to get the name.
-Call gc.getAge() to get the age.
-Call gc.getid() to get the ID.
-Print all three values in a single line separated by spaces.
8. End the Program

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
   def __init__(self,name,age,id):
     Child.__init__(self,name,age)
     self.id=id
   def getid(self):
     return self.id
name=input()
age=int(input())
id=int(input())
gc = Grandchild(name,age,id)
print(gc.getName(), gc.getAge(), gc.getid())
```

### OUTPUT

![image](https://github.com/user-attachments/assets/d56ab102-e7da-4216-add7-3410d3d4165c)

### RESULT
Thus the Python program to get the name, age, and ID of a person and display them using multilevel inheritance was implemented and executed successfully.
