# Quiz 016


## Paper Solution
![IMG_1101](https://github.com/user-attachments/assets/8bdb4932-1b5b-4565-bb1d-b1a2184ebeb6)


## Code
```.py
def transform_string(input_string):
    
    vowels = {
        'a': '4',
        'e': '3',
        'i': '1',
        'o': '0',
        ' ': '_'
    }
    transformed_string = ""
    for char in input_string:
        if char.lower() in vowels:
            transformed_string += vowels[char.lower()]
        else:
            transformed_string += char
        
    return transformed_string

input_string = "Hello World"
result = transform_string(input_string)
print(result)

```

## Proof of work
![image](https://github.com/user-attachments/assets/b3576d48-1dbf-4dee-8f20-51902b911286)
