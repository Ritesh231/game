# game
def main():
    pass

if __name__ == '__main__':
    main()
import random
for n in range(10):
    n=n+1
    computer_point=0
    human_point=0

    x=int(input("Enter your choice"))
    list=["Snake","Gun","Water","Rubber"]
    y=random.choice(list)
    print(" Choose \n 1 for 'Snake' \n 2 for 'Gun' \n 3 for 'Water' \n 4 for 'Rubber' ")
    print("Computer Chosed",y)
    if x==1:
        if y=="Snake":
            print("Tie")
        elif y=="Gun":
            print("You Lost")
            computer_point=computer_point+1
        elif y=="Rubber":
            print("You Won")
            human_point+human_point+1
        else:
            print("You Won")
            human_point=human_point+1
    elif x==2:
        if y=="Snake":
            print("You Won")
            human_point=human_point+1
        elif y=="Gun":
            print("Tie")
        elif y=="Rubber":
            print("You Won")
            human_point=human_point+1
        else:
            print("You Lost")
            computer_point=computer_point+1
    if x==3:
        if y=="Snake":
            print("You Lost")
            computer_point=computer_point+1
        elif y=="Gun":
            print("You Won")
            human_point=human_point+1
        elif y=="Rubber":
            print("You Lost")
            human_point=human_point+1
        else:
            print("You Lost")
            computer_point=computer_point+1
    elif x==4:
        if y=="Snake":
            print("You Won")
            human_point=human_point+1

        elif y=="Rubber":
          print("Tie")



print("Game over!")
if computer_point>human_point:
    print(f"You Lost the Game\nYour points {human_point}\nComputer Points {computer_point}")
elif computer_point<human_point:
    print(f"You Won the Game\nYour points {human_point}\nComputer Points {computer_point}")
else:
    print(f"Tie! Tie! Tie!\nYour points {human_point}\nComputer Points {computer_point}")
