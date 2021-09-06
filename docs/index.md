# New File Modified on September 06/2021


#Title
**Dev:** *SVaddi*  
**Date:** *09.03.2021*
## Structured Error Handling (Try-Except)
When ever there are multiple developers/coders handling the script, there might be bugs that the new coders create. For example, they might change the name of data file, leading to some errors.
```
# This script describes
# ------------------------------------------------- #
# Title: Error handling
# Description: A simple example of Pickling data
# ChangeLog: (Who, When, What)
# <SVaddi>,<8.31.2021>,Created Script
# ------------------------------------------------- #
# Handle it
# Demonstrates handling exceptions
# try/except
try:
    num = float(input("Enter a number:"))
except:
    print("something went wrong!")
# Specifying  exception type

try:
    num = float(input( "\nEnter a number: "))
except ValueError:
    print("That was not a number!")
# handle multiple exception types

print()
for value in (None, "Hello World!"):
    try:
        print("Attempting to convert", value, "--->", end=" ")
        print(float(value))
    except (TypeError,ValueError):
        print("Something went wrong")
# get an exception's Argument

try:
    num = float (input("\nEnter a number:"))
except ValueError as e:
    print("That was not a number! Or as Python would say....")
    print(e)
# Adding an else Clause
# try/except/else
try:
    num = float (input("\nEnter a number: "))
except ValueError:
    print("That was not a number!")
else:
    print("You entered the number", num)
input("\n\nPress the enter key to Exit.")

