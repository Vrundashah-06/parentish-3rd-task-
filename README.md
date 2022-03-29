# parentish-3rd-task-
code of 3rd task

from tkinter import *
from tkinter import messagebox

root = Tk()
root.title("Parentish: Desktop App")
root.iconbitmap("C:/Users/dell/Downloads/parentish.ico")
root.geometry("800x500")
root.resizable(False, False)

def my_click():
    top = Toplevel(root)
    top.iconbitmap("C:/Users/dell/Downloads/parentish.ico")
    top.geometry("750x250")

    padding = {'padx': 5, 'pady': 5}

    label=Label(top, text="Enter the pin", font=('Arial', 14))
    label.pack()
    entry=Entry(top, width=50,show='*',font=('Arial', 10))
    entry.pack()
    submit=Button(top, text="Submit", padx=20, pady=5,font=('Arial', 10),command=lambda: print_text(""))
    submit.pack(pady=5)


button_start = Button(root, text="Start", padx=50, pady=10,command=my_click,font=('Arial', 14))
button_start.pack(side=LEFT, padx=70)

button_stop = Button(root, text="Stop", padx=50, pady=10,command=my_click,font=('Arial', 14))
button_stop.pack(side=RIGHT, padx=70)

root.mainloop()
