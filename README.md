# Image_Viewer_by_Python_Tkinter-
# working (Under Process) :)
from tkinter import *
from PIL import ImageTk, Image

win = Tk()
win.title("Image Viewer")

from tkinter import *
from PIL import ImageTk, Image

win = Tk()
win.title("Image Viewer")

img1 = ImageTk.PhotoImage(Image.open("1-13957_free-icons-png-bird-transparent-background.png"))
img2 = ImageTk.PhotoImage(Image.open("6b28d7fb925370efd08537f2cf29be78.png"))
img3 = ImageTk.PhotoImage(Image.open("R.png"))

img_list = [img1, img2, img3]
label = Label(image=img1)
label.grid(row=0, column=0, columnspan=3)

def forward():
    global label
    global button_forward
    global button_back

    label.grid_forget()
    label= Label(image=img_list[img_number-1])





button_back = Button(win, text="<<")
button_exit = Button(win, text="Exit" ,command=win.quit)
button_forward = Button(win, text=">>", command=lambda: forward(2))

button_back.grid(row=1, column=0)
button_exit.grid(row=1, column=1)
button_forward.grid(row=1, column=2)

win.mainloop()

button_back = Button(win, text="<<")
button_exit = Button(win, text="Exit" ,command=win.quit)
button_forward = Button(win, text=">>")

button_back.grid(row=1, column=0)
button_exit.grid(row=1, column=1)
button_forward.grid(row=1, column=2)

win.mainloop()
