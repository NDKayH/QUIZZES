# Quiz 018


## Paper Solution


## Code
```.py
# AB + not(B) + not(C)B
def boolean_expression(A, B, C):
    return (A and B) or (not B) or (not C and B)

print("| A | B | C | AB + not B + not CB |")
print("|---|---|---|---------------------|")

for A in [0, 1]:
    for B in [0, 1]:
        for C in [0, 1]:

            result = boolean_expression(A, B, C)

            print(f"| {A} | {B} | {C} | {int(result)} |")

```

## Proof of work
![image](https://github.com/user-attachments/assets/a3be11e8-e1ee-49b3-9039-454f3b149a83)
