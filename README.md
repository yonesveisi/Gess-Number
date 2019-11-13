# Gess-Number
# programmer : younes veisi
import random
num = random.randint(1, 1000)
user = int(input("Please enter your guess: "))
Points = 20
while 1:
    print("Points : ", Points)
    if user == num:
        print("You Win")
        Points += 1
        break
    elif user > num:
        Points -= 1
        print("please enter lower number:")
        user = int(input("enter your guess: "))
    elif user < num:
        Points -= 1
        print("please enter bigger number:")
        user = int(input("enter your guess: "))
    if Points == 0:
        print("Your Point is ZERO.\n"
              "You do not have any choice. SORRY")
        break
