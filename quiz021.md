# Quiz 021

## Code
```.py
from matplotlib import pyplot as plt
import matplotlib

matplotlib.use('MacOSX')

# create the lists x and y
start = -10
step = 0.2  
x, y = [], []

for i in range(int(20 / step)):  # 20 = -10 to 10
    x_val = start + step * i
    x.append(x_val)
    y.append(2 * (x_val + 5) ** 2)

plt.plot(x, y, color='red')
plt.xlabel("x")
plt.ylabel("f(x) = 2(x + 5)^2")
plt.title("Graph of f(x) = 2(x + 5)^2")
plt.grid(True)
plt.show()

```

### Proof of Work
![image](https://github.com/user-attachments/assets/54d36d3b-7eb3-412e-b6b9-ba654c9c46cb)

