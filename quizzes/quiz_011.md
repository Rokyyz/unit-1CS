# Quiz011



# 1. flow diagram





# 2. solutions


```.py
def mult_table(number:int)->str:
    Table = ' '
    if number > 2 and number < 10:
        for i in range(1,11):
            Table +=f'{number} * i \n'
        else:
            Table = 'error'
        return Table

x = mult_table(3)
print(x)

```
# 3. proof of work

