# Apnaproject
This is my new github project
Author - Ayan Santra

# List 
numb = ['ayan',2,4,6]
print(numb[2])


Python Data Structures: Source code
Lecture: List in Python



Creating a list of people.

people = ['John','Rob','Mike']


Printing out this list

print(people)


Printing an individual element inside of a list.

print(people[0])


Print the second member’s name

print(people[1])


Creating a list of numbers

numbers =[10,20,30,40,50]


A list with different types of data.

Movies = [’Spiderman’,’Batman’,1,2,4.5,’Hello’]


Checking order of lists

Example two lists

a = [1,2]
b=[2,1]
print(a==b)


Lecture: List Slicing

List slicing:

a[m:n] Returns list items from index m to n but does not include n
# -ve index  -6        -5      -4       -3           -2           -1
fruits = ['apple', 'mango', 'peach', 'orange', 'watermelon', 'grape']
# index     0         1       2         3          4            5
 
# list slicing
print(fruits[0:3])
print(fruits[1:3])
 
Lecture: List slicing using negative index

a[-m:-n] Returns list items from index -m to -n but does not include n
Example:

# -ve index  -6        -5      -4       -3           -2           -1
fruits = ['apple', 'mango', 'peach', 'orange', 'watermelon', 'grape']
# index     0         1       2         3          4            5
 
Negative indexing:

print(fruits[-6])
# slicing using -ve indexing
print(fruits[-5:-1])
Lecture: In and not operators



fruits = ['apple','mango','peach','orange','watermelon','grape']
 
print('apple' in fruits)
print('banana' in fruits)
print('apricot' not in fruits)
print('orange' not in fruits)
Lecture: List functions



Calculating number of items in string

print(len(fruits))


Inserting elements into a list:

fruits.insert(index,"Element to be inserted")
fruits.insert(1,"Pineapple")


Append

fruits.append('Hello')
 


Adding contents of one list into another

fruits.append(['guvava','apricot'])
 


Add items of one list to another, we use extend

fruits.extend(['guvava','apricot'])


Remove objects from a list

fruits.remove('apple')


Remove the last item in the list using pop

fruits.pop()
print(fruits)


Finding index of an item

print(fruits.index('apple'))


Min and max:

scores = [1, 2, 3, 4, 5, 6, 90, 30]
print(max(scores))
Lecture: Concat & Replicate operations on a list



Concat

a = [1, 2, 3]
b = [4, 5, 6]
print(a+b)


Replicate

print(a*3)


Lecture: Nesting lists

a = [1, 2, [3, 4, 5], 6, 7, 8, [9, 10]]
 
print(a[2])
print(a[2][0])


Lecture: Mutability of lists



a = [1, 2, 3]
a[1] = 100
print(a)
Modifying multiple items in a list:

a = [1, 2, 3]
a[0:4] = [10, 20, 30]
print(a)


Lecture: Tuples



#creating a tuple
fruits = ('apple','orange','mango','pineapple')
# printing a tuple
print(fruits)
#immutability of a tuple
fruits[1]='peach'
print(fruits)
# indexing
print(fruits[1])
#slicing
print(fruits[1:3])
#negative indexing
print(fruits[-1])


Lecture: Dictionaries



people={"John":32,"Rob":40,"Tim":20}
print(people["Rob"])
Mutability



people["Rob"]=90
print(people["Rob"])




ids = {1:"John",2:"Rob",3:"Matt"}
print(ids[2])


Another way to create a dictionary ,using the dict() function:

The argument to the dict function should be a key value pair

people =dict(
    john=32,
    rob=45,
    tim=20
)
print(people["john"])


Adding a new value

people={"John":32,"Rob":40,"Tim":20}
people["Mike"]=34
print(people)


Deleting an entry using a key

del people["John"]
print(people)


Lecture: Dictionary functions

people={"John":32,"Rob":40,"Tim":20}
 
 
print(people.get('John'))
 
 
 
prices ={'iphone':500,'ipad':400}
new_prices = {'iphone':600,'ipad':400,'imac':1500}
prices.update(new_prices)
print(prices)
 
 
new_prices = {'iphone':600,'ipad':400,'imac':1500}
new_prices.pop('ipad')
print(new_prices)
 
print(new_prices.keys())
 
 
print(new_prices.items())
 
 
print(new_prices.values())


Lecture: Sets



Set function

#creating a set
numbers = set([1,2,3,4,5,6])
print(numbers)


Creating a set is by simply using curly braces

numbers = {1,2,3,4,5}
print(numbers)


Checking the uniqueness property of set:

numbers = {1,2,3,4,1,4}
print(numbers)


Passing duplicate strings to a set:

names = {'John','Rob','Mike','John'}
print(names)


Set with different data types

s = {"John",2,4.5,True}
print(s)




Lecture: Set operations

