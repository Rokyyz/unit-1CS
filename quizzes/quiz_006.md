# Quiz006



# 1. flow diagram

![quiz 6](https://github.com/Rokyyz/unit-1CS/assets/134658259/1387a924-524c-4012-8084-1f334115b78e)


# 2. solutions


```.py

count = 0
for i in range(1,11):
    for e in range(1,11):
        count += 1
        print (f'{count}-Room {i}F{e:2d}')

```


```.py
a = int(input('please input the room you are looking for: '))
floor = 0
room = 0
if a %10 != 0:
    floor = a // 10 + 1
    room = a % 10
    room = (f'Room {floor}F{room:02d}')
else:
    floor = a // 10
    room = (f'Room {floor}F10')
print(room)

```

# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-11 at 23 07 19" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/e2e0c282-1ada-4b2f-8c09-349cb79e51eb">
<img width="1440" alt="Screenshot 2023-09-11 at 23 07 54" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/7b36e522-1907-4c57-ac9b-6be3ae50ab38">


