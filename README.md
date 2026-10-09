# numerical-integration-methods
A simple interactive web application demonstrating the trapezoidal rule, Simpson's rule, and automatic step-size selection.

## Mathematical Methods

### 1. Trapezoidal Rule

The interval is divided into n subintervals of width

$h = \frac{(b - a)}{n}$.

The integral is approximated by

$$T_n = h \left[ \frac{f(a)}{2} + \sum_{i=1}^{n-1} f(a + ih) + \frac{f(b)}{2} \right]$$


### 2. Simpson's Rule

Simpson's rule uses quadratic approximations and requires an even number of subintervals.

$$S_n = \frac{h}{3} \left[ f(x_0) + 4 \sum_{i=1, 3, \dots}^{n-1} f(x_i) + 2 \sum_{i=2, 4, \dots}^{n-2} f(x_i) + f(x_n) \right]$$


### 3. Automatic Step-Size Selection

The program refines the interval by doubling the number
of subintervals and estimates the error by comparing
successive approximations.

## Available Functions

- $f(x) = x^2$
- $f(x) = \sin(x)$
- $f(x) = e^x$
- $f(x) = x + 1$

## How to Run

1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. Select a function and enter the interval, n, and desired accuracy.
4. Click Calculate integral.

No additional packages are required.

## Technologies

- HTML
- CSS
- JavaScript

## Author

Karamat Ali
