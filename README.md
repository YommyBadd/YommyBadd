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

### Project 2 (Holiday Decider)
Holiday Decider is a program developed to help users make an informed decision about where they can afford to travel to based on their budget. This program puts in consideration flight cost, hotel cost for chosen number of days and car rental cost for chosen number of days for desired number of cities to travel to. Using this program would help users see the total cost of holiday in each of the desired cities and eventually aid in decision-making based on available fund.
See below for the code block used for the Holiday Decider.

''' py


def hotel_cost(num_nights):
    # You can set the hotel cost per night
    per_night_rate = 250  # Changeable rate
    return num_nights * per_night_rate

def plane_cost(city_flight):
    # Define different flight costs for each city
    if city_flight == "Mexico":
        return 1300  
    elif city_flight == "Bangkok":
        return 1500  
    elif city_flight == "Rome":
        return 800    
    else:
        return 0  

def car_rental(rental_days):
    # Define the daily rental cost for the car
    daily_rental_rate = 120  
    return rental_days * daily_rental_rate

def holiday_cost(hotel_cost, plane_cost, car_rental):
    return hotel_cost + plane_cost + car_rental

##### Get user inputs
city_flight = input("Enter the city you will be flying to (Mexico, Bangkok, Rome): ")
num_nights = int(input("Enter the number of nights you will be staying at a hotel: "))
rental_days = int(input("Enter the number of days for which you will be hiring a car: "))

##### Calculate costs
hotel_total = hotel_cost(num_nights)
plane_total = plane_cost(city_flight)
car_total = car_rental(rental_days)
total_cost = holiday_cost(hotel_total, plane_total, car_total)

##### Print out details
print("\nHoliday Details:")
print(f"City Flight: {city_flight}")
print(f"Hotel Cost: ${hotel_total}")
print(f"Plane Cost: ${plane_total}")
print(f"Car Rental Cost: ${car_total}")
print(f"Total Holiday Cost: ${total_cost}")
'''

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
