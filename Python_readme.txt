learning python the hard way readMe file


Exercise 1- 

Print("to print text same was as written") 


Exercise 2- 

# hash is for comments 

"""
for multiple 
line 
comments
"""



Exercise 3- 

print("total:", 20+20) # will print as [ total: 40 ]
print( 1+2+3+4+5 ) # will print as [ 15 ]
print("what you think?", 5 > 6 ) # will print in true or false and can use any operations < > = 
				 # The print will be [ what you think? False ] 
# Greater than > ; less than < ; equal to == ; not equal to != ; greater than or equal to >= ; less than equal to <= 


Exercise 4- 

car = 40 				# 40 is stored as the car value 
driver = 30 				# 30 is stored as the driver value 
cars_not_driven = car - driver 		# cars_not_driven will be 10 (40-30)
car_color = 'sky Blue'			# car_color will be stored as sky blue

print("how many cars are not driven?", cars_not driven) 	# will print [ how many cars are not driven? 10 ]
print("there were", car, "cars") 				# will print as [ there were 40 cars]
print(f"there were {driver} drivers") 				# will print as [ there were 30 drivers ]

Exercise 6 (continue from Exercise 4)

x = f"Color of the car is {car_color} and all {car} have the same color"  # x is Color of the car is sky blue and all 40 have same color 
y = "all the car is R34" 					      # y is all car is R34
z = "or all the cars are R35"					      # ....................

print(f"I said: {x}")				# will print as [ I said: Color of the car is sky blue and all 40 have same color ]
print(f"I also said: {y}")			# will print as [ I also said: all the car is R34 ]

print (y+z) 					# will print as [ all the car is R34 or all the cars are R35 ]


Exercise 7 (continue from Exercises 4 & 6)

print("One of the best car is {}" .format('AMG')) 	# will print as [ One of the best car is AMG ]
print("." *10) 						# will print as [ .......... ] 

Car = "one of the best car is {}"
make = AMG

print(Car.format(make))					# will print as [ one of the best car is AMG ]



Exercise 8

formatter = "{} {} {} {}"						# setting up the format 
print (formatter.format(1, 2, 3, 4))					# will print as [ 1 2 3 4 ]
print(formatter.format(formatter, formatter, formatter, formatter))	# will print as [ {} {} {} {} {} {} {} {} {} {} {} {} {} {} {} {} ]
print(formatter.format(							# will print everything in one line 
    "Monday, Tuesday, Wednesday, Thursday, Friday",			# [ Monday, Tuesday, Wednesday, Thursday, Friday Seven days a week 
    "Seven days a week",						# Every hour every minute every second You know night after night ]
    "Every hour every minute every second",
    "You know night after night",
))

Exercise 9-   

'''
list- Add data, Remove data, Change data 
Tuples- cannot be changed, Immutable, made quickly   
'''

#List in example 
list_numbers = [2, 3, 4, 5, 6, 7, 8, 9, 10]

#tuple in example 
tuple_number = (2, 3, 4, 5, 6, 7, 8, 9, 10)

#there is a difference in how to give a print command 
print("list- ", list_numbers)		# [  list-  [2, 3, 4, 5, 6, 7, 8, 9, 10]   ]
print("tuple- " , tuple_number)         # 

print("-----------Assignment -------------")

#(age, contry, know_python)

survey = (27, "Vietnam", True)
age = survey[0]
coutry = survey[1]
know_python = survey[2]

print("Age- ", age ) 				# [  Age- 27  ]
print("Country- ", coutry)			# [  Country-  Vietnam ]
print("know's Python- ", know_python)		# [  know's Python-  True ]

survey2 = (21, "Switzerland", False)
age, coutry, know_python = survey2

print("Age- ", age )
print("Country- ", coutry)
print("know's Python- ", know_python)



Exercise 10- 


Print("\tI'am tabbed in") 				# will be printed with tab because of "\t" [	I'am tabbed in ]
print("I will be split\on other line") 			# will move to ther line because of "\" [ I will be split
												  on other line	]
print("I'am \\a\\ GTR")					# [ I'am \a\ GTR ]


Exercise 11

print("what is your age?",  end=' ')		# input command will be asked by the user as 
age = input()					# [ what is your age?  ] 

age = input("what is your age?  ") 		#same thing 


Exercise 13- 


from sys import argv 				#calling out function argv from sys library 


script, first, second, third = argv		# script will be file name by default, "first" will be user input same with "second" & "third"

print("The script is been called" , script)     # [ The script is been called (file_name) ]
print("your first variableis: ", first)		# [ your first variableis: (user_input) ]


----------
to run code- 
go to file location in folder > press "ctrl + L" > type "cmd" > "enter" > type (example)- python ex13.py one two three" 
-> "one two three" is the user input while runing code
-> "script, first, second, third = argv" 	script is file_name; 	there has to be -three- input  
----------


Exercise 14- 

from sys import argv

script, user_name = argv				# user_name will be inputed before running code, only 1 user input
prompt = '>'

print(f"Hi {user_name}, I am the {script} Script ")	# [ Hi (user_name), I am the (file_name) script 
print(f"your name is {user_name}?")			# [ your name is (user_input)?
likes = input(prompt)					    >    ]

print(f"which car you drive {user_name}?")
car = input(prompt)

print(f" you name is {user_name} and you drive {car}") 

Exercise 15- 


from sys import argv
script, filename = argv  		# type file name example- ReadMe.txt or ex13.py

txt = open(filename)			# file will open 

print(f"Here's your file {filename}")	# File_name will print here 
print(txt.read())			# all the data in file will print 


Exercise 18-

def print_two_again(arg1, arg2):  		#arg1 and arg2 will be picked in print statment
    print(f"arg1: {arg1}, arg2: {arg2}")

def print_one(arg1):
    print(f"arg1: {arg1}")

def print_none():
    print("I got nothing")

print_two_again("Samsung", "Apple")		#will be print as it was defined in args
print_one("First")
print_none()					# [ I got nothing ] 


Exercise 19-

def chease_and_craker(chease_count, boxes_of_crakers):
    print(f"you have {chease_count} chease!")

print("we have just give the function numbers directly: ")
chease_and_craker(20, 30)

print("we can do math even inside too:")
chease_and_craker( 10+20 , 30+50 )







