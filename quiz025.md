# Quiz 025

## Code
```.py
def count_letters(my_dict, msg):
    for char in msg:
        if char in my_dict:  # Update count only for keys already in my_dict
            my_dict[char] += 1
    return my_dict

# Inputs
my_dict = {'w': 0, 'l': 0, 'c': 0}
msg = "hello world"

# Update my_dict with counts from msg
case1 = count_letters(my_dict, msg)
print(case1)

```

### Proof of Work
![image](https://github.com/user-attachments/assets/f212a4a4-188c-431f-80ab-d2c63772d8b6)

