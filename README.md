# Letter Triangle Pattern in C++

A beginner-friendly C++ program that demonstrates pattern printing using nested loops.

This project generates a **Letter Triangle Pattern**, where each row prints consecutive uppercase alphabets starting from **A**. It is a popular pattern-printing problem from Striver's A2Z DSA Sheet and helps strengthen understanding of nested loops, character manipulation, and ASCII values.

---

## 📌 Features

* Prints a Letter Triangle Pattern
* Uses nested `for` loops
* Demonstrates character iteration using ASCII values
* Beginner-friendly implementation
* Helps improve logical thinking and pattern recognition

---

## 🛠️ Technologies Used

* C++
* Standard Input/Output (`iostream`)

---

## 📂 Problem Statement

Given an integer `N`, print a triangle pattern where each row contains consecutive uppercase letters starting from **A**.

### Example

For:

```txt
N = 5
```

Output:

```txt
A
A B
A B C
A B C D
A B C D E
```

---

## 📸 Screenshot

<img width="1207" height="785" alt="Screenshot 2026-06-30 145900" src="https://github.com/user-attachments/assets/31ff40d6-e3c8-4172-8f1e-437bc0dd8500" />

Example folder structure:

```txt
project-folder/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
```

---

## 💻 Source Code

```cpp
void nLetterTriangle(int n) {
    for (int i = 0; i < n; i++) {
        for (char ch = 'A'; ch <= 'A' + i; ch++) {
            cout << ch << " ";
        }
        cout << endl;
    }
}
```

---

## ▶️ How to Run

1. Compile the program:

```bash
g++ main.cpp -o main
```

2. Run the executable:

```bash
./main
```

3. Enter the value of `N`.

---

## 📸 Example Output

### Input

```txt
4
```

### Output

```txt
A
A B
A B C
A B C D
```

---

## 📖 Learning Concepts

This project helps beginners understand:

* Nested loops
* Pattern printing
* Character data type (`char`)
* ASCII value manipulation
* Loop control statements
* Algorithmic thinking

---

## 🔍 Pattern Explanation

The pattern is created using two nested loops.

### Outer Loop

Controls the number of rows.

```cpp
for (int i = 0; i < n; i++)
```

### Inner Loop

Prints characters from **A** up to the current row's character.

```cpp
for (char ch = 'A'; ch <= 'A' + i; ch++)
```

For each row, one additional letter is printed, resulting in a growing alphabetical triangle.

---

## ⏱️ Complexity Analysis

### Time Complexity

```txt
O(N²)
```

The nested loops perform approximately **N²** iterations.

### Space Complexity

```txt
O(1)
```

The program uses only loop variables and does not require additional memory.

---

## 👨‍💻 Author

Developed as a beginner-friendly C++ practice project for learning nested loops, character manipulation, and pattern printing.
