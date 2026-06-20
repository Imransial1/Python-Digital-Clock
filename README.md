# Digital Clock Using Python

A simple Digital Clock application built with Python and Tkinter.

## Features

- Real-time clock updates every second
- Displays current time in HH:MM:SS format
- Shows the current date
- Simple and user-friendly GUI

## Technologies Used

- Python
- Tkinter

## How to Run

import tkinter as tk
from time import strftime

# Main Window
root  = tk.Tk()
# Title for clock
root.title("Digital Clock")

def time():
    string = strftime('%H:%M:%S %p \n %D')
    label.config(text=string)
    label.after(1000,time)
label = tk.Label(root, font=('calibri',50,'bold'),background='yellow',foreground='black')
label.pack(anchor='center')

time()

root.mainloop()
