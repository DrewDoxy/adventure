print("Let's hope this program works! Time to play")

Name = input("What is your name? ")
Age = int(input("How old are you? "))


health = 10



if Age >= 20:
    print("You're in.")
    wants_to_play = input("Do you want to play? (Y/N) ").lower()
    if wants_to_play == "yes":
        print("Let's get it.")
        print("You are starting with", health, "health points.")

        weapon = input("Pick a weapon (sword/shield) ").lower()
        if weapon == "shield":
            health +=5

        left_or_right = input("Here's your first choice . . . do you want to head left or right? (left/right) ").lower()
        if left_or_right == "left":
            ans = input("Nice, you went left and reached a lake. Do you want to swim across or go the long way around (across/around)? ").lower()

            if ans == "around":
                print("You went around and avoided danger. You still have full health and are on the other side of the lake. ")

            elif ans == "across":
                print("You managed to get across, but you were bit by a gator and lost 5 health. ")
                health -= 5

            ans = input("Next, you notice a river and a mountain. Which one do you go to (river/mountain)? ").lower()

            if ans == "river".lower():
                print("You found a boat, but the boat sinks and a gator bites you . . . again.")
                health -= 5
                if health <= 0:
                    print("You now have 0 health, and you lose the game")
                else:
                    print("You're still alive. In fact, you just won the game!")

            else:
                print("You successfully climbed the mountain! Victory achieved.")


        else:
            print("You rolled off the side of the cliff. Sorry, you're done.")
    else:
        print("Fine, be that way")
elif Age >=12:
    print("Grab a parent before you strap in.")
    wants_to_play = input("Do you want to play? (Y/N) ").lower()
    if wants_to_play == "yes":
        print("Make sure a parent's nearby so we can play.")
        print("You are starting with", health, "health points.")

        weapon = input("Pick a weapon (sword/shield) ").lower()
        if weapon == "shield":
                health += 5

        left_or_right = input("Here's your first choice . . . do you want to head left or right? (left/right) ").lower()
        if left_or_right == "left" or weapon == "sword":
            ans = input("Nice, you went left and reached a lake. Do you want to swim across or go the long way around (across/around)? ").lower()
            if ans == "around":
                    print("You went around and avoided danger. You still have full health and are on the other side of the lake. ")
            elif ans == "across":
                print("You managed to get across, but you were bit by a gator and lost 5 health. ")
                health -= 5

            ans = input("Next, you notice a river and a mountain. Which one do you go to (river/mountain)? ").lower()

            if ans == "river".lower():
                print("You found a boat, but the boat sinks and a gator bites you . . . again.")
                health -= 5
                if health <= 0:
                    print("You now have 0 health, and you lose the game")
                else:
                    print("You're still alive. In fact, you just won the game!")

            else:
                print("You successfully climbed the mountain! No health points lost.")
                print("Congratulations on clearing the game!")


        else:
            print("You rolled off the side of the cliff. Sorry, you're done.")
    else:
        print("We're done here, buddy.")
