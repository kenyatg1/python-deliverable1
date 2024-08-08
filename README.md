name = input("Welcome to GC mini golf! What is your name? ")
plays = input(f"Hi, {name}! Would you like to play 3 or 6 holes? ")
if plays == "3":
    hole_1 = int(input(f"How many putts for hole 1? (par: {plays}) "))
    hole_2 = int(input(f"How many putts for hole 2? (par: {plays}) "))
    hole_3 = int(input(f"How many putts for hole 3? (par: {plays}) "))
    score = [hole_1, hole_2, hole_3]
    a = (sum(score))
    score = 9 - a
    if score < 0:
        net = score * -1
        print(f"Nice try, {name}... Your total score was: +{net}.")
    elif score in range(1, 8):
        print(f"Great job, {name}! Your total score was: -{score}.")
    elif score == 0:
        print(f"Good game, {name}. You total score was {score}")
elif plays == "6":
    hole_1 = int(input(f"How many putts for hole 1? (par: {plays}) "))
    hole_2 = int(input(f"How many putts for hole 2? (par: {plays}) "))
    hole_3 = int(input(f"How many putts for hole 3? (par: {plays}) "))
    hole_4 = int(input(f"How many putts for hole 4? (par: {plays}) "))
    hole_5 = int(input(f"How many putts for hole 5? (par: {plays}) "))
    hole_6 = int(input(f"How many putts for hole 6? (par: {plays}) "))
    score = [hole_1, hole_2, hole_3, hole_4, hole_5, hole_6]
    a = (sum(score))
    score = 18 - a
    if score < 0:
        net = score * -1
        print(f"Nice try, {name}... Your total score was: +{net}.")
    elif score in range (1, 17):
        print(f"Great job, {name}! Your total score was: -{score}.")
    elif score == 0:
        print(f"Good game, {name}. You total score was {score}")

        hello
