# CIS129_YourName_Lab4
This is my submission of lab 4!

# Module 4 Lab 4
# Elias Wilber
# 10/09/2024
# This is my attempt at Mod 4 Lab 4


def main():

# declare local variables

    storeAmount = 0
    monthlySales = 0                                        # monthly sales amount
    empAmount = 0                                           # employee bonus amount
    salesIncrease = 0                                       # percent of sales increase

def getSales(prompt):
    monthlySales = float(input("what were this months sales?"))
    return monthlySales

# This function gets the percent of increase in sales

def getIncrease(prompt):
    salesIncrease = float(input("what is the sales increase?: " ))
    salesIncrease = salesIncrease / 100
    return salesIncrease

# This function determines the storeAmount bonus


def calcStoreBonus(monthlySales):
    if monthlySales >= 110000:
        storeAmount = 6000
    elif 110000 > monthlySales >= 100000:
        storeAmount = 5000
    elif 100000 > monthlySales >= 90000:
        storeAmount = 4000
    elif 90000 > monthlySales >= 80000:
        storeAmount = 3000
    else:
        storeAmount = 0
    return storeAmount

def calcEmpBonus(salesIncrease):

# This function determines the empAmount bonus

    if salesIncrease >= .05:
        empAmount = 75.00
    elif salesIncrease >= .04:
        empAmount = 50.00
    elif salesIncrease >= 0.3:
        empAmount = 40.00
    else:
        empAmount = 0.00
    return empAmount

def printBonus(monthlySales, salesIncrease):
    
# This function prints the bonus information

    print("The store bonus amount is $", )
    print("The employee bonus amount is $", )
    if storeAmount == 6000 and empAmount == 75:
        print('Congrats! You have reached the highest bonus amounts possible! ')
