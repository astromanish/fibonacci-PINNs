# Fibonacci-Activated PINNs: Enhancing Physics-Informed Neural Networks

This repository contains the code, results, and documentation for my thesis project, which explores the role of Fibonacci sequence-based activation functions in Physics-Informed Neural Networks (PINNs). The project demonstrates the effectiveness of the proposed activation function compared to traditional ones like tanh and sigmoid across various physics problems.

## Abstract

Physics-Informed Neural Networks (PINNs) have emerged as a powerful tool for solving complex differential equations. This thesis investigates the impact of activation functions on PINN performance, specifically focusing on a novel activation function inspired by the Fibonacci sequence. We compare its performance with traditional tanh and sigmoid functions across five diverse physics problems, showcasing its potential to enhance accuracy and convergence.

## Repository Structure

- `Fibonacci_PINNs.ipynb`: The main Jupyter Notebook containing all code for training and evaluating PINN models.
  - Section 1: Training and evaluation with tanh and sigmoid activations on all five equations.
  - Section 2: Training and evaluation with the proposed Fibonacci-based activation on all five equations.

- `results/` : Generated plot images for each problem and activation function

- `docs/`
  - `thesis.pdf`: Complete thesis report
  - `presentation`: Slides used for thesis defense. Find it here [text](https://www.canva.com/design/DAGHFFvpyUM/9LlI44cvoajoWKCo_3sNxg/edit?utm_content=DAGHFFvpyUM&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
  - `reference papers`: Some of the paper used as references for the project
  - `certificate.pdf`: Completion certificate

- `latex/`
  - `thesis.zip`: LaTeX source code for the thesis document

- `README.md`: This file

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/astromanish/fibonacci-PINNs.git
   cd fibonacci-PINNs
   ```

2. Set up a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

   Typical dependencies might include:
   - tensorflow or pytorch
   - numpy
   - matplotlib
   - deepxde
   - jupyter

## Usage

All code is contained in a single Jupyter Notebook, making it easy to run and experiment with different settings.

1. Start Jupyter Notebook:
   ```
   jupyter notebook
   ```

2. Open `Fibonacci_PINNs.ipynb` in your browser.

3. Run the cells in order:
   - First section: Models with tanh and sigmoid activations
   - Second section: Models with the proposed Fibonacci-based activation

4. Experiment by modifying hyperparameters, network architectures, or even the activation functions themselves.

5. Results (plots) will be saved in the `results/` directory.

## Problems Covered

The notebook addresses five diverse physics problems:

1. 1D Poisson Equation
2. 1D Burgers' Equation
3. Time-Dependent 1D Heat Equation
4. 2D Helmholtz Equation
5. 2D Elastostatic Problem

Each problem is solved using three different activation functions:
- Hyperbolic Tangent (tanh)
- Sigmoid
- Proposed Fibonacci-based activation

## Results

The `results/` directory contains visualizations comparing the performance of each activation function for each problem. Key findings show that the Fibonacci-based activation function:

- Accelerates convergence in most cases
- Provides higher accuracy, especially in complex scenarios
- Shows robustness across various physics domains

For detailed analysis and discussion, please refer to the thesis report.

## Thesis Document

The complete thesis is available as `docs/thesis.pdf`. Its LaTeX source code is provided in `latex/thesis.zip` for those interested in the document structure or wishing to build it themselves.

## Contributing

This repository is for a completed thesis project, so new contributions aren't expected. However, if you find bugs or have suggestions for future work, please open an issue.


## Contact

[Manish Singh] - [manish.singh.mat19@itbhu.ac.in]


## Acknowledgments

- Thesis Advisor: Dr. Rajeev
- Indian Institute of Technology (BHU) VARANASI for computational resources
- Open-source community behind TensorFlow/PyTorch and other libraries

## Note on Reproducibility

To ensure reproducibility, the notebook includes:
- Random seed settings
- Detailed hyperparameter configurations
- Clear explanation of the Fibonacci-based activation function

Feel free to reach out if you have questions or need help reproducing the results.