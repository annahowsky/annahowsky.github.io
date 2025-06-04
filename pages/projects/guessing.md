---
layout: default
title: Guessing Game
description: Guessing a number between 1 and 10 in Python!

---

## My Python Guessing Game
Here's the script for a simple guessing game. The user will get three chances to input their guess at the secret number!
<br>

```python
import random
winning_number = random.randint(1, 10)
attempts = 0
guess_limit = 3
while attempts < guess_limit:
    guess = int(input("Guess a number between 1-10: "))
    attempts += 1
    if guess == winning_number:
        print("Congratulations, you guessed it!")
        break
    elif attempts < guess_limit:
        print("Please guess again.")
else:
        print(f"Sorry, the number was {winning_number}. Try again next time!")
```

Back to [Projects](../projects.md)

[Homepage](../../index.md)