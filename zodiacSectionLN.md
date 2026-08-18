# Chinese Zodiac Sign

1. Asks the user to enter a year of birth. The baseline year is 1900.
2. Validates the user input so it is not earlier than 1900.
3. If the user enters an invalid year, displays an appropriate message and stops the program.
4. Otherwise, determines the Chinese zodiac sign based on the year of birth, starting from 1900. A zodiac sign recurs every 12 years, following this order:
      i. Rat (鼠 / Shǔ)
      ii. Ox (牛 / Niú)
      iii. Tiger (虎 / Hǔ)
      iv. Rabbit (兔 / Tù)
      v. Dragon (龙 / Lóng)
      vi. Snake (蛇 / Shé)
      vii. Horse (马 / Mǎ)
      viii. Goat (羊 / Yáng)
      ix. Monkey (猴 / Hóu)
      x. Rooster (鸡 / Jī)
      xi. Dog (狗 / Gǒu)
      xii. Pig (猪 / Zhū)

5. Only the year of birth is considered (no month/day needed).

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

<img width="466" height="178" alt="Screenshot 2026-08-18 150812" src="https://github.com/user-attachments/assets/0a319b27-9b75-4c30-81d0-df325639ac56" />

