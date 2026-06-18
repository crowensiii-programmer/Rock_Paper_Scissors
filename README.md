# Rock_Paper_Scissors
A simple Rock Paper Scissors game

#Rock Paper Scissors.


#1. Three choices that are random. -done
#2. User Input. - done
#3. compare input together.
#4. Function to play game.

#Getting a random choice from the computer
import random
three_options = ["Rock","Paper","Scissors"]
random_computer_choice = random.choice(three_options)
#print(random_computer_choice)

#user input

choice_user1 = input("Type Rock,Paper,or Scissors: ")
#print("This is what the user selected: " + choice_user1)


#Checking to see if the logic
#if choice_user1 in three_options:
  #  print("The User selected: " + choice_user1)
#else:
  #  print("Error Message: Selection is incorrect!")
    

def playGame():
    if choice_user1 == random_computer_choice:
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "This game is a tie."
#User Picks Rock
    elif choice_user1 == "Rock" and random_computer_choice == "Paper":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "Computer Wins."
    elif choice_user1 == "Rock" and random_computer_choice == "Scissors":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "User Wins."
#User Picks Paper
    elif choice_user1 == "Paper" and random_computer_choice == "Scissors":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "Computer Wins."
    elif choice_user1 == "Paper" and random_computer_choice == "Rock":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "User Wins."
#User Pick Scissors
    elif choice_user1 == "Scissors" and random_computer_choice == "Paper":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "User Wins."
    elif choice_user1 == "Scissors" and random_computer_choice == "Rock":
        print("Choice User: " + choice_user1)
        print("Computer Choice: " + random_computer_choice)
        return "Computer Wins."
       
print(playGame())
