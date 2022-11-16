# Investment-interests
#Interest rates for several customers with diverse amount to invest using cash or card 
# Write a programme that will: 

# Investment Amount = input()
# Customer type = input(corporate, retail, walk-in)
# payment = input(cash, card)

# Interest
# Customer type (corporate) and Payment (Cash)
# <500,000 = 10%
# >=500,000 = 15%
# >=1,000,000 = 20%
# >=2,000,000 = 25%
# Customer type (corporate) and Payment (card)
# <500,000 = 10.5%
# >=500,000 = 15.5%
# >=1,000,000 = 20.5%
# >=2,000,000 = 25.5%

# Customer type (retail) and Payment (Cash)
# Retail
# <500,000 = 5%
# >=500,000 = 10%
# >=1,000,000 = 15%
# >=2,000,000 = 20%
# Customer type (retail) and Payment (card)
# <500,000 = 5.5%
# >=500,000 = 10.5%
# >=1,000,000 = 15.5%
# >=2,000,000 = 20.5%

# Customer type (walk-in) and Payment (Cash)
# <500,000 = 2%
# >=500,000 = 8%
# >=1,000,000 = 10%
# >=2,000,000 = 15%
# Customer type (Walk-in) and Payment (card)
# <500,000 = 2.5%
# >=500,000 = 8.5%
# >=1,000,000 = 10.5%
# >=2,000,000 = 15.5%

# else Customer must be corporate, retail, walk-in
# Print all the necessary details

#--------------- Write your code below----------------------------#
investment_Amount = int(input('what is your investment amount?:      '))
Customer_type = input('Are you Cooperate, Retail or Walk in?  ')
Payment = input('what is your payment mode(cash or card)')
interest = ''
if Customer_type == 'corporate' and Payment == 'cash':
    if investment_Amount < 500000:
        interest = str(0.1*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.15*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.2*investment_Amount)
    else:
        interest = str(0.25*investment_Amount)
if Customer_type == 'corporate' and Payment == 'card':
    if investment_Amount < 500000:
        interest = str(0.105*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.155*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.205*investment_Amount)
    else:
        interest = str(0.255*investment_Amount)
if Customer_type == 'retail' and Payment == 'cash':
    if investment_Amount < 500000:
        interest = str(0.05*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.1*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.15*investment_Amount)
    else:
        interest = str(0.2*investment_Amount)
if Customer_type == 'retail' and Payment == 'card':
    if investment_Amount < 500000:
        interest = str(0.055*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.105*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.155*investment_Amount)
    else:
        interest = str(0.205*investment_Amount)
if Customer_type == 'walk-in' and Payment == 'cash':
    if investment_Amount < 500000:
        interest = str(0.02*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.08*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.1*investment_Amount)
    else:
        interest = str(0.15*investment_Amount)
else:
    if investment_Amount < 500000:
        interest = str(0.025*investment_Amount)
    elif investment_Amount >= 500000:
        interest = str(0.085*investment_Amount)
    elif investment_Amount >=1000000: 
        interest = str(0.105*investment_Amount)
    else:
        interest = str(0.155*investment_Amount)
print(f"if you want to invest {investment_Amount} in great british pounds as a {Customer_type} customer,with {Payment}, you would have to pay interest of {interest}")
   
    
