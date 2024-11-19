# Newton's Method Optimization Visualizer

This repository contains a MATLAB implementation of **Newton's Method** for optimizing a quadratic function. The script visualizes the optimization process by plotting the path taken by the algorithm as it converges to the function's minimum point using the gradient and Hessian matrix.

This code was developed as part of our Optimization course project at IASBS, in collaboration with my groupmate, [Erfan Faridi](https://github.com/erfanfaridii/).

## Features

- **Contour Plot Visualization**: Displays the contour plot of the quadratic function and overlays the optimization path.
- **Newton's Method**: Implements the Newton's method optimization, using the inverse of the Hessian matrix and the gradient for point updates.
- **Convergence Check**: Iterates until the change in the function's value is sufficiently small (below a specified threshold).
- **Detailed Results**: Outputs the number of iterations, the minimum point, and the function value at the minimum.

## Prerequisites

- MATLAB R2016b or later.
- Symbolic Math Toolbox.

## Getting Started

### Clone the Repository
```bash
git clone https://github.com/username/Newton-Method-Optimization-Visualizer.git
cd Newton-Method-Optimization-Visualizer
```

### Run the Script

1. Open `newton_method_visualizer.m` in MATLAB.
2. Run the script.

### Output

- The script will display:
  - The number of iterations taken to reach the minimum.
  - The coordinates of the minimum point.
  - The function value at the minimum.
- A contour plot with the optimization path overlaid.

## Customization

- **Initial Point**: Modify the initial point `x`:
  ```matlab
  x = [-2, 2.5];
  ```

- **Learning Rate**: Adjust the learning rate to control the step size:
  ```matlab
  learningRate = 1;
  ```

- **Tolerance**: Change the stopping criteria for convergence:
  ```matlab
  if (errorAmountx1 < 10e-4 && errorAmountx2 < 10e-4)
  ```

- **Function**: Replace the function `f` with your desired quadratic function:
  ```matlab
  f(x1, x2) = (10 * x1 ^ 2) - (4 * x1 * x2) + (x2 ^ 2);
  ```

## Example Output

The script minimizes the function:

\[
f(x_1, x_2) = 10x_1^2 - 4x_1x_2 + x_2^2
\]

and provides the following results:
- The number of iterations until convergence.
- The coordinates of the minimum point found.
- The function value at the minimum.
- A contour plot visualizing the optimization path.

## Acknowledgments

- MATLAB Documentation: [Symbolic Math Toolbox](https://www.mathworks.com/products/symbolic.html)
- Newton's Method: [Wikipedia](https://en.wikipedia.org/wiki/Newton%27s_method)
