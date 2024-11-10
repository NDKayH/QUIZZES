# Quiz 022

## Code
```.py
from matplotlib import pyplot as plt
import matplotlib
import numpy as np

matplotlib.use('MacOSX')

# humidity data (y-values)
h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0,
     53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0,
     49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]

# manually create time intervals (10 min steps)
t = [i * 10 for i in range(len(h))]  # generates 0, 10, 20, ... 310

# scatter plot for observed data
plt.scatter(t, h, linewidth=1, color="#000000", label="Observed Data")

# fit a linear model (y = m*x + b)
m, b = np.polyfit(t, h, 1)
H_model = [m * ti + b for ti in t]  # model line values using list comprehension

plt.plot(t, H_model, color="red", linewidth=2, label=f"Linear Model: H_model = {m:.2f}*t + {b:.2f}")

plt.xlabel('Time (minutes)')
plt.ylabel('Relative Humidity (%)')
plt.title('Relative Humidity Over Time')
plt.legend()
plt.grid(True)

plt.show()

```

## Proof of work
![image](https://github.com/user-attachments/assets/4e70e0b0-c882-4ed4-9439-96205acf8d5d)
