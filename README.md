# Polynomial Trainer

A browser-based learning tool that helps students practice reading properties of polynomial functions from their graphs.

## Features

- **Random polynomial generation** up to degree 5, with integer roots and small integer coefficients
- **Two display modes**: standard (expanded) form or factored form (easier)
- **Hideable formula** for extra challenge
- **End behavior exercise**: determine whether the graph goes from bottom-left to top-right, top-left to bottom-right, etc.
- **Zeros and multiplicities**: enter each zero and its multiplicity (1, 2, or 3)
- **Detailed feedback**: tells you exactly which zeros are wrong, missing, or have incorrect multiplicities
- **Score tracking** across the session
- **Solution reveal** with red dots on the graph at each zero

## Polynomial Constraints

| Property | Range |
|---|---|
| Degree | 2 to 5 |
| Leading coefficient | -3, -2, -1, 1, 2, 3 |
| Roots | Integers in [-4, 4] (distinct) |
| Multiplicities | 1, 2, or 3 |

All polynomials are generated in factored form `f(x) = a(x - r1)^m1 (x - r2)^m2 ...` and then expanded for standard form display.

## How to Use

1. Open `index.html` in any modern browser
2. A polynomial is plotted on the graph
3. **End behavior**: select one of the four radio button options describing how the graph behaves at the far left and far right
4. **Zeros**: add entries for each zero you can see on the graph, with its multiplicity
   - Multiplicity 1: graph crosses the x-axis
   - Multiplicity 2: graph touches the x-axis and bounces back
   - Multiplicity 3: graph crosses with an inflection point
5. Click **Check Answer** to verify
6. Click **Show Solution** if stuck — zeros are highlighted with red dots

## Tech Stack

- Vanilla HTML, CSS, JavaScript
- HTML5 Canvas for plotting
- No dependencies, no build step
- Hostable on GitHub Pages

## License

MIT License — free to use, modify, and distribute.
