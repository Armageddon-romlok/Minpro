# Minpro
Risky farel wijaya  2509116066
<img width="1920" height="1080" alt="The Last of Us™ Part II Remastered Screenshot 2025 09 05 - 21 20 09 34" src="https://github.com/user-attachments/assets/4f627dda-b444-4ea8-9c29-c3fbd77aa359" />

flowchart
'''
import random

def main():
    print("Welcome to Guess the Number!")
    number = random.randint(1, 100)
    attempts = 0

    while True:
        guess = input("Guess a number between 1 and 100: ")
        try:
            guess = int(guess)
        except ValueError:
            print("Please enter a valid number.")
            continue

        attempts += 1

        if guess < number:
            print("Higher!")
        elif guess > number:
            print("Lower!")
        else:
            print(f"Congratulations! You guessed the number in {attempts} attempts.")
            break

if __name__ == "__main__":
    main()
