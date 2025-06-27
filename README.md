# oops
#Amount Management
account = {}

class account:
    def __init__(self,acc_no,balance):
        self.acc_no = acc_no
        self.balance = balance
        print("your account no is", acc_no,"\n","your balance is",balance )
       
    def debited(self,amount):
        self.balance -= amount
        print("Rs", amount,"was debited")
        print("Total balance is:", self.total_balance())


    def credit(self,ammount):
        self.balance += ammount
        print("Rs", ammount, "was credited")
        print("Total balance is:", self.total_balance())


    def total_balance(self):
        return self.balance




acc1 = account(2351004795,1000)
acc1.debited(100)
acc1.credit(500)
