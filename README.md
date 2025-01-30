# Simple Calculator with C++

A terminal-based simple calculator application designed to perform various arithmetic operations, such as addition, subtraction, multiplication, division, and modulus.

## 🧑‍💻 About the Project

This project was created by **Aaliyah Barakatullah Asura**, a **Biomedical Engineering student of the 2024 batch**, part of the **Newton group**, as a task for the **TLS.

### 🌟 Features:
- Supports the following arithmetic operations:
  - **Addition** (`+`)
  - **Subtraction** (`-`)
  - **Multiplication** (`*`)
  - **Division** (`/`)
  - **Modulus** (`%`)
- User-friendly input through a terminal interface.
- Displays operation results directly.

## 🚀 How to Run

### Prerequisites:
- A **C++ compiler** (e.g., GCC).
- Code editor or IDE (e.g., Visual Studio Code, Code::Blocks, or your preferred editor).

### Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/username/simple-calculator.git
   ```
2. Navigate to the project directory:
   ```bash
   cd simple-calculator
   ```
3. Compile the program:
   ```bash
   g++ -o calculator calculator.cpp
   ```
4. Run the program:
   ```bash
   ./calculator
   ```
   
## 📄 Code Structure

The program uses:
1. **Variable declarations** to store input and results.
2. A **switch-case** structure to select arithmetic operations.
3. **Input validation** to ensure the program runs without errors.

### Sample Code:
```cpp
#include <iostream>
#include <string>

using namespace std;

int main()
{
    int bil1, bil2, pil;
    float hasil;
    string operasi;

    cout << "SELECT AN ARITHMETIC OPERATOR" << endl;
    cout << "1. Addition" << endl;
    cout << "2. Subtraction" << endl;
    cout << "3. Multiplication" << endl;
    cout << "4. Division" << endl;
    cout << "5. Modulus" << endl;
    cout << "Enter your choice: ";
    cin >> pil;

    cout << "Enter the first number: ";
    cin >> bil1;
    cout << "Enter the second number: ";
    cin >> bil2;

    switch (pil)
    {
        case 1:
            hasil = bil1 + bil2;
            operasi = '+';
            break;
        case 2:
            hasil = bil1 - bil2;
            operasi = '-';
            break;
        case 3:
            hasil = bil1 * bil2;
            operasi = '*';
            break;
        case 4:
            hasil = bil1 / bil2;
            operasi = '/';
            break;
        case 5:
            hasil = bil1 % bil2;
            operasi = '%';
            break;
        default:
            cout << "Invalid operator selected" << endl;
    }

    cout << "----------------------------------" << endl;
    cout << " " << bil1 << operasi << bil2 << " = " << hasil << endl;
}
```

## 📊 Example Output

Here’s an example of how the program works in the terminal:

```
SELECT AN ARITHMETIC OPERATOR
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Modulus
Enter your choice: 1
Enter the first number: 10
Enter the second number: 5
----------------------------------
 10+5 = 15
```

## ✨ Author

- **Name:** Aaliyah Barakatullah Asura  
- **Program:** Biomedical Engineering 
- **Group:** Newton
- **University:** Universitas Gadjah Mada
