# Apros v0.0.1
# Created by Pauli

import time
import os
import webbrowser as browser

version = "0.0.1"

print("Welcome to Apros " + version)

def next_line():
    print("")
    time.sleep(1)

def main_function():
    question = input("What do you want to know? \n")
    lowerQuestion = question.lower()
    splitQuestion = lowerQuestion.split()

    if lowerQuestion == "time":
        next_line()
        print(time.strftime("%H:%M", time.localtime()))
    
        next_line()
        main_function()

    elif splitQuestion[0] == "open":
        next_line()
        browser.open("www." + splitQuestion[1], new=2)

        next_line()
        main_function()

    elif lowerQuestion == "info":
        next_line()
        print("it is", time.strftime("%H:%M %A %d. %B %Y", time.localtime()))
    
        next_line()
        main_function()

    elif lowerQuestion == "year":
        next_line()
        print(time.strftime("%Y", time.localtime()))

        next_line()
        main_function()

    elif lowerQuestion == "os":
        next_line()
        print("You are using", os.name)
        
        next_line()
        main_function()

    elif lowerQuestion == "help":
        next_line()
        print("commands: time, day/date, os, info, year, open \"website\".something, exit")

        next_line()
        main_function()

    elif lowerQuestion == "exit":
        exit()

    elif lowerQuestion == "day" or "date":
        next_line()
        print(time.strftime("%d. %B %A", time.localtime()))      

        next_line()
        main_function()

    else:
        next_line()
        print("Invalid input. Try again. You can try \"help\"")
        
        next_line()
        main_function()

main_function()
