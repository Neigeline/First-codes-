# First-codes-
Trying to create something beautiful

arabicDico = []
translitDico = []
frenchDico = []
pageNumber = []
more = "Let's go"

import csv
while more != "" :

    print (more)
    
    arabicWord = input("What is the arabic word: ")
    arabicDico.append(arabicWord)
    print (arabicDico)

    translit = input("What is the transliteration: ")
    translitDico.append(translit)
    print (translitDico)

    frenchWord = input("What is the french word: ")
    frenchDico.append(frenchWord)
    print (frenchDico)

    page = input("What is the page of the word: ")
    pageNumber.append(page)
    print (pageNumber)

    print ("Here's the total dictionnary so far")
    print (list(zip(pageNumber,frenchDico,translitDico,arabicDico,)))

    more = input("Press enter if you want to exit the program.")

with open("dico.txt","w") as file:
    file.write(str(list(zip(pageNumber,frenchDico,translitDico,arabicDico))))

with open("dico.txt","r") as file:
    dico2 = eval(file.readline())


## Now, it'd be good that each time I add new words it adds them to the same file

## Find a command to search elements in the list

#Understand better how to choose the directory
#Learn the commands I've used

   
    
