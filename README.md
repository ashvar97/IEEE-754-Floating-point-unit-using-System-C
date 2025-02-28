# IEEE 754 Floating-Point Unit using SystemC

## Overview
This project presents a **SystemC-based implementation** of an **IEEE 754 compliant Floating-Point Unit (FPU)**. The FPU supports fundamental arithmetic operations—**addition, subtraction, multiplication, and division**—for both **single-precision (32-bit)** and **double-precision (64-bit)** floating-point numbers. Designed for hardware-accurate simulations, this module facilitates the integration and verification of floating-point arithmetic in digital systems.

## Features
- **Arithmetic Operations**: Supports **addition**, **subtraction**, **multiplication**, and **division** operations.
- **IEEE 754 Compliance**: Adheres to the IEEE 754 standard for binary floating-point arithmetic.
- **Precision Support**: Implements both **single-precision (32-bit)** and **double-precision (64-bit)** formats.
- **Exception Handling**: Detects and manages conditions such as **overflow**, **underflow**, **division by zero**, and **invalid operations**.
- **Rounding Modes**: Incorporates multiple rounding modes, including **nearest-even**, **toward zero**, **toward positive infinity**, and **toward negative infinity**.

## Repository Structure
```
📂 IEEE-754-Floating-point-unit-using-System-C
├── Addition_Final.cpp          # Implementation of floating-point addition
├── Addition_check.cpp          # Testbench for floating-point addition
├── Division_Final.cpp          # Implementation of floating-point division
├── Division_check.cpp          # Testbench for floating-point division
├── Multiplication_Final.cpp    # Implementation of floating-point multiplication
├── Multiplication_check.cpp    # Testbench for floating-point multiplication
├── Subtract_Final.cpp          # Implementation of floating-point subtraction
├── README.md                   # Project documentation
└── .gitattributes              # Git attributes configuration
```

## Getting Started
### Prerequisites
- **SystemC Library**: Ensure the SystemC library is installed on your system. Refer to the [Accellera SystemC page](https://www.accellera.org/downloads/standards/systemc) for installation instructions.

### Compilation and Execution
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ashvar97/IEEE-754-Floating-point-unit-using-System-C.git
   cd IEEE-754-Floating-point-unit-using-System-C
   ```

2. **Compile the Modules**:
   - Use a C++ compiler (e.g., `g++`) with SystemC includes and libraries.
   - Example compilation command for addition module and its testbench:
     ```bash
     g++ -I /path/to/systemc/include -L /path/to/systemc/lib-linux Addition_Final.cpp Addition_check.cpp -o fp_addition -lsystemc -lm
     ```
   - Replace `/path/to/systemc/` with the actual SystemC installation path.

3. **Run the Executable**:
   ```bash
   ./fp_addition
   ```
   Repeat the compilation and execution steps for multiplication, division, and subtraction modules by replacing the filenames accordingly.

## Usage
- **Integration**: Incorporate these modules into larger SystemC projects requiring floating-point arithmetic.
- **Verification**: Utilize the provided testbenches (`*_check.cpp`) to verify the correctness of each arithmetic operation.
- **Customization**: Modify the modules to support additional operations or to optimize performance for specific applications.

## Contributing
Contributions are welcome! To contribute:
1. **Fork the Repository**.
2. **Clone Your Fork**:
   ```bash
   git clone https://github.com/your-username/IEEE-754-Floating-point-unit-using-System-C.git
   ```
3. **Create a New Branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Make Your Changes**.
5. **Commit Changes**:
   ```bash
   git commit -am 'Add new feature: your-feature-name'
   ```
6. **Push to Your Fork**:
   ```bash
   git push origin feature/your-feature-name
   ```
7. **Submit a Pull Request**.

For major changes, please open an issue first to discuss your proposed modifications.

## License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.

---
**Author**: Ashwin Varkey  
**Contact**: [ashvar97@gmail.com](mailto:ashvar97@gmail.com) | [LinkedIn](https://www.linkedin.com/in/ashvar97/)

*Note: This project is intended for educational purposes and may require further validation for deployment in production environments.*
