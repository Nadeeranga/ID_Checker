# ID_Checker
#You enter some Sri Lanka NIC number and you can get answer gender and birthday of NIC number holder  
def InvalidEnter():
    command = print("You entered invalid NIC number, Please restart the program and reenter NIC Number")

id_name = input("Enter Your Name (Only letters) : ")

if(id_name.isdigit()==True):
    print("You entered invalid name")

else:
    id_number = input("Enter Your NIC Number : ")

    number_count1 = id_number[0:9]

    if (id_number.__len__() == 10 and number_count1.isdigit() == True and (id_number[9] == "v" or id_number[9] == "V")):

        gender_number = int(id_number[2:5])
        if (0 < gender_number <= 366):
            print(id_name, "your Gender is Male")
        elif (500 < gender_number < 866):
            print(id_name, "your Gender is Female")

        year_number = id_number[0:2]
        month_number = int(id_number[2:5])

        if (month_number > 500):
            month_number = month_number - 500

        if (1 <= month_number <= 31):
            print("Birthday is : ", month_number, ". 01", ". 19" + str(year_number))
        elif (31 < month_number <= 60):
            date_number = month_number - 31
            print("Birthday is : ", date_number, ". 02", ". 19" + str(year_number))
        elif (60 < month_number <= 91):
            date_number = month_number - 60
            print("Birthday is : ", date_number, ". 03", ". 19" + str(year_number))
        elif (91 < month_number <= 121):
            date_number = month_number - 91
            print("Birthday is : ", date_number, ". 04", ". 19" + str(year_number))
        elif (121 < month_number <= 152):
            date_number = month_number - 121
            print("Birthday is : ", date_number, ". 05", ". 19" + str(year_number))
        elif (152 < month_number <= 182):
            date_number = month_number - 152
            print("Birthday is : ", date_number, ". 06", ". 19" + str(year_number))
        elif (182 < month_number <= 213):
            date_number = month_number - 182
            print("Birthday is : ", date_number, ". 07", ". 19" + str(year_number))
        elif (213 < month_number <= 244):
            date_number = month_number - 213
            print("Birthday is : ", date_number, ". 08", ". 19" + str(year_number))
        elif (244 < month_number <= 274):
            date_number = month_number - 244
            print("Birthday is : ", date_number, ". 09", ". 19" + str(year_number))
        elif (274 < month_number <= 305):
            date_number = month_number - 274
            print("Birthday is : ", date_number, ". 10", ". 19" + str(year_number))
        elif (305 < month_number <= 335):
            date_number = month_number - 305
            print("Birthday is : ", date_number, ". 11", ". 19" + str(year_number))
        elif (335 < month_number <= 366):
            date_number = month_number - 335
            print("Birthday is : ", date_number, ". 12", ". 19" + str(year_number))
        else:
            InvalidEnter()

    elif (id_number.__len__() == 12 and id_number.isdigit() == True):

        gender_number = int(id_number[4:7])
        if (0 < gender_number <= 366):
            print("Gender is Male")
        elif (500 < gender_number < 866):
            print("Gender is Female")

        year_number = id_number[0:4]
        month_number = int(id_number[4:7])

        if (month_number > 500):
            month_number = month_number - 500

        if (1 <= month_number <= 31):
            print("Birthday is : ", month_number, ". 01", ".", year_number)
        elif (31 < month_number <= 60):
            date_number = month_number - 31
            print("Birthday is : ", date_number, ". 02", ".", year_number)
        elif (60 < month_number <= 91):
            date_number = month_number - 60
            print("Birthday is : ", date_number, ". 03", ".", year_number)
        elif (91 < month_number <= 121):
            date_number = month_number - 91
            print("Birthday is : ", date_number, ". 04", ".", year_number)
        elif (121 < month_number <= 152):
            date_number = month_number - 121
            print("Birthday is : ", date_number, ". 05", ".", year_number)
        elif (152 < month_number <= 182):
            date_number = month_number - 152
            print("Birthday is : ", date_number, ". 06", ".", year_number)
        elif (182 < month_number <= 213):
            date_number = month_number - 182
            print("Birthday is : ", date_number, ". 07", ".", year_number)
        elif (213 < month_number <= 244):
            date_number = month_number - 213
            print("Birthday is : ", date_number, ". 08", ".", year_number)
        elif (244 < month_number <= 274):
            date_number = month_number - 244
            print("Birthday is : ", date_number, ". 09", ".", year_number)
        elif (274 < month_number <= 305):
            date_number = month_number - 274
            print("Birthday is : ", date_number, ". 10", ".", year_number)
        elif (305 < month_number <= 335):
            date_number = month_number - 305
            print("Birthday is : ", date_number, ". 11", ".", year_number)
        elif (335 < month_number <= 366):
            date_number = month_number - 335
            print("Birthday is : ", date_number, ". 12", ".", year_number)
        else:
            InvalidEnter()

    else:
        InvalidEnter()