Check if an item is present in the set

s = {"John",2,4.5,True}
print("John" in s)


Union

seta = {1,2,3,4,5}
setb = {4,5,6,7,8}
 
 
print(seta | setb )
print(seta.union(setb))


Intersection

seta = {1,2,3,4,5}
setb = {4,5,6,7,8}
 
print(seta & setb )
print(seta.intersection(setb))


Difference operation



print(seta - setb )
print(seta.difference(setb))


Symmetric difference.



print(seta ^ setb)
print(seta.symmetric_difference(setb))


Lecture: Adding & removing elements of a set

Adding element to set

seta.add(10)
print(seta)


Removing element from a set:

seta.remove(1)
print(seta)


Discard element from a set



seta.discard(10)
print(seta)


Pop
a = seta.pop()
print(a)


Clear
Removes all the elements from a set
seta.clear()


Lecture: Searching items in a list
products = ['phone','tablet','computer','laptop','journal'] item = input("Enter product to search: ") print(item in products)



Lecture: Adding & Removing Items

#inital list of products
products = ['phone','tablet','computer','laptop','journal']
 
# displaying initial list of products
print(f"Current list of items is:{products}")
 
# removing products
remove_item = input("Enter product to remove: ")
products.remove(remove_item)
 
# displaying list after product removal
print(f"Current list of items is:{products}")
 
#adding products
add_item = input("Enter product to add: ")
products.append(add_item)
 
# displaying list after adding products
print(f"Current list of items is:{products}")
 
Lecture: Adding list item at a position
#inital list of products
products = ['phone','tablet','computer','laptop','journal']
 
# displaying initial list of products
print(f"Current list of items is:{products}")
 
 
#adding products
add_item = input("Enter product to add: ")
 
#Accept product after where you want to place the current product
add_after = input(f"After which product do you want to place {add_item} ?")
index = products.index(add_after)
print(index)
products.insert(index+1,add_item)
 
# displaying list after adding products
print(f"Current list of items is:{products}")


Lecture: Adding, Deleting, Editing Dictionary Values

products ={
'phone':100,'tablet':200,'computer':300,'laptop':400,'journal':40
}
 
# print all the items inside a dictionary
print(products)
 
# search for price of product
product = input("Enter product to get price: ")
print(f"Price of {product} is ${products[product]}")
 
 
# add a product along with the price
new_product = input("Enter the product you want to add: ")
new_product_price = input(f"Enter the price for {new_product}")
products[new_product]=new_product_price
#showing the entire dictionary
print(f"Product successfully added, here is the list of products {products}")
 
# delete a product
deleted_product = input("Enter the product you want to delete")
del products[deleted_product]
print(f"Product successfully deleted, here is the list of products {products}")
 
 
# change price of the product
price_change_product = input("Enter the product to change price")
prince_change = input(f"Enter the new price for {price_change_product}")
products[price_change_product]=prince_change
print(f"Price successfully changed, here is the list of products {products}")


Section notes::

Section Notes
A list is used to store a list of items.

It is a data structure in Python that allows you to store multiple items in one place.

A variable allows you to store a single item, such as a single name. However, if you need to store multiple names, you need to use lists.

A list is an alternative to arrays in Python. In Java and C, we have arrays, but in Python, we have lists.



Let's create a list of people:

people = ['John', 'Rob', 'Mike']


To print out this list, use:

print(people)


To print an individual element inside a list, every item in the list has an index position. The first element has an index position of 0.



Let's try printing the first element:

print(people[0])


To print the second member's name:

print(people[1])


Now let's create a list of numbers:

numbers = [10, 20, 30, 40, 50]


To print elements using an index, use:

print(numbers[0])
In the next lecture, we will perform some operations on the list.



A list can have different types of data:

Movies = ['Spiderman', 'Batman', 1, 2, 4.5, 'Hello']


Lists are ordered, which means that a list is not just a collection of items; the items are in a specific order, and their order does matter.

For example, the two lists:

a = [1, 2]
b = [2, 1]
are not the same.



To check if the two lists are equal, use:

print(a == b)
You will get the result as false.



Negative list indexing:

In Python, negative list indexing refers to accessing elements of a list using negative integers as the index.

When you use a negative index, Python starts counting from the end of the list. So, the last element in the list has an index of -1, the second-to-last has an index of -2, and so on.

For example, consider the following list:

my_list = [10, 20, 30, 40, 50]
Here, my_list[-1] would give the value 50, my_list[-2] would give the value 40, and so on.

Negative indexing can be useful when you want to access the last few elements of a list, but you don't know the exact length of the list.



List slicing:

List slicing is a way to extract a portion of a list in Python.

a[m:n] 
Returns a sublist of a starting from index m up to but not including index n.



In the following example, we have a list of fruits and we are slicing the list to extract certain portions:

