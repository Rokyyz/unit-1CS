# Quiz009



# 1. flow diagram

![Com Sci 4](https://github.com/Rokyyz/unit-1CS/assets/134658259/f3039b9d-14c5-44fa-9b2d-f2f5d7dee1b8)



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
