# Quiz 026

## Code
```.py
def flip(input_dict):
    output_dict = {}
    
    for key, value in input_dict.items():
        output_dict[value] = key
    
    return output_dict

test1 = {'a': 1, 'b': 2, 'c': 3}

case1 = flip(test1)
print(case1)

```

### Proof of Work
![image](https://github.com/user-attachments/assets/aaa75401-e61a-48f1-a2e1-97b928b4c202)


