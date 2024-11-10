# Quiz 016


## Paper Solution


## Code
```.py
def average_word_length(input_list):
    if not isinstance(input_list, list):
        raise TypeError("Input must be a list of words.")
    
    total_length = sum(len(word) for word in input_list)
    
    if len(input_list) == 0:
        return 0.0  # to avoid division by zero if the list is empty
    
    average_length = total_length / len(input_list)
    return average_length

# example 
input_list = ["hello", "main"]
result = average_word_length(input_list)
print(result)  # expected output: 4.5

```

## Proof of work
<img width="1470" alt="Screenshot 2024-11-10 at 15 38 44" src="https://github.com/user-attachments/assets/56508611-d2e0-4b43-ae95-7b015dfc46d9">

