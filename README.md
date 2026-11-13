from datetime import datetime

print("--- Event Deadline Date Formatter ---")

event_title = input("Enter event title: ")
year = int(input("Enter year: "))
month = int(input("Enter month: "))
day = int(input("Enter day: "))

try:
    event_date = datetime(year, month, day)

    print("\nFormatted Output:")
    print(f"Event: {event_title.upper()}")
    print(f"Date: {event_date.strftime('%B %d, %Y')}")
    print(f"Year: {event_date.year}")
    print(f"Month: {event_date.strftime('%B')}")
    print(f"Day: {event_date.day}")
    print(f"Weekday: {event_date.strftime('%A')}")

except ValueError:
    print("\nInvalid date entered. Please check your year, month, and day values.")
