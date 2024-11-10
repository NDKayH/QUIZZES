# Quiz 024


## Paper Solution


## Code
```.py
import matplotlib.pyplot as plt
import numpy as np

# data for relative humidity
h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0,
     53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0,
     49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]

# time in minutes (10 min intervals)
t = np.arange(0, len(h) * 10, 10)

# calculate the mean of t and h
t_mean = np.mean(t)
h_mean = np.mean(h)

# calculate the slope (m) and intercept (b) manually
numerator = sum((t[i] - t_mean) * (h[i] - h_mean) for i in range(len(t)))
denominator = sum((t[i] - t_mean) ** 2 for i in range(len(t)))
slope = numerator / denominator
intercept = h_mean - slope * t_mean

# calculate model values for H_model = m * t + b
H_model = slope * t + intercept

# plotting the data and the linear model
plt.figure(figsize=(10, 6))
plt.plot(t, h, 'o', label='Observed Data')
plt.plot(t, H_model, 'r-', label=f'Linear Model: H_model = {slope:.2f}*t + {intercept:.2f}')
plt.xlabel('Time (minutes)')
plt.ylabel('Relative Humidity (%)')
plt.title('Relative Humidity Over Time')
plt.legend()
plt.grid(True)
plt.show()

```

## Proof of work





