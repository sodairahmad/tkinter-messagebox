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

END()...................................................................................................................................

COLOR CHOOSER OPTION

from tkinter import *
from tkinter import colorchooser

def choose():
    color=colorchooser.askcolor()
    print(color)
    colorHex=color[1]
    window.config(bg=colorHex)

window= Tk()
window.geometry("420x420")

button= Button(window,text="click me to choose color",command=choose)
button.pack()

window.mainloop()

END()........................................................................................................................
