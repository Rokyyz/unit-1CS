# Quiz009



# 1. flow diagram

![IMG_E85DDDD7C833-1](https://github.com/Rokyyz/unit-1CS/assets/134658259/c9a0fe68-2aef-4a81-a39c-befdd090d76f)



# 2. solutions


```.py
units = ['Tera','Giga', 'Mega', 'Kilo', 'Unit', 'Mili', 'Micro', 'Nano', 'Pico']
def powersTen(num:int)-> str:
    e = ''
    count = 0
    for i in range(-12,1,3):
        count += 1
        r = abs(i//3)
        e += f'{num}{"000" * r}'.ljust(20)
        e += f'{units[count -1]} gram of salt\n'
    for n in range(0,12,3):
        count +=1
        t = n//3
        e += f"0.{'000'* t}00{num}".center(3).ljust(20)
        e += f"{units[count-1]} gram of salt\n"
    return e

x = powersTen(1)
print(x)

```
# 3. proof of work

<img width="1440" alt="Screenshot 2023-09-30 at 20 27 28" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/905a17ff-ba5d-4b36-a3db-ee3099562859">
