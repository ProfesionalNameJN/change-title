# change-title
from tkinter import *
from tkmacosx import Button
root = Tk()
root.title("change the title by typing in a title")
root.geometry("1000x750")
red_button = Button(root, text="click to change title", command=changeTitle)
T = Text(root, height = 5, width = 52)
def changeTitle():
	root.title(T.get("1.0", END))
root.mainloop()