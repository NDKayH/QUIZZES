# Quiz 020

## Code
```.py
import random
from matplotlib import pyplot as plt

def produce(n=5, m=3, s=2):
    random.seed(1234)
    x_values = [random.randint(0, 100) for _ in range(n)]
    y_values = [x * (0.5 * (m / s) ** 2) for x in x_values]
    return x_values, y_values

x, y = produce(n=5, m=3, s=2)

plt.scatter(x, y, color="blue", label="y = x * (1/2 * (m/s)^2)")
plt.plot(x, y, color="blue", linestyle='--')  # Connect the points with a dashed line
plt.xlabel("x")
plt.ylabel("y(x)")
plt.title("Graph of y = x * (1/2 * (m/s)^2)")
plt.legend()
plt.grid(True)
plt.show()
```

### Proof of Work
![image](https://github.com/user-attachments/assets/c2e33df3-a1aa-4531-99ad-f775a5da478a)

