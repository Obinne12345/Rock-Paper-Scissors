# Rock-Paper-Scissors
You have been tasked to create a simple version of this game with Python. In your version, one player will be controlled by the computer and the other player controlled by you - the user (i.e CPU vs Player). 
import random

user_action = input("Enter a choice (R, p, S): ")

possible_actions = ["R", "p", "S"]
computer_action = random.choice(possible_actions)

print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")
    
if user_action == computer_action:
    print(f"Both players selected {user_action}. It's a tie!")
elif user_action == "R":
    if computer_action == "S":
        print("Rock smashes scissors! You win!")
    else:
        print("Paper covers rock! You lose.")
elif user_action == "p":
    if computer_action == "R":
        print("Paper covers rock! You win!")
    else:
        print("Scissors cuts paper! You lose.")
elif user_action == "S":
    if computer_action == "P":
        print("Scissors cuts paper! You win!")
    else:
        print("Rock smashes scissors! You lose.")

while True:
    user_action = input("Enter a choice (R, P, S): ")
    possible_actions = ["R", "P", "S"]
    computer_action = random.choice(possible_actions)
    print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")

    if user_action == computer_action:
        print(f"Both players selected {user_action}. It's a tie!")
    elif user_action == "R":
        if computer_action == "S":
            print("Rock smashes scissors! You win!")
        else:
            print("Paper covers rock! You lose.")
    elif user_action == "P":
        if computer_action == "R":
            print("Paper covers rock! You win!")
        else:
            print("Scissors cuts paper! You lose.")
    elif user_action == "S":
        if computer_action == "P":
            print("Scissors cuts paper! You win!")
        else:
            print("Rock smashes scissors! You lose.")

    play_again = input("Play again? (yes/no): ")
    if play_again.lower() != "yes":
        break
     
