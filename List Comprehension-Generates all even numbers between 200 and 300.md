# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
    class Generate:
        def __init__(self, first,d,last):
            self.first = first
            self.d = d
            self.last=last
        def Ap_generate(self):
            L=[i for i in range(self.first,self.last+1,self.d)]
            return L

    Series = Generate(200,2,301)
    print(Series.Ap_generate())
## OUTPUT:
<img width="1140" height="210" alt="image" src="https://github.com/user-attachments/assets/169506b7-a372-4ec3-83d9-cf1dd7cae180" />
<img width="1167" height="208" alt="image" src="https://github.com/user-attachments/assets/1003cff1-aaf2-4966-bcff-d00ff4bf4459" />
<img width="1150" height="190" alt="image" src="https://github.com/user-attachments/assets/2a108182-5fa6-4fc8-97bd-2ce8e927ea3d" />
<img width="1148" height="197" alt="image" src="https://github.com/user-attachments/assets/16e70158-a5aa-477d-9e1d-6113667ef068" />


## RESULT:
Thus the program executed successfully .
