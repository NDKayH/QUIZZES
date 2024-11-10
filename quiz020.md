# Quiz 001


## Paper Solution


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
![image](https://github.com/user-attachments/assets/c2e33df3-a1aa-4531-99ad-f775a5da478a)
