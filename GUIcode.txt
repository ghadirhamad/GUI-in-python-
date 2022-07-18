import  tkinter as tk
window = tk.Tk();
window.geometry("550x500") # width-height
window.title("sign In")
window.configure(bg='white')
topFrame = tk.Frame(bg='white')
midFrame1=tk.Frame(bg='white')
midFrame1_1=tk.Frame(bg='white')
midFrame2=tk.Frame(bg='white')
midFrame2_2=tk.Frame(bg='white')
bottomFrame = tk.Frame(bg='white')
bottomFrame1 = tk.Frame(bg='white')

lbl1 = tk.Label(topFrame, text="Sign In", font=('Georgia Bold', 20),bg='white')
lbl1.pack(fill='both',padx=5, pady=15, side=tk.LEFT)

lbl2 = tk.Label( midFrame1, text="Email adress                                                                         ",bg='white', font=('Georgia Bold', 12), justify='left')
lbl2.pack(fill='y' ,side=tk.LEFT, padx=0, pady=10)

entry1 = tk.Entry(midFrame1_1,font=('Georgia Bold', 12), width=40, relief='sunken',bg='white')
entry1.insert(0, '  Enter email')
entry1.config(fg='gray')
entry1.pack(side='bottom',ipady=7)

lbl3 = tk.Label( midFrame2, text="Password                                                                                ",bg='white', font=('Georgia Bold', 12))
lbl3.pack(side='right')

entry2 = tk.Entry(midFrame2_2,justify='left', relief='sunken', bg='white', font=('Georgia Bold', 12), width=40)
entry2.insert(0, '  Enter password')
entry2.config(fg='gray')
entry2.pack(side='bottom', ipady=7)

check = tk.Checkbutton(bottomFrame, text="Remember me                                                                 ",bg='white', font=('Georgia Bold', 12), relief='flat', justify='right')
check.pack(side='left', ipady=4, )

btn = tk.Button(bottomFrame1, text='Submit', bg='skyblue',fg='white',relief='flat',font=('Georgia', 12),width=44)
btn.pack(side='top',ipady=2)

lbl5 = tk.Label(bottomFrame1, text=('password?'), fg='sky blue',bg='white', font=('Georgia Bold', 11),justify='right')
lbl5.pack(side='right')
lbl4 = tk.Label(bottomFrame1, text=('Forget'),fg='gray',bg='white', font=('Georgia Bold', 11),justify='right')
lbl4.pack(side='right',ipady=7)


topFrame.pack(ipady=15)
midFrame1.pack(ipady=5)
midFrame1_1.pack()
midFrame2.pack(ipady=8)
midFrame2_2.pack(ipady=2)
bottomFrame.pack(ipady=10)
bottomFrame1.pack()
window.mainloop()
