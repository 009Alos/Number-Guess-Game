# Number-Guess-Game
import random
user_name=input("Enter the your name ")
print('-'*10,f"Welocome {user_name} Ji in Number Guess Game ",'-'*10)
print('-'*10,"You Can Chosse Number Between 1 to 10",'-'*10)
print('*'*10,"If you want to quit then type '999' at the place of number",'*'*10)
while True:
    try:
   
   
        number=int(input("Enter the your number Please :"))
        A=random.randint(1,10)
        if 999==number:
            print(f"your Potential is too Low {user_name} to playing this game ")
            break
        elif A>number :
            print("Your number Chossed Number is Too Low ")
            print(A)
        elif A<number:
            print("Your number Chossed Number is Too High ")
            print(A)
        elif A == number :
            print("Wow! you chosse Right Number")
            print(A)
            break
        
            
    except:
        print("you entered Wrong number or invalid formate")
print(f"Thanks For Playing Game {user_name}")
