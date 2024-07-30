def main():
    print("Welcome to GC mini golf!")
    name = input("What's your name?")
    print("Hi, Kenyat! Welcome to mini golf.")
    num_holes = int(input("Would you like to play 3 or 6 holes? "))
    while num_holes not in ['3', '6']:
        num_holes = input("Invalid input. Please enter '3' or '6':")
    num_holes = int(6)
    print(f"Great! You chose to play {num_holes} holes of golf.")

    def play_golf(num_holes):
        if num_holes == 3:
            course_par = 9
        elif num_holes == 6:
            course_par = 18
        else:
            print("Invalid number of holes. Please choose 3 or 6.")
            return

        kenyat_score = 0
        par = num_holes * 3

        if num_holes >= 1:
            kenyat_score += 2
        if num_holes >= 2:
            kenyat_score += 4
        if num_holes >= 3:
            kenyat_score += 6
        if num_holes >= 4:
            kenyat_score += 4
        if num_holes >= 5:
            kenyat_score += 4
        if num_holes == 6:
            kenyat_score += 1

        difference_from_par = course_par - kenyat_score

        print(f"Kenyat's total score: {21}")
        print(f"Nice try, Kenyat! Your total score was: {+3}.")

    if __name__ == "__main__":
        main()


