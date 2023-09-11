# Quiz008



# 1. flow diagram

![quiz 8](https://github.com/Rokyyz/unit-1CS/assets/134658259/32f364d4-e35c-4edd-8e51-02a59b8992f9)


# 2. solutions


```.py
def cipher(text:str, shift:int)-> str:
    secret = ''
    i = 0
    for let in text:
        if let == ' ':
            secret += " "
            continue
        else:
            i = ord(let) + shift
            if i > 122:
                i -= 26
            elif i < 97:
                i += 26
        secret += chr(i)
    return secret

print(cipher(text='hello world', shift=13))
print(cipher(text='abcdefghijklmnopqrstuvwxyz', shift=13))
print(cipher(text='secret', shift=10))

```
# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-11 at 23 10 21" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/f6f66c5a-ccfc-4ecb-8be9-10a556fa1c4c">

