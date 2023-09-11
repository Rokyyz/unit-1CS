# Quiz002



# 1. flow diagram

![quiz 2](https://github.com/Rokyyz/unit-1CS/assets/134658259/20566995-8556-40d8-94be-c4d8194ac00d)


# 2. solutions


```.py

a = input('please input an integer: ')
b = input('please input an integer: ')

is20 = False

if int(a) == 20 or int(b) == 20 or int(a) + int(b) == 20:
    is20 = True

print(is20)

```

```.py
def is_20(nums1:list, nums2: list)-> bool:
    for num1 in nums1:
        for num2 in nums2:
            if num1 == 20 or num2 == 20 or num1 + num2 == 20:
                return True
            else:
                return False

print(is_20([10,30,10,26], [20, 15, 5, -6]))


```
# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-05 at 22 31 24" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/f0c03e4a-5071-46f4-a5e5-2025754a63f6">
<img width="1440" alt="Screenshot 2023-09-05 at 22 32 27" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/7f5cffd1-864e-48fd-899a-3cc84392019f">
<img width="1440" alt="Screenshot 2023-09-05 at 22 33 17" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/ef2722c7-189d-421e-bc13-aac5660062b9">
<img width="1440" alt="Screenshot 2023-09-05 at 22 33 50" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/5388755e-87fb-472a-9e37-3dace6558943">


<img width="1440" alt="Screenshot 2023-09-05 at 22 29 34" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/5c6c15db-bc76-4a16-8d94-7217dbc1079f">