# -ve index  -6        -5      -4       -3           -2           -1
fruits = ['apple', 'mango', 'peach', 'orange', 'watermelon', 'grape']
# index     0         1       2         3          4            5
 
# list slicing
print(fruits[0:3])  # prints ['apple', 'mango', 'peach']
print(fruits[1:3])  # prints ['mango', 'peach']


Here, the first slice fruits[0:3] returns a sublist of fruits starting from index 0 up to but not including index 3. So it includes the elements at indices 0, 1, and 2 which are 'apple', 'mango', and 'peach' respectively.



Similarly, the second slice fruits[1:3] returns a sublist starting from index 1 up to but not including index 3. So it includes the elements at indices 1 and 2 which are 'mango' and 'peach' respectively.





List slicing using negative indexing:

a[-m:-n] returns list items from index -m to -n but does not include n


List functions:



Calculating the number of items in a list

print(len(fruits))


Inserting elements into a list:

fruits.insert(index,"Element to be inserted")
fruits.insert(1,"Pineapple")


Appending an element to the end of a list:

fruits.append('Hello')


To add the contents of one list into another, we use extend:

fruits.extend(['guava', 'apricot'])
Now the fruits will be added as individual items.



To remove an object from a list:

fruits.remove('apple')


To remove the last item in the list using pop:

fruits.pop()
print(fruits)


Finding the index of an item in a list:

print(fruits.index('apple'))








Getting the maximum values in a list:

scores = [1, 2, 3, 4, 5, 6, 90, 30] print(max(scores))



Tuples:

Like lists, tuples are also collections of items or objects.

However, the difference between tuples and lists is that tuples are immutable.

Once the items in the tuple are defined, we cannot change them.



Let's create a tuple and explain every code line by line:

# Creating a tuple
fruits = ('apple', 'orange', 'mango', 'pineapple')
# Printing a tuple
print(fruits)
# Immutability of a tuple
fruits[1] = 'peach'
print(fruits)
# Indexing
print(fruits[1])
# Slicing
print(fruits[1:3])
# Negative indexing
print(fruits[-1])
Advantages of using a tuple:

Program execution is fast with tuples. As tuples are immutable, they should be used when we don't want the data to be changed.



Dictionaries:



Dictionaries are a data structure provided by Python, just like lists.

We can store data inside a dictionary that we can later use in our program.

Let's understand what dictionaries are in Python.

We can take the example of a dictionary in the real world, which is a big book that contains the meanings of words.

If you want to find the meaning of the word "garden", you would look up that word and you will be able to find its meaning. Hence we can say that a dictionary contains a pair, i.e., a word and its meaning.

In Python, a dictionary is similar. Instead of the meaning and word, we have keys and values. Let's create a dictionary.



Suppose you want to save the age of multiple people.

people = {"John": 32, "Rob": 40, "Tim": 20}
# Here John is the key, and 32 is the value.
# Elements of a list are accessed with index,
# elements of a dictionary are accessed with a key.
# Find the age of Rob, find a value depending on a key.
print(people["Rob"])


Dictionaries are mutable, and we can change the value of a certain key. Let's try changing the age.

people["Rob"] = 90
print(people["Rob"])


We can have anything as a key-value pair in a dictionary. For example, we can have an integer as a key and a string as a value, which is exactly opposite to what we have currently. However, we cannot have the same key-value in a single dictionary.

ids = {1: "John", 2: "Rob", 3: "Matt"}
print(ids[2])


Another way to create a dictionary is by using the dict() function. The argument to the dict() function should be a key-value pair.

# We pass values as keyword arguments to the dict function.
# We have not learned about keyword arguments, but we will discuss them when we learn about functions.
people = dict(
    john=32,
    rob=45,
    tim=20
)
print(people["john"])


We can add a new value to a dictionary.

people = {"John": 32, "Rob": 40, "Tim": 20}
people["Mike"] = 34
print(people)


We can delete an entry using a key.

del people["John"]
print(people)


Sets:



A mathematical set is nothing but a collection of unique elements.



Similarly, a set in Python is a collection of elements where each element is unique and duplicates are not allowed.



Sets in Python are unordered.



There are two ways to create a set in Python:

Using the set() function:

#creating a set
numbers = set([1,2,3,4,5,6])
print(numbers)
Using curly braces:

numbers = {1,2,3,4,5}
print(numbers)


When creating a set, if duplicates are present, the set will automatically remove them:

numbers = {1,2,3,4,1,4}
print(numbers) # Output: {1, 2, 3, 4}


The same holds true for strings:

names = {'John','Rob','Mike','John'}
print(names) # Output: {'Rob', 'John', 'Mike'}


To create an empty set, we cannot use empty curly braces ({}) as it creates an empty dictionary. We need to use the set() function:

s = set()


