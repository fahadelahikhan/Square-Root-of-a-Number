# Square Root of a Number 🔢

![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A simple Python implementation that calculates the square root of a number using the bisection method. Developed as an educational tool to demonstrate numerical approximation techniques.

## About
This project provides a clear example of the bisection method for approximating square roots. It serves both as a practical tool and a teaching aid in numerical methods.

## Features
- Approximates square roots accurately using the bisection method.
- Handles special cases like 0 and 1 gracefully.
- Configurable tolerance and maximum iteration parameters.
- Provides informative error messages for invalid inputs.
- Easy to integrate into other Python projects.

## Quick Start

### Installation
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/fahadelahikhan/Square-Root-of-a-Number.git
cd Square-Root-of-a-Number
```

### Basic Usage
Use the `square_root_bisection` function in your Python code:
```python
from square_root import square_root_bisection

result = square_root_bisection(16)
print(result)  # Output: Approximately 4.0
```

## Example
Here's a realistic scenario using the function:
```python
# Calculate the square root of 25
N = 25
root = square_root_bisection(N)
print(f"The square root of {N} is {root}")  # Output: The square root of 25 is approximately 5.0
```

## How It Works
The function implements the bisection method:
- **Initialization**: Sets `low` to 0 and `high` to `max(1, square_target)`.
- **Iteration**: Computes the midpoint and its square.
- **Convergence**: Continues narrowing the interval until the squared midpoint is within a specified tolerance of the target number.
  
This iterative approach demonstrates a fundamental numerical technique in a concise manner.

## License
Distributed under the [MIT License](LICENSE).

> **Note**: This project is provided as-is without any warranty. Use it responsibly and at your own risk.
