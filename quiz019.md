# Quiz 019

## Paper Solution
![IMG_1104](https://github.com/user-attachments/assets/a0584b37-6ceb-43f8-8b89-dd19a0d7f4d2)


## Code
```.py
import random

def produce(n=5, m=3, s=2):
    random.seed(1234) 
    x_values = [random.randint(0, 100) for _ in range(n)]
    y_values = [x * (0.5 * (m / s) ** 2) for x in x_values]
    return list(zip(x_values, y_values))

# Example usage
sample = produce(n=5, m=3, s=2)
print(" |   x   |   y(x)   |")
print("---------------------")
for x, y in sample:
    print(f" | {x:>4} | {y:>7.2f} |")

```

### Proof of Work
![image](https://github.com/user-attachments/assets/7dca9e20-bf9f-4996-bd74-0394a63e9375)
