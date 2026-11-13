# Version 2: Added date formatting using Python's datetime module
from datetime import datetime

# Ask the user for event details
event_title = input("Enter event title: ")
year = int(input("Enter year: "))
month = int(input("Enter month: "))
day = int(input("Enter day: "))

# Create a datetime object from the user's inputs
event_date = datetime(year, month, day)

# Format the outputs
formatted_title = event_title.upper()
readable_date = event_date.strftime("%B %d, %Y").replace(" 0", " ")
month_name = event_date.strftime("%B")
weekday_name = event_date.strftime("%A")

# Display the formatted result
print("\nFormatted Output:")
print(f"Event: {formatted_title}")
print(f"Date: {readable_date}")
print(f"Year: {year}")
print(f"Month: {month_name}")
print(f"Day: {day}")
print(f"Weekday: {weekday_name}")
