#The program calculates the costs of a holiday

def holiday_costs(a, b, c):
  total = int(a) + int(b) + int(c)
  return(description + str(total))
#user requested to choose the holiday destination, each city has a different cost
city = input("Enter city of travel;1. Johannesburg, 2. Cape Town:")
if city == "1":
  city_flight = 1500
else:
  city_flight = 2050
#user requested to select number of days the will be staying at a hotel
num_nights = int(input("Enter no. of nights of stay: "))
#user requested to select number of days the will be hiring a car
rental_days = int(input("Enter number of days of car hire: "))

#The below argument calculates the hotel costs per day
hotel_costs = num_nights * 1450
#The below argument calculates the plane costs as per destination selected
plane_costs = city_flight
#The below argument calculates the rental costs per day
car_rental = rental_days * 435

description = "The total cost for your holiday is: R"
print("\n")
#The below argument calculates the total holiday costs
costs = holiday_costs(hotel_costs,plane_costs, car_rental)
print(costs)
