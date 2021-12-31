# Tip-Calculator
Programme to generate the individual bill after inputting the number of people and tip to be added. 

print("welcome to the tip calculator!")
total_bill = float(input("what was the total bill?"))
tip = int(input("how much tip would you like to give? 10, 12, or 15?"))
people = int(input("How many people to split the bill?"))

bill_plus_percentage = total_bill * (tip / 100 + 1)
individual_bill = bill_plus_percentage / people 
final_bill = "{:.2f}".format(individual_bill) #Final bill rounded to two decimal places

print(f"Each person should pay: {final_bill}")
