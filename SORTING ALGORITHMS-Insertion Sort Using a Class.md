# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:

    class InsertionSorter:
        def __init__(self):
            self.nums = []

        def create_list(self, n):
            self.nums = [int(input()) for _ in range(n)]

        def insertion_sort(self):
            for i in range(1, len(self.nums)):
                key = self.nums[i]
                j = i - 1
                while j >= 0 and key < self.nums[j]:
                    self.nums[j + 1] = self.nums[j]
                    j -= 1
                self.nums[j + 1] = key

        def print_list(self):
            for num in self.nums:
                print(num)

    sorter = InsertionSorter()
    n = int(input())
    sorter.create_list(n)

    print("Before Sorting")
    sorter.print_list()

    sorter.insertion_sort()

    print("After Sorting")
    sorter.print_list()

## OUTPUT:
<img width="1139" height="647" alt="image" src="https://github.com/user-attachments/assets/d56a0ab9-8ec2-4d0f-adbb-c1d39dd2e62a" />

## RESULT:
Thus the program executed successfully .
