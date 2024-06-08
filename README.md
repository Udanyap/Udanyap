#this function adds two numbers
def add(x,y):
    return x+y
#this fuction subtracts two numbers
def sub(x,y):
    return x-y
#this function multiple two numbers
def multiple(x,y):
    return x*y
#this function divides two numbers
def divide(x,y):
    return x/y
print("select operation")
print("1.add")
print("2.sub")
print("3.mutliple")
print("4.divide")
while True:
    # take input from the user
     choice=input("enter choice(1/2/3/4):")
     # check if choice is one of the four otions
     if choice in('1','2','3','4'):
         try:
             num1=float(input("enter first number:"))
             num2=float(input("enter second number:"))
             
         except ValueError:   
                 print("invalid input.please enter a number.")
                 continue
         if choice=='1':
                     print(num1,"+",num2,"=",add(num1,num2))
         elif choice=='2':
                     print(num1,"-",num2,"=",sub(num1,num2))
         elif choice=='3':   
                     print(num1,"*",num2,"=",multiple(num1,num2))
         elif choice=='4':     
                     print(num1,"/",num2,"=",divide(num1,num2))
                     #check if user wants another calculation
                     #break the while loop if answer is no
                     next_calculation=input("let's do next calculation?(yes/no):")
                     if next_calculation=="no":
                         break
                     else:
                            print("invalid input")
                    

