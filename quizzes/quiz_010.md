# Quiz010



# 1. flow diagram

![Com Sci 5](https://github.com/Rokyyz/unit-1CS/assets/134658259/3d939b77-3ecc-498b-bb10-b1ae99c828fa)



# 2. solutions


```.py
months = int(input("Please enter your month num 1-12: "))
day = ["Fri","Sat","Sun","Mon","Tue","Wed","Thu"]
start_day=[2,5,5,1,3,6,1,4,0,2,6,0]
number_of_days = [31,28,31,30,31,30,31,31,30,31,30,31]

calendar = ""

for days in range(1, number_of_days[months-1]+1):
    w = (days-1) % 7
    t = start_day[months - 1]
    x = (w+t)%7
    calendar += f"{day[x]}{days}\t"

    if days % 7 == 0:
        calendar += "\n"

print(calendar)

```
# 3. proof of work

<img width="1440" alt="Screenshot 2023-09-30 at 20 30 02" src="https://github.com/Rokyyz/unit-1CS/assets/134658259/f1b52acb-225c-4ec6-9b44-a77664013d8f">

