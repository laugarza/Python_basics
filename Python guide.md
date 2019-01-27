
# Basics
### Python data types:
**int**, or **integer**: a number without a fractional part. savings, with the value 100, is an example of an integer.

**float**, or **floating-point**: a number that has both an integer and fractional part, separated by a point.  The value 1.1, is an example of a float.

**str**, or **string**: a type to represent text. You can use single or double quotes to build a string.

**bool**, or **boolean**: a type to represent logical values. Can only be True or False (the capitalization is important!).

### Convert types:
Convert the types of your variables. More specifically, you'll need str(), to convert a value into a string. str(savings), for example, will convert the float savings to a string.

Similar functions such as int(), float() and bool() will help you convert Python values into any type.

	# Definition of savings and result
	savings = 100
	result = 100 * 1.10 ** 7
	print("I started with $" + str(savings) + " and now have $" + str(result) + ". Awesome!")

	# Result
	I started with $100 and now have $194.87171000000012. Awesome!
	
# Lists
A list is a compound data type; you can group values together:

	# area variables (in square meters)
	hall = 11.25
	kit = 18.0
	liv = 20.0
	bed = 10.75
	bath = 9.50

	#Create list areas
	areas = [hall, kit, liv, bed, bath]

	#Print areas
	print(areas)

	#Result
	[11.25, 18.0, 20.0, 10.75, 9.5]

## Subset lists
	# Create the areas list
	areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

	# Sum of kitchen and bedroom area: eat_sleep_area
	print(areas[3] + areas[7])

	# Print the variable eat_sleep_area
	eat_sleep_area = areas[3] + areas[7]
	print(eat_sleep_area)

	#Result
	28.75

## Slicing the list
Possible to _slice_ your list, which means selecting multiple elements from your list.

	# Create the areas list
	   areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]
        
    # Use slicing to create downstairs
        downstairs = areas[:6]
        
	# Use slicing to create upstairs
        upstairs = areas[6:]
        
	# Print out downstairs and upstairs
        print(downstairs)
        print(upstairs)
        
	# Results	
	['hallway', 11.25, 'kitchen', 18.0, 'living room', 20.0]
	['bedroom', 10.75, 'bathroom', 9.5]

## Extend lists
	# Create the areas list and make some changes
		areas = ["hallway", 11.25, "kitchen", 18.0, "chill zone", 20.0,
	         "bedroom", 10.75, "bathroom", 10.50]

	# Add poolhouse data to areas, new list is areas_1
		areas_1 = areas + ["poolhouse", 24.5]
	print(areas_1)
	
	# Add garage data to areas_1, new list is areas_2
		areas_2 = areas_1 + ["garage", 15.45]
		print (areas_2)

## Delete list elements
Remove elements from your list. You can do this with the  `del`  statement:

	x = ["a", "b", "c", "d"]
	x_new = del(x[2])

## # Inner workings of lists
to prevent changes in a  master list, for example  `areas_copy`  from also taking effect in `areas`, you'll have to do a more explicit copy of the `areas` list. You can do this with using the command `list()`

	# Create list areas
	areas = [11.25, 18.0, 20.0, 10.75, 9.50]

	# Create areas_copy
	areas_copy = list(areas)

	# Change areas_copy
	areas_copy[0] = 5.0

	# Print areas
	print(areas)
	print(areas_copy)	

	#Results
	areas = [11.25, 18.0, 20.0, 10.75, 9.50]
	areas_copy = [5.0, 18.0, 20.0, 10.75, 9.50]

#Functions
 `len()` get the length of the list; it also works on strings to count the number of character
  `complex()` returns a complex number, 
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTMzNTYwNzQ5NCwxMTM4MDA4OTk4LDgyNj
IxNzAwMSwtMTgxMDEwMDU1NSwtMTY0ODYyODkzN119
-->