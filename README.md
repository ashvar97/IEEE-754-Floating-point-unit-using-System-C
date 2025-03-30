# IEEE 754 Floating-Point Unit using SystemC

## Overview
This project presents a **SystemC-based implementation** of an **IEEE 754 compliant Floating-Point Unit (FPU)**. The FPU supports fundamental arithmetic operations—**addition, subtraction, multiplication, and division**—for both **single-precision (32-bit)** floating-point numbers. Designed for hardware-accurate simulations, this module facilitates the integration and verification of floating-point arithmetic in digital systems.

## Features
- **Arithmetic Operations**: Supports **addition**, **subtraction**, **multiplication**, and **division** operations.
- **IEEE 754 Compliance**: Adheres to the IEEE 754 standard for binary floating-point arithmetic.
- **Precision Support**: Implements both **single-precision (32-bit)** and **double-precision (64-bit)** formats.
- **Exception Handling**: Detects and manages conditions such as **overflow**, **underflow**, **division by zero**, and **invalid operations**.
- **Rounding Modes**: Incorporates multiple rounding modes, including **nearest-even**, **toward zero**, **toward positive infinity**, and **toward negative infinity**.

## Repository Structure

Copy
├── .DS_Store                     # macOS directory metadata (auto-generated, ignore)
├── .gitattributes                # Git configuration for line endings and file types
├── Addition_Final.cpp            # Core 32-bit floating-point addition implementation
├── Addition_check.cpp            # Verification testbench for addition operation
├── Division_Final.cpp            # IEEE 754 compliant division implementation  
├── Division_check.cpp            # Division unit test with edge cases  
├── Multiplication_Final.cpp      # Floating-point multiplier with rounding support  
├── Multiplication_check.cpp      # Multiplier validation with exhaustive tests  
├── Subtract_Final.cpp            # Accurate floating-point subtraction module  
├── Verilog/                      # Optional RTL implementations (VHDL available)  
└── README.md                     # Project documentation and usage guide  
Key features:

## Compilation & Usage

1. Install SystemC dependencies:  
   ```bash
   sudo apt install systemc-dev  # Ubuntu/Debian

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

**Author**: Ashwin Varkey  
**Contact**: [ashvar97@gmail.com](mailto:ashvar97@gmail.com) | [LinkedIn](https://www.linkedin.com/in/ashvar97/)

*Note: This project is intended for educational purposes and may require further validation for deployment in production environments.*