A set can contain elements of different data types:

s = {"John",2,4.5,True}
print(s) # Output: {2, 4.5, True, 'John'}
Note that the order of elements is not retained in a set.



Set operations:



Sets cannot be sliced or indexed as they are not ordered.

However, there are different operations that can be performed on sets, which are similar to those of mathematical sets.

These operations include finding union, intersection, difference, and symmetric difference.



Union:

When you perform the union of two sets, you get all the elements of set a and all the elements of set b, but with no duplicate entries.

seta = {1, 2, 3, 4, 5}
setb = {4, 5, 6, 7, 8}
 
# union
print(seta | setb)
# the above could also be written as
print(seta.union(setb))


Intersection:

The intersection of two sets includes only those values which are common between the two sets.

seta = {1, 2, 3, 4, 5}
setb = {4, 5, 6, 7, 8}
 
# intersection
print(seta & setb)
# the above code could also be written as
print(seta.intersection(setb))


Difference operation:

The difference operation takes the elements of set a and removes all the elements which are present in set b.

It removes the values from set a which are common to both set a and set b.

# difference
print(seta - setb)
# the above code could also be written as
print(seta.difference(setb))


Symmetric difference:

The symmetric difference returns only those elements that are either in set a or in set b but not both.

print(seta ^ setb)
# this could also be written as
print(seta.symmetric_difference(setb))




Adding & removing elements of a set:



Adding elements to a set:

seta.add(10)
print(seta)


Removing elements from a set:

seta.remove(1)
print(seta)


Discarding elements from a set:

This works the same as remove, but does not raise an exception if the element is not present in the set.

seta.discard(10)
print(seta)


Pop:

This removes and returns a randomly chosen element from a set.

a = seta.pop()
print(a)


Clear:

This removes all the elements from a set.

seta.clear()
print(seta)


Searching for items in a list:

products = ['phone', 'tablet', 'computer', 'laptop', 'journal']
item = input("Enter the product to search: ")
print("Is the product in the list?", item in products)
Please note that this search is case-sensitive, so it will not work if you search for a product using capital letters. Here's an example:

Example:

Enter the product to search: Laptop
Is the product in the list? False
In the above example, the search for "Laptop" (with a capital 'L') returns False because the list contains "laptop" (with a lowercase 'l').



Adding and removing items form a list:

We first accept input from the user to add or remove items.

We then use the append & remove methods to add and remove accepted values from the list respectively:



# Initial list of products
products = ['phone', 'tablet', 'computer', 'laptop', 'journal']
 
# Displaying the initial list of products
print(f"The current list of items is: {products}")
 
# Removing products
remove_item = input("Enter the product to remove: ")
products.remove(remove_item)
 
# Displaying the list after removing the product
print(f"The current list of items is: {products}")
 
# Adding products
add_item = input("Enter the product to add: ")
products.append(add_item)
 
# Displaying the list after adding the product
print(f"The current list of items is: {products}")


Adding items at a specific position in a list:

To add items at a specific position, we make use of the index of the list along with the insert method.

The insert method of a list allows us to insert an item at a specific index position in a list.

# Initial list of products
products = ['phone', 'tablet', 'computer', 'laptop', 'journal']
 
# Displaying the initial list of products
print(f"The current list of items is: {products}")
 
# Adding products
add_item = input("Enter the product to add: ")
 
# Accepting the product after which you want to place the current product
add_after = input(f"After which product do you want to place {add_item}? ")
index = products.index(add_after)
products.insert(index + 1, add_item)
 
# Displaying the list after adding products
print(f"The current list of items is: {products}")


Adding, deleting and editing items of a dictionary:

To add a new item to a Python dictionary, we simply add a new value at a specific key for that dictionary.

To delete an item from a dictionary we use "del".

To update an item inside a Python dictionary, we use it's key and simply add a new value for the specified key.

products = {
    'phone': 100,
    'tablet': 200,
    'computer': 300,
    'laptop': 400,
    'journal': 40
}
 
# Print all the items inside the dictionary
print(products)
 
# Search for the price of a product
product = input("Enter the product to get the price: ")
print(f"The price of {product} is ${products[product]}")
 
# Add a product along with its price
new_product = input("Enter the product you want to add: ")
new_product_price = input(f"Enter the price for {new_product}: ")
products[new_product] = new_product_price
 
# Show the entire dictionary
print(f"Product successfully added. Here is the list of products: {products}")
 
# Delete a product
deleted_product = input("Enter the product you want to delete: ")
del products[deleted_product]
print(f"Product successfully deleted. Here is the list of products: {products}")
 
# Change the price of a product
price_change_product = input("Enter the product to change the price: ")
price_change = input(f"Enter the new price for {price_change_product}: ")
products[price_change_product] = price_change
print(f"Price successfully changed. Here is the list of p


