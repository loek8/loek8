import random

def guess_the_number():
    secret_number = random.randint(1, 100)
    attempts = 0

    print("Welkom bij Guess the Number!")
    print("Ik heb een nummer tussen 1 en 100 in gedachten. Kun jij het raden?")

    while True:
        guess = int(input("Doe een gok: "))
        attempts += 1

        if guess < secret_number:
            print("Hoger!")
        elif guess > secret_number:
            print("Lager!")
        else:
            print("Goed gedaan! Je hebt het nummer geraden in", attempts, "pogingen.")
            break

guess_the_number()v
