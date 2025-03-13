# Square Root of a Number 📐

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A Python implementation of the bisection method for calculating square roots of non-negative numbers.

## 📜 About
This project demonstrates a numerical approach to finding square roots using the bisection method. It's an educational tool for understanding iterative numerical methods and root-finding algorithms.

## ✨ Features
- Calculates square roots for non-negative real numbers
- Uses the bisection method for efficient convergence
- Customizable tolerance and maximum iterations
- Handles edge cases (0 and 1) efficiently
- Clear output formatting

## 🚀 Quick Start

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/fahadelahikhan/Square-Root-of-a-Number.git
   cd Square-Root-of-a-Number
   ```

2. Run the application:
   ```bash
   python "Square Root of a Number.py"
   ```

### Basic Usage
```python
# Import the square root function
from square_root import square_root_bisection

# Calculate square root of 25
result = square_root_bisection(25)
# Output: The square root of 25 is approximately 5.0

# Calculate square root of 2 with custom tolerance
result = square_root_bisection(2, tolerance=1e-10)
# Output: The square root of 2 is approximately 1.4142135623730951
```

### Example Calculation
```python
# Calculate square root of 16
square_root_bisection(16)
# Output: The square root of 16 is approximately 4.0

# Calculate square root of 50 with custom iterations
square_root_bisection(50, max_iterations=200)
# Output: The square root of 50 is approximately 7.0710678118654755
```

## 📖 How It Works
The bisection method works by:
1. Establishing an interval [low, high] that contains the square root
2. Repeatedly dividing the interval in half
3. Checking if the midpoint squared is close enough to the target value
4. Adjusting the interval based on whether the midpoint is too high or too low
5. Continuing until the desired tolerance is achieved or maximum iterations are reached

The algorithm uses the property that for a continuous function f(x) = x² - target, if f(low) < 0 and f(high) > 0, then there must be a root between low and high.

## ⚖️ License
Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

> **Note**: This implementation is for educational purposes and demonstrates basic numerical methods. For production use, consider using optimized mathematical libraries like NumPy.
