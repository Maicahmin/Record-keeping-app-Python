# Record-keeping-app-Python

the application will ask the user to choose between:

a. add data

b. delete data

c. end

If Add data, the application will ask the user to input key and its value

a. Enter Key: Lastname

b. Enter Value: Doe

Store the information in a dictionary

Display the result

If Delete Data, the application will ask for the key

a. Enter Key: Lastname

Remove the item from the dictionary

Display the result

If End, display THANK YOU

----------------------------------------------------------------------------------------------------

    print()

    print(">>>>>> Record Keeping App <<<<<<<")

    print()

    print("Available Operators:")

    print("A) Add Data")

    print("B) Delete Data")

    print("C) End")


    dict = {'fname': 'Maicah', 'lname': 'min'}


    while True:

    selection = str(input("\nSelect an option [A,B,C]: "))
    
    if selection.upper() == "A":
    
        a = input("\nEnter Key: ")
        
        b = input("Enter Value: ")
        
        dict [a] = [b]
        
        print("Result: " + str(dict))
        
        continue


    elif selection.upper() == "B":
    
        key = input("Enter key : ")
        
        if key in dict:
        
            del dict[key]
            
            print("Result: " + str(dict))


    elif selection.upper() == "C":
    
        print("\nThank you! ")
        
        break
        
    else:
    
        print("Invalid input.")
