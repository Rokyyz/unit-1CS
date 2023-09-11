# Quiz005



# 1. flow diagram

![quiz 5](https://github.com/Rokyyz/unit-1CS/assets/134658259/b17dd30c-fc2b-4006-890f-d7f86bd3799d)


# 2. solutions


```.py

def sum_letters(text:str)-> int:
    alphabet = 'abcdefghijklmnopqrstuvwxyz'
    sum_total = 0
    for let in text.lower():
        index = -1
        for i in range(len (alphabet)):
            if let == alphabet[i]:
                index = i + 1
                sum_total += index
    return(sum_total)
x = sum_letters('Math')
print(x)

```

```.py

def ascii_sum(word:str)->int:
    character_sum = 0
    for character in word:
        character_sum += int(ord(character))
    return character_sum
x = ascii_sum('Math')
print(x)


```

# 3. proof of work
<img width="1440" alt="Screenshot 2023-09-11 at 23 15 15" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/c037589c-ec9a-42d7-8df6-25788c7e0e3a">
<img width="1440" alt="Screenshot 2023-09-11 at 23 15 49" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/f72d8dfb-1a1d-48fd-bb18-dadbb7e717cf">
<img width="1440" alt="Screenshot 2023-09-11 at 23 18 38" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/22c24667-fd36-48af-8345-a8746a90142a">
<img width="1440" alt="Screenshot 2023-09-11 at 23 18 58" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/5a57d679-02a0-4a83-8353-4b9b4cefb1ae">


<img width="1440" alt="Screenshot 2023-09-11 at 23 14 58" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/e4af6a97-a394-4555-a4df-c6b6757d751e">
