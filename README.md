# Employee-datails
To print Employee details using python 
#!/bin/python3
class emp:
    def __init__(self):
        self.name=input("Enter the Name: ")
        self.empno=input("Enter the Empno: ")
        self.bpay=input("Enter the Basicpay: ")
class Scientist (emp):
     def __init__(self):
         emp.__init__(self)
         self.TA=input("Enter the Technical allowance: ")
         self.Category=input("Enter the Category: ")
     def disp(self):
         print("\nEmploye name",self.name,"\nEmpno",self.empno,"\nBasicpay",self.bpay,"\nTechnical allowance",self.TA,"\nCategory",self.Category)
class officer (emp):
    def __init__(self):
        emp.__init__(self)
        self.Grade=input("Enter the Grade of Officer: ")
        self.Department=input("Enter the DEpartment of Officer: ")
    def disp(self):
        print("\nEmploye name",self.name,"\nEmpno",self.empno,"\nBasicpay",self.bpay,"\nGrade",self.Grade,"\nDepartment",self.Department)
while True:
    print("Menu")
    print("1.Employe")
    print("2.Scientist")
    print("3.Officer")
    print("4.Exit")
    ch=input("choice")
    if ch=="1":
        b1=emp()
    elif ch=="2":
        b1=Scientist()
        b1.disp()
    elif ch=="3":
        b3=officer()
        b3.disp()
    elif ch=="4":
        break
    else:
        print("Invalid choice")
