# ATM-machine-code
I just tried a mini python project code to create a ATM machine interface
username=input("enter the input username")
password=str(input("enter the input userpassword"))
amount=int(input("enter the previous amount from the bank"))
print("welcome to bank of India ATM machine")
print('''
       1.enter
       2.clear
       ''')
entry_option=int(input("choose your option"))
if entry_option==1:
 print('''
        1.Enter your credentials
        2.Insert your card
        ''')
 process_option=int(input("enter the process option"))
 if process_option==1:
  C_username=input("username")
  C_password=str(input("Password"))
  if C_username==username and C_password==password:
        print('''
              1.Credit
              2.Debit
              ''')
        transaction_option=int(input("enter the transaction_option"))
        if transaction_option==1:
          print('''
                  1.Cash
                  2.Check
                  ''')
          pay_option=int(input("enter the pay option"))
          if pay_option==1:
            cash_amount=int(input("enter the cash_amount"))
            amount=amount-cash_amount
            print("Total amount need to pay:",amount)
            print('''
                1.receipt
                2.No receipt
                ''')
            print_option=int(input("print_option"))
            if print_option==1:
                print("======ATM=======")
                print("Username:",username)
                print("paied_amount:",cash_amount)
                print("Total balance Amount:",amount)
                print("Thanks for visiting")
                print("================")
            else:
                    print("Exit")
          else:
              print("insert the check") 
        else:
            print('''
                    1.Deposit
                    2.Withdrawal
                    ''')
            Debit_option=int(input("choose the debit option"))
            if Debit_option==1:
             Deposit_amount=int(input("enter the Deposit amount"))
             amount+=Deposit_amount
             print("Total Balance amount:",amount)
             print('''
                1.receipt
                2.No receipt
                ''')
             print_option=int(input("print_option"))
             if print_option==1:
                print("======ATM=======")
                print("Username:",username)
                print("Deposit_amount:",Deposit_amount)
                print("Total Balance Amount:",amount)
                print("Thanks for visiting")
                print("================")
             else:
                    print("Exit")
            else:
              withdrawal_amount=int(input("enter the withdrawal amount"))
              amount-=withdrawal_amount
              print("Total Balance amount:",amount)
              print('''
                1.receipt
                2.No receipt
                ''')
              print_option=int(input("print_option"))
              if print_option==1:
                  print("======ATM=======")
                  print("Username:",username)
                  print("Withdrawal_amount:",withdrawal_amount)
                  print("Total Balance Amount:",amount)
                  print("Thanks for visiting")
                  print("================")
              else:
                    print("Exit")                
  else:
          print("Incorrect credentials")
                 
 else:
     print("Insert the card")
     print('''
              1.Credit card
              2.Debit card
              ''')
     transaction_option=int(input("enter the transaction_option"))
     if transaction_option==1:
          print('''
                  1.Cash
                  2.Check
                  ''')
          pay_option=int(input("enter the pay option"))
          if pay_option==1:
            cash_amount=int(input("enter the cash_amount"))
            amount=amount-cash_amount
          else:
              print("insert the check") 
     else:
            print('''
                    1.Deposit
                    2.Withdrawal
                    ''')
            Debit_option=int(input("choose the debit option"))
            if Debit_option==1:
             Deposit_amount=int(input("enter the Deposit amount"))
             amount+=Deposit_amount
             print("Balance Amount:",amount)
             print('''
                1.receipt
                2.No receipt
                ''')
             print_option=int(input("print_option"))
             if print_option==1:
                print("======ATM=======")
                print("Username:",username)
                print("Deposit_amount:",Deposit_amount)
                print("Total Amount:", amount)
                print("Thanks for visiting")
                print("================")
             else:
                    print("Exit")
            else:
              withdrawal_amount=int(input("enter the withdrawal amount"))
              amount-=withdrawal_amount
              print("Balance amount:",amount)
              print('''
                1.receipt
                2.No receipt
                ''')
              print_option=int(input("print_option"))
              if print_option==1:
                  print("======ATM=======")
                  print("Username:",username)
                  print("Withdrawal_amount:",withdrawal_amount)
                  print("Total Amount:", amount)
                  print("Thanks for visiting")
                  print("================")
              else:
                    print("Exit")                                     
else:
 print("clear my transcation details")
print("Thank you for choosing bank of India")
             
             
 
