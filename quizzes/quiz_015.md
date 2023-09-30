# Quiz015



# 1. flow diagram

![IMG_FA7FBA70BA55-1](https://github.com/Rokyyz/unit-1CS/assets/134658259/0026e908-6aee-49ac-9799-4c0596312bf2)


# 2. solutions


```.py

def door_flipper(n):
    door = [False]*n
    for stu in range(n):
        for d in range (stu,n,stu+1):
            door[d] = not door[d]
    return door

x = door_flipper(1)
print(x)

```
# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-30 at 23 16 20" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/c86b1132-a2c9-435c-aa29-48d2c10f1b95">
