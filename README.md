from tkinter import*
from tkinter import ttk
from tkinter import messagebox
from PIL import ImageTk

class Register:
    def __init__(self,root):
        pass
        self.root=root
        self.root.title("registration window")
        self.root.geometry("1199x600+100+50")
       # self.root.config(bg="light sky blue")


        #background image

        self.bg=ImageTk.PhotoImage(file="C:\Python\PICTURE/downloa (4).jpg")
        self.bg_image=Label(self.root,image=self.bg).place(x=0,y=0)

        #login frame
        title = Label(text="REGISTER HERE", font=("times new roman", 20, "bold"),bg="orange", fg="red").place(x=400, y=30)


        first_name = Label(text="First Name", font=("times new roman", 15, "bold"), fg="black").place(x=50,
                                                                                                              y=200)
        txt_first_name = Entry(font=("times new roman", 15, "bold"), fg="grey").place(x=50, y=230)

        #_________________________________________2row

        last_name = Label(text="Last Name", font=("times new roman", 15, "bold"), fg="black").place(x=50,
                                                                                                            y=260)
        txt_last_name = Entry( font=("times new roman", 15, "bold"), fg="grey").place(x=50, y=290)

        #_______________________________________3row

        contact = Label(text="contact number", font=("times new roman", 15, "bold"), fg="black").place(x=50,
                                                                                                               y=320)
        txt_contact = Entry(font=("times new roman", 15, "bold"), fg="grey").place(x=50, y=350)

        #________________________________________4row

        Email = Label(text="Email address", font=("times new roman", 15, "bold"), fg="black").place(x=50,
                                                                                                            y=390)
        txt_Email = Entry(font=("times new roman", 15, "bold"), fg="grey").place(x=50, y=420)


        #___________________________________________5row

        #question = Label(text="security question", font=("times new roman", 15, "bold"),fg="black").place(x=50,y=460)

        #txt_question=Entry(font=("times new roman",15,"bold"), fg="grey").place(x=50,y=490)

        #_________________________________________6row

        ts=Label(text="plz fill the infromation to apply this job", font=("times new roman", 25, "italic")).place(x=340,y=100)

        password = Label(text="Enter password", font=("times new roman", 15, "bold"),fg="black").place(x=395,y=200)
        txt_password = Entry(font=("times new roman", 15, "bold"), fg="grey").place(x=395, y=230)

        cpassword = Label(text="confirm password", font=("times new roman", 15, "bold"), fg="black").place(x=400, y=270)
        txt_cpassword = Entry(font=("times new roman", 15, "bold"), fg="grey").place(x=400, y=300)

        #_________button


        forgot= Button(text="forgot password ? ",bd=0, font=("times new roman", 15, "bold")).place(x=950, y=450)


        submit= Button(text="Login  ? ",font=("times new roman", 25, "bold")).place(x=400, y=490)

        self.bg = ImageTk.PhotoImage(file="C:\Python\PICTURE/n.jpg")
        self.bg_image = Label(self.root, image=self.bg).place(x=600, y=350)


        # def check_function(self):
        #     if self.password.get()=="" or self.cpassword.get()=="":
        #         messagebox.showerror("error","all fields are required",parent=self.root)
        #     elif self.password.get()!="shubh" or self.cpassword.get()!="12345":
        #         messagebox.showerror("error","all fields are required",parent=self.root)
        #     else:
        #         messagebox.showinfo("welcome",f"welcome{self.firstname()}")





root = Tk()
obj = Register(root)
root.mainloop()
