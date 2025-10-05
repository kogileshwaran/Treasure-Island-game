# Treasure-Island-game
Simple Treasure Island game

<img width="886" height="573" alt="image" src="https://github.com/user-attachments/assets/b4645da0-776b-4ef2-a7de-457fe73857fa" />

------------------Python code ----------------


print("Welcome to Treasure Island.")
print("Your mission is to find the treasure.")

choose1 = input('You\'re at a cross road. Where do you want to go?'
                'Type "left" or "right".\n').lower()
if choose1 == "left":
    choose2 = input('You\'ve come to a lake. There is an island in the middle of the lake.\n'
                    'Type "wait" to wait for a boat. '
                    'Type "swim" to swim across.\n').lower()
    if choose2 == "wait":
        choose3 = input("You arrive at the island unharmed.\n "
                        "There is a house with 3 doors.\n"
                        "One red, one yellow and one blue.\n"
                        "Which colour do you choose?\n").lower()
        if choose3 == "red":
            print ("It's a room full of fire. Game Over.")
        elif choose3 == "yellow":
            print("You found the treasure! You Win!")
        elif choose3 == "blue":
            print ("You enter a room of beasts. Game Over.")
        else:
            print("game Over")
    else:
        print("You got attacked by an angry trout. Game Over.")
else:
    print("You fell into a hole. Game Over.")
