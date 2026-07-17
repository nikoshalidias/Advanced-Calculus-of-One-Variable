# Advanced Calculus of One Variable — Interactive Python Notebooks

Interactive and educational Jupyter notebooks accompanying the book **_Advanced Calculus of One Variable with Python and AI_** by **Nikolaos Halidias**.

The repository contains one notebook for each chapter of the book. The notebooks combine rigorous mathematical explanations with symbolic computation, numerical experiments, visualizations, interactive controls, quizzes, and guided exercises. They are designed to help the reader explore the ideas of the book actively—not to replace proofs or the verification of mathematical hypotheses.

## Notebooks

| Chapter | Notebook | Main topics | Run in Colab |
|---|---|---|---|
| 1. The Riemann–Stieltjes Integral and Applications | [`Riemann_Stieltjes_Interactive_Notebook.ipynb`](Riemann_Stieltjes_Interactive_Notebook.ipynb) | Tagged and Darboux–Stieltjes sums, smooth and step integrators, bounded variation, numerical error bounds, improper integrals, and expectation as a Stieltjes integral | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Riemann_Stieltjes_Interactive_Notebook.ipynb) |
| 2. Infinite Series | [`Infinite_Series_Interactive_Notebook.ipynb`](Infinite_Series_Interactive_Notebook.ipynb) | Partial sums, Cauchy criterion, convergence tests, remainder bounds, condensation, Cauchy products, Dirichlet cancellation, alternating series, and rearrangements | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Infinite_Series_Interactive_Notebook.ipynb) |
| 3. Sequences and Series of Functions | [`Uniform_Convergence_Interactive_Notebook.ipynb`](Uniform_Convergence_Interactive_Notebook.ipynb) | Pointwise, uniform, and locally uniform convergence, supremum error, Dini’s theorem, equicontinuity, interchange with integration and differentiation, the Weierstrass and Dirichlet tests, and varying Stieltjes integrators | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Uniform_Convergence_Interactive_Notebook.ipynb) |
| 4. Power Series, Taylor Expansions, and Applications | [`Power_Series_Taylor_Applications_Interactive_Notebook.ipynb`](Power_Series_Taylor_Applications_Interactive_Notebook.ipynb) | Radius and endpoints, compact uniform convergence, Abel’s theorem, Taylor polynomials and error bounds, smooth versus analytic functions, probability-generating functions, branching processes, root finding, quadrature, and infinite products | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Power_Series_Taylor_Applications_Interactive_Notebook.ipynb) |
| 5. Fourier Series and Orthogonal Expansions | [`Fourier_Series_Interactive_Notebook.ipynb`](Fourier_Series_Interactive_Notebook.ipynb) | Orthogonal projection, Fourier coefficients, partial sums, Dirichlet and Fejér kernels, modes of convergence, Gibbs phenomenon, coefficient decay, Parseval’s identity, the heat equation, complex series, and convolution | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Fourier_Series_Interactive_Notebook.ipynb) |
| 6. The Fourier Transform and Its Applications | [`Fourier_Transform_Applications_Interactive_Notebook.ipynb`](Fourier_Transform_Applications_Interactive_Notebook.ipynb) | $L^1$ and $L^2$, transform pairs and operational rules, user-defined transforms, convolution, inversion, Plancherel and uncertainty, heat kernels, characteristic functions, the central limit theorem, and differential or integral equations | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Fourier_Transform_Applications_Interactive_Notebook.ipynb) |
| 7. The Laplace Transform and Its Applications | [`Laplace_Transform_Applications_Interactive_Notebook.ipynb`](Laplace_Transform_Applications_Interactive_Notebook.ipynb) | Regions of convergence, transform pairs, shifts, derivatives, convolution, periodic functions, Gamma and Beta functions, moment-generating functions, inverse transforms, Bromwich inversion, ODEs, Volterra equations, delays, difference equations, and PDEs | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Laplace_Transform_Applications_Interactive_Notebook.ipynb) |
| 8. Introduction to Differential Equations | [`Differential_Equations_Interactive_Notebook.ipynb`](Differential_Equations_Interactive_Notebook.ipynb) | Slope fields, Picard iteration, symbolic ODE solving, Euler’s method, second-order equations, Wronskians, power-series solutions, matrix exponentials, characteristics, PDE classification, heat, wave and Laplace equations, Black–Scholes, and finite differences | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nikoshalidias/Advanced-Calculus-of-One-Variable/blob/main/Differential_Equations_Interactive_Notebook.ipynb) |

## Educational design

Each notebook follows a common structure:

- mathematical explanations in English before the corresponding code cells;
- displayed mathematics rendered with MathJax;
- interactive sliders, buttons, selectors, and animations;
- symbolic calculations where they clarify the theory;
- numerical experiments and plots that make limiting behaviour visible;
- theorem and method selectors that emphasize hypotheses;
- self-check quizzes with immediate feedback;
- practice generators with guided or revealed solutions;
- direct verification of candidate solutions, especially after formal Fourier or Laplace calculations.

The notebooks repeatedly distinguish between **discovery** and **proof**. A graph or finite computation may suggest the correct conclusion, but a rigorous result still requires the hypotheses and argument stated in the book.

## Running the notebooks

### Google Colab

Use the **Open in Colab** badge in the table above. No local installation is required. Run the cells from top to bottom and allow the setup cell to install a missing package when necessary.

### JupyterLab or Jupyter Notebook

Clone the repository and enter its directory:

```bash
git clone https://github.com/nikoshalidias/Advanced-Calculus-of-One-Variable.git
cd Advanced-Calculus-of-One-Variable
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

On Linux or macOS:

```bash
source .venv/bin/activate
```

On Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

Install the required packages and start JupyterLab:

```bash
python -m pip install --upgrade pip
python -m pip install jupyterlab numpy scipy sympy matplotlib ipywidgets
jupyter lab
```

Several notebooks can install missing educational dependencies automatically in their setup cell, but installing the environment in advance gives the most consistent experience.

## Recommended learning workflow

1. Read the mathematical explanation before running the code.
2. Predict what the graph or numerical output should show.
3. Run the cell and change one parameter at a time.
4. Identify the theorem that explains the observation.
5. Check every hypothesis and distinguish numerical evidence from proof.
6. Complete the quiz or practice generator before revealing the solution.

## Software

The notebooks use the scientific Python ecosystem, principally:

- [NumPy](https://numpy.org/) for numerical arrays and computation;
- [SciPy](https://scipy.org/) for integration, optimization, special functions, and probability tools;
- [SymPy](https://www.sympy.org/) for symbolic mathematics;
- [Matplotlib](https://matplotlib.org/) for visualization;
- [ipywidgets](https://ipywidgets.readthedocs.io/) for interactive controls;
- [Jupyter](https://jupyter.org/) and [Google Colab](https://colab.research.google.com/) as notebook environments.

## Author

**Nikolaos Halidias**  
Department of Statistics and Actuarial–Financial Mathematics  
University of the Aegean, Samos, Greece

## Feedback

Questions, corrections, and suggestions for new experiments may be submitted through the repository’s issue tracker.
