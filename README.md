## Welcome to YommyBadd GitHub Repository 👋

![CFP_6942a](https://github.com/YommyBadd/YommyBadd/assets/154757933/2b1d0855-e029-4410-9569-68242966751e)

## About Me

Hello! I am Abayomi Badejo, a passionate Data Scientist interested in Data Science/Analyst role. This repository showcases some of my projects and contributions. Feel free to explore!

## Projects

### Project 1 (Finance Calculator)
The Finance Calculator project was developed to help anyone with free cash at hand decide whether to invest their money on simple/compound interest basis or a home bond program. The Finance Calculator's output based on the user's inputs will help the user make an informed decision on where to put their money.
See below for the code block used for the Finance Calculator.

'''py
if user_choice == 'investment':
    # Investment calculation
    principal = float(input("Enter the amount of money you are depositing: "))
    interest_rate = float(input("Enter the interest rate (as a percentage): ")) / 100
    years = int(input("Enter the number of years you plan on investing: "))
    interest_type = input("Do you want 'simple' or 'compound' interest? ").lower()

    if interest_type == 'simple':
        amount = principal * (1 + interest_rate * years)
    elif interest_type == 'compound':
        amount = principal * math.pow((1 + interest_rate), years)
    else:
        print("Invalid interest type. Please choose 'simple' or 'compound'.")

    print(f"The total amount after {years} years with {interest_rate * 100}% {interest_type} interest will be: {amount:.2f}")

elif user_choice == 'bond':
    # Bond calculation
    present_value = float(input("Enter the present value of the house: "))
    annual_interest_rate = float(input("Enter the annual interest rate: ")) / 100
    months = int(input("Enter the number of months you plan to take to repay the bond: "))

    monthly_interest_rate = annual_interest_rate / 12
    repayment = (monthly_interest_rate * present_value) / (1 - math.pow((1 + monthly_interest_rate), -months))

    print(f"The monthly repayment on the bond will be: {repayment:.2f}")
'''

### Project 2
Description of Project 2...
<!--
**YommyBadd/YommyBadd** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
