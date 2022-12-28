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

COLOR CHOOSER OPTION IN PYTHON USING TKINTER

CODE

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

HOW TO ENTER TEXT IN PYTHON

CODE()

from tkinter import *
def submit():
    get=text.get('1.0',END)
    print(get)
window=Tk()


text=Text(window,bg='Light Yellow',font=("bold",25),height=8,width=20,padx=20,pady=20,
          fg="red")
text.pack()
button=Button(window,text='submit',command=submit)
button.pack()

window.mainloop()
 
END()...............................................................................................

HOW TO SEARCH FILE AND OPEN FILE IN PYTHON USING TKINTER 

CODE

from tkinter import *
from tkinter import filedialog

def openFile():
    filepath=filedialog.askopenfilename(initialdir="C:\\Users\\hp\\PycharmProjects\\sodair_ahad",
                                        title='Open file okay',
                                        filetypes=(("text files","*.txt"),("All Files","*.*")))
    file=open(filepath,'r')
    print(file.read())
    file.close()

window=Tk()
button=Button(text='Open File',command=openFile)
button.pack()


window.mainloop()

END()........................................................................................

how to save user input as file(txt,all,html)  at any locaton in your laptop by using tkinter
CODE()

from tkinter import *
from tkinter import filedialog

def savefile():
    filepath=filedialog.asksaveasfile(initialdir="C:\\Users\\hp\\PycharmProjects\\sodair_ahad",
        defaultextension='.txt',
                                      filetypes=[
                                          ("all files",".*"),
                                          ("HTME FILE",".html"),
                                          ("Text FILE", ".txt")
        ])
    if file is None:
        return 
    #filetext=str(text.get(1.0,END))
    filetext=input("enter some text that you want to save ")
    filepath.write(filetext)
    filepath.close()

window= Tk()

button=Button(text='save file',command=savefile)
button.pack()
text=Text(window)
text.pack()


window.mainloop()
