# Polynomial Trainer

A browser-based learning tool that helps students analyse polynomial functions — determine end behaviour and find zeros with multiplicities.

**[Try it in your browser](https://holgerschl.github.io/PolynomialTrainer/app.html)** | **[Project website](https://holgerschl.github.io/PolynomialTrainer/)**

## Features

- **Random polynomial generation** (degree 2–5) with integer roots and small integer coefficients
- **Two display modes**: standard (expanded) form or factored form (easier)
- **End behaviour exercise**: determine whether the graph rises or falls at each end
- **Zeros and multiplicities**: enter each zero and its multiplicity
- **Graph on demand**: the plot is hidden by default — work from the formula first, then reveal to verify
- **Detailed feedback**: tells you exactly which zeros are wrong, missing, or have incorrect multiplicities
- **Solution reveal** with red dots on the graph at each zero
- **Score tracking** across the session

## Polynomial Structure

Each generated polynomial has the form:

```
f(x) = a · x^k · (bx² + cx + d)^m
```

| Component | Description | Range |
|---|---|---|
| **a** | Leading coefficient | −3, −2, −1, 1, 2, 3 |
| **k** | Power of x (root at 0 with multiplicity k) | 0 to degree |
| **bx² + cx + d** | Inner factor (quadratic or linear, monic, integer roots) | Roots in [−4, 4] |
| **m** | Power of the inner factor | 0, 1, 2, or 3 |
| **Degree** | Total: k + deg(inner) · m | 2 to 5 |

The inner factor always has "nice" integer roots so students can solve by factoring or the quadratic formula without a calculator.

## How to Use

1. Open the app in any modern browser — no installation needed
2. A polynomial formula is displayed (toggle between standard and factored form)
3. **End behaviour**: select one of the four options describing how the graph behaves at the far left and far right
4. **Zeros**: add entries for each zero, with its multiplicity
   - Multiplicity 1: graph crosses the x-axis
   - Multiplicity 2: graph touches the x-axis and bounces back
   - Multiplicity 3: graph crosses with an inflection point
5. Click **Check Answer** to verify
6. Click **Show Graph** to visualise the polynomial
7. Click **Show Solution** if stuck — zeros are highlighted with red dots

## Project Structure

```
PolynomialTrainer/
├── app.html         The web application (single file)
├── index.html       Project website (GitHub Pages)
├── README.md        This file
├── LICENSE          MIT License
└── .gitignore
```

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- HTML5 Canvas for plotting
- No dependencies, no build step
- Hosted on GitHub Pages

## License

MIT License — free to use, modify, and distribute.
