# projects-1

**Here I am on a projects that is Rock, paper, Scissor game.**


This project allows the user to play a simple Rock, Paper, Scissors game against the computer.

```python
import random
choices = ("Rock", "Paper", "Scissors")

Rock =  '''
         ✊
'''
Paper =  '''
         🤚
'''
scissor = '''
         ✌️
'''
game_image = [Rock, Paper, scissor]
user_choice = int(input("Enter your choice: type 0 for rock, 1 for paper, 2 for scissors: "))

if user_choice >= 3 or user_choice < 0:
    print("You entered an invalid number")
else:
    print("You chose:")
    print(game_image[user_choice])

    computer_choice = random.randint(0, 2)
    print("Computer chose:")
    print(game_image[computer_choice])

   
    if computer_choice == user_choice:
        print("It's a draw!")
    elif (computer_choice == 0 and user_choice == 2) or (computer_choice == 1 and user_choice == 0) or (computer_choice == 2 and user_choice == 1):
        print("You lose!")
    else:
        print("You win!")
```

**output**
```python
Enter your choice: type 0 for rock, 1 for paper, 2 for scissors:  0
You chose:

         ✊

Computer chose:

         ✌️

You win!
```



