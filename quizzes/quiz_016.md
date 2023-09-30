# Quiz016



# 1. flow diagram

![IMG_20337D2FACA2-1](https://github.com/Rokyyz/unit-1CS/assets/134658259/f6a295ee-6c00-4454-921f-8ddb1e2e4775)


# 2. solutions


```.py

def wordcnt(words:list)-> int:
    count = 0
    count2 = 0
    for i in words:
        count += 1
        for n in i:
            count2 += 1
    countall = count2/count
    return countall
x = wordcnt(['hello','main'])
print(x)

```
# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-30 at 23 19 03" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/ff7c2c1a-f1a6-42c1-9db5-b88c1e379882">
