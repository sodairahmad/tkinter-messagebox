# tkinter-messagebox
how to use messagebox of tkinter 

from tkinter import *
from tkinter import messagebox

def click():
    #messagebox.showinfo(title='information box',message=" you are a human ")
    #messagebox.showwarning(title='warning box', message=" are you in sense or OK ")
    #print(messagebox.showerror(title='error box', message=" you are doing something wrong "))
     print(messagebox.askyesnocancel(title='ask question', message=" are you sure ,"
                                                                   " not or confused ",icon='question'))




window= Tk()

button= Button(window,text='click me',command=click)
button.pack()

window.mainloop()
