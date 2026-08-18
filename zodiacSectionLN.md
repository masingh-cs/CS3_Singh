# Chinese Zodiac Sign

Activity 3 - Implementation Selection Structure - Chinese Zodiac

Requirements:

Asks the user to enter a year of birth. The baseline year is 1900.
Validates the user input so it is not earlier than 1900.
If the user enters an invalid year, displays an appropriate message and stops the program.
Otherwise, determines the Chinese zodiac sign based on the year of birth, starting from 1900. A zodiac sign recurs every 12 years, following this order:
Rat (鼠 / Shǔ)
Ox (牛 / Niú)
Tiger (虎 / Hǔ)
Rabbit (兔 / Tù)
Dragon (龙 / Lóng)
Snake (蛇 / Shé)
Horse (马 / Mǎ)
Goat (羊 / Yáng)
Monkey (猴 / Hóu)
Rooster (鸡 / Jī)
Dog (狗 / Gǒu)
Pig (猪 / Zhū)
Only the year of birth is considered (no month/day needed).

```python
zodiacSigns = [
    "Rat (鼠 / Shǔ)",
    "Ox (牛 / Niú)",
    "Tiger (虎 / Hǔ)",
    "Rabbit (兔 / Tù)",
    "Dragon (龙 / Lóng)",
    "Snake (蛇 / Shé)",
    "Horse (马 / Mǎ)",
    "Goat (羊 / Yáng)",
    "Monkey (猴 / Hóu)",
    "Rooster (鸡 / Jī)",
    "Dog (狗 / Gǒu)",
    "Pig (猪 / Zhū)"
]

birthYear = int(input("Enter your birth year: "))

if birthYear < 1900:
    print("\nInvalid Year, it should not be earlier than 1900")
else:
    sign = (birthYear - 1900) % 12
    zodiacSign = zodiacSigns[sign]

    print("\nYour Chinese Zodiac Sign is :", zodiacSign)
```

![Program output screenshot](images/zodiac_screenshot1.png)
