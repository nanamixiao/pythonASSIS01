# pythonASSIS01

## Hi professor, I am still trying to figure out,how to export my file with .py type, I'm using pycharm, only type it supports it's HTML

``` python



""" xiaofeng xing
     Date: 02/21/2025
     Homework 01 etc
     input 7-10 to print the M
"""
# store the char *
asterisk = "*"
space = " "

# control the loop
identify = True
# output the result if the number is invaild
while identify :
    # received from user input
    lineNum = int(input("Enter the number of row between 7 and 10: "))

    if not (10 >= lineNum >= 7):
        print("Incorrect entry. Please try again")

    # if it's valid number run the code
    else:
        # set the identify to false
        identify = False

        # calculate the colum # depend on row number
        columNum = 2 * lineNum + 1
        # for the first line
        for i in range(columNum):
            if i == 0 or i == columNum - 1 or i == (columNum - 1) / 2:
                print(asterisk, end="")
            else:
                print(space, end="")
        print()

        # use to calculate the * position
        numOfSpace = 2
        # the second to the end line
        for i in range(lineNum - 1):
            for j in range(columNum):
                # determine if the begining or ending or in the middle print the *

                if j == lineNum - i - 1 or j == lineNum + numOfSpace - i - 1 or j == 0 or j == columNum - 1:
                    print(asterisk, end="")
                else:
                    print(space, end="")
            numOfSpace += 2
            print()  # enter the newline



````


