# Quiz 017


## Paper Solution
![IMG_1102](https://github.com/user-attachments/assets/eb985ab6-e317-4839-970a-b758bf16ecaf)

## Code
```.py
def get_truth():

    header = "| A | B | C |\n|---|---|---|\n"
    
    rows = []
    
    for A in [0, 1]:
        for B in [0, 1]:
            for C in [0, 1]:

                rows.append(f"| {A} | {B} | {C} |")
    
    table = header + "\n".join(rows)
    return table

table = get_truth()
print(table)

```

## Proof of work
![image](https://github.com/user-attachments/assets/c3ab9d73-47f6-4692-94b8-dca8ea2d9081)


