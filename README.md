# Gradient Descent

**Name:** Omar Alejandro Guzmán Munguía <br>
**Email:** omar.guzman5063@alumnos.udg.mx

The objective of this activity is to apply the Gradient Descent optimization algorithm to find a local minimum of a two-dimensional function, specifically the `Matyas Function`.

The `Matyas Function`is defined as:

$$ f(x, y) = 0.26(x^2 + y^2) - 0.48xy $$

This function is a convex surface with a single global minimum at the point  (0,0).

Matyas Function
```python
def f_matyas(x, y):
    return 0.26 * (x**2 + y**2) - 0.48 * x * y
```

Gradient of the Matyas function
```python
def grad_f_matyas(x, y):
    grad_x = 0.52 * x - 0.48 * y
    grad_y = 0.52 * y - 0.48 * x
    return np.array([grad_x, grad_y])
```

### Steps Performed

**Gradient Descent Implementation**

- The Gradient Descent algorithm was implemented to iteratively update the parameters *x* and *y* in the direction of the negative gradient of the function. This process continues until convergence to the minimum is achieved.

- The learning rate and number of iterations were carefully tuned to ensure efficient and accurate convergence.

**Visualization**

- The surface of the Matyas Function was plotted to visualize its convex shape and the location of the global minimum.

- The trajectory of the Gradient Descent algorithm was overlaid on the surface plot to demonstrate the path taken by the algorithm to reach the minimum.
