
# Quiz 031

## Code
```.py
from matplotlib import pyplot as plt
import numpy as np
import matplotlib

matplotlib.use('MacOSX')

plt.style.use('ggplot')

x = []
y = []

for i in range(100):
    x_val = -2 + 0.04 * i
    x.append(x_val)
    y.append(x_val**2)

x1, y1 = x, y 
x2, y2 = [-val for val in y], x  # 90° clockwise rotation
x3, y3 = [-val for val in x], [-val for val in y]  # 180° rotation
x4, y4 = y, [-val for val in x]  # 90° counterclockwise rotation

plt.figure(figsize=(8, 8))
plt.plot(x1, y1, color="red", label="Parabola 1 (x-axis)")
plt.plot(x2, y2, color="blue", label="Parabola 2 (x axis)")
plt.plot(x3, y3, color="black", label="Parabola 3 (y-axis)")
plt.plot(x4, y4, color="purple", label="Parabola 4 (y-axis)")

# Add labels, title, legend, and grid
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Four Parabolas Aligned with Axes')
plt.legend()
plt.grid(True)

plt.show()

```

### Proof of Work
![Uploading image.png…]()


