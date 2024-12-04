# Quiz 027

## Code
```.py
def sort_dict(in_dict):

    un_list = []
    or_list = []

    for v in in_dict.values():
        un_list.append(v)
    
    un_list.sort()

    for val in un_list:
        for key, value in in_dict.items():
            if value == val and key not in or_list:
                or_list.append((key, value))

    out_dict = dict(or_list)

    return out_dict

test1 = {'apple': 5, 'banana': 2, 'orange': 8, 'grape': 1}

case1 = sort_dict(in_dict = test1)
print(case1)

```

### Proof of Work
![image](https://github.com/user-attachments/assets/540a2723-f822-453e-9253-3be00201fc7b)



