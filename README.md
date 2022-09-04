# adventure
Choose Your Own Adventure Game

print("Let's hope this program works! Time to play")

Name = input("What is your name? ")
Age = int(input("How old are you? "))

print("Your name is", Name + ". You are", str(Age), "years old.")

if Age >= 20:
    print("You're in.")
    wants_to_play = input("Do you want to play? ")
    if wants_to_play == "Yes":
        print("Let's get it.")
    elif wants_to_play == "yes":
        print("Let's get it")
    else:
        print("Fine, be that way")
elif Age >=12:
    print("Grab a parent before you strap in.")
    wants_to_play = input("Do you want to play? ")
    if wants_to_play == "Yes":
        print("Make sure your parent's nearby so we can play.")
    else:
        print("Maybe next time")
else:
    print("We're done here, buddy.")
