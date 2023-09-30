# Quiz014

# 1. flow diagram


![IMG_3F8470510869-1](https://github.com/Rokyyz/unit-1CS/assets/134658259/96ddd0a1-6dae-493a-b57f-b79cc2b6cc83)



# 2. solutions


```.py
def blackbox3(word:str):
    read = " "
    vars = []
    alpha = 'abcdefghijklmnopqrstuvwxyz'
    for i in range(26):
        vars.append(0)
    for k in range(len(word)):
        letter = word[k]
        if letter == " ":
            read += " "
        for i in range(len(alpha)):
            if letter == alpha[i]:
                vars[i]+=1
                read += f"{vars[i]}"
    return read
out = blackbox3(word = 'hello world')
print(out)

```
# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-30 at 20 50 41" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/294422d8-5044-4b4f-a1cb-0589385429aa">


<img width="1440" alt="Screenshot 2023-09-30 at 20 51 42" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/b289976a-d9f0-4d8c-9895-200c49ef2e35">
