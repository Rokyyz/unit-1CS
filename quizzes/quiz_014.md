# Quiz014

# 1. flow diagram




# 2. solutions


```.py
def blackbox3(word:str):
    read = " "
    vars = []
    alpha = 'abcdefghijklmnopqrstuvwxyz'
    for i in range(26):
        vars.append(0)
    for k in range(len(word)):
        letter = word[k].lower()
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
<img width="1440" alt="Screenshot 2023-09-30 at 20 56 56" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/e6a4a9e9-3bd5-403e-a44d-e27d67efb288">
<img width="1440" alt="Screenshot 2023-09-30 at 20 57 22" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/743855ac-7824-4876-9de3-0d4c0de40af8">
<img width="1440" alt="Screenshot 2023-09-30 at 20 51 42" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/b289976a-d9f0-4d8c-9895-200c49ef2e35">
