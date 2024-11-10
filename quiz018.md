# Quiz 018


## Paper Solution


## Code
```.py
# AB + not(B) + not(C)B
def table(A, B, C):
    return (A and B) or (not B) or (not C and B)

print("| A | B | C | AB + not B + not CB |")
print("|---|---|---|---------------------|")

for A in [0, 1]:
    for B in [0, 1]:
        for C in [0, 1]:

            result = table(A, B, C)

            print(f"| {A} | {B} | {C} |          {int(result)}          |")

```

## Proof of work
![image](https://github.com/user-attachments/assets/310f2424-a8b4-47a4-985f-832bb93d9746)
