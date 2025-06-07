---
layout: default
title: The Car Game
description: Starting and Stopping the Car in Python

---

Here's the Python script for a simple car game.
The user will be asked to start or stop the car.
Where is it going? We will have to find out - in a future project!
<br>

```python
print("Welcome to the car game. Enter instructions for the car. Type help for a list of instructions.")
started = False
while True:
    command = input("Enter a new instruction: ").lower()
    if command == "help":
        print("""
start - to start the car
stop - to stop the car
quit - to exit the game
    """)
    elif command == "start":
        if started:
            print("The car has already been started!")
        else:
            started = True
            print("The car has started...")
    elif command == "stop":
        if not started:
            print("The car is already stopped!")
        else:
            started = False
            print("The car has stopped!")
    elif command == "quit":
        print("The game is over.")
        break
    else:
        print("I don't understand this instruction. Type help for help.")
```

Back to [Projects](../projects.md)

[Homepage](../../index.md)