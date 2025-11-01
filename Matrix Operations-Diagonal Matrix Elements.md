# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
    def get_matrix(row, col):
        matrix = []
        for i in range(row):
            line = input().split()
            mat = [int(x) for x in line]
            matrix.append(mat)
        return matrix

    def print_diagonal_matrix(mat):
        row = len(mat)
        col = len(mat[0])
        for i in range(row):
            for j in range(col):
                if i == j:
                    print(mat[i][j], end=' ')
                else:
                    print(' ', end=' ')
            print() 


    rows = int(input())
    cols = int(input())

    mat = get_matrix(rows, cols)

    print(mat)
    print_diagonal_matrix(mat)


### Output:
<img width="1135" height="366" alt="image" src="https://github.com/user-attachments/assets/44d3c991-8e52-4961-898f-8e8f374ee15a" />

## Result
Thus the program executed successfully .
