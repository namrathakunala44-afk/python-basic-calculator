# python-basic-calculator
A continuous python calculator with input error handling for basic arithmetic operations.
def add(a,b):
    return a+b
def sub(a,b):
    return a-bX
def mult(a,b):
    return a*b
def div(a,b):
    if(b!=0):
        return a/b
    else:
        return "ERROR division by zero"
def rem(a,b):
    return a%b
while True:
    print("Enter x,y values(enter numbers only):")
    x=int(input())
    y=int(input())
    print("select an operation(+,-,*,/):")
    choice=input()
    if choice=="+":
        print(f"The addition is{add(x,y)}")
    elif choice=="-":
        print(f"The differnce is{sub(x,y)}")
    elif choice=="*":
        print(f"The product is{mult(x,y)}")
    elif choice=="/":
        print(f"The quotient is{div(x,y)}") 
    elif choice=="%":
        print(f"The remainder is{rem(x,y)}")
    else:
        print("INVALID CHOICE! PLEASE ENTER A VALID CHOICE")  
    print("Do you want to perform another calcualtoion?")
    again=input("Type 'yes' to continue ,or any other key to exit").lower()
    if again!="yes":
        print("Goodbye! Thanks for using the calculator.")
        break
