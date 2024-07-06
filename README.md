# Image_Viewer_by_Python_Tkinter-
from tkinter import *
from PIL import ImageTk,Image

win=Tk()
win.title("Image Viewer")




img1 = ImageTk.PhotoImage(Image.open("4847261534.jpg"))
img2 = ImageTk.PhotoImage(Image.open("5594238194.jpg"))
img3 = ImageTk.PhotoImage(Image.open("7452702220.jpg"))

img_list = [img1,img2,img3]
label =Label(image=img1)
label.grid(row=0,column=0, columnspon=3)



button_back= Button(win, text="<<")
button_exit= Button(win, text="Exit", command=win.quit)
button_forward= Button(win, text="<<")

button_back.grid(row=1,column=0)
button_exit.grid(row=1,column=1)
button_forward.grid(row=1,column=2)






win.mainloop()
