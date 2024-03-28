# CIS_BrendaCeja_Lab5
# Brenda Ceja
# March 27 2024
#This program is meant to calculate the total number of bottles collected for seven days.
#This program will also calculate the total payout for the bottles.
# Step 1: Declare variables
total_bottles = 0  # This will store the accumulated bottle values
counter = 1  # This will control the loop
today_bottles = 0  # This will store the number of bottles returned on a day
keep_going = "y"  # This will be used to run the program again

# Step 3: Loop and run program again
while keep_going.lower() == "y":
    # Step 2: Code to set value of variables
    NBR_OF_DAYS = 7
    total_payout = 0
    total_bottles = 0  # code to set value to variable total_bottles
    counter = 0  # code to set value of counter
    while counter < NBR_OF_DAYS:
        print("Enter number of bottles returned for day #", counter + 1, ":")  # This will create the flow-like chart of the answer
        today_bottles = int(input())
        total_bottles += today_bottles
        counter += 1
    # calcPayout
    PAYOUT_PER_BOTTLE = 0.10
    total_payout = total_bottles * PAYOUT_PER_BOTTLE
    # printInfo Code
    print("Total number of bottles collected: ", total_bottles)
    print("Total payout for the week: $", total_payout)
    if counter == 7:
        keep_going = input("Do you want to enter another week's worth of data? (Enter 'y' or 'n'): ")
