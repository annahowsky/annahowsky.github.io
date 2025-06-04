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
else:
    print(f"Sorry, the number was {winning_number}. Try again next time!")
```