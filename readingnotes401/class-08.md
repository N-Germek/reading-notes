# List Comprehensions in Python

## Lists

Lists are the most dynamic way to code in Python and list comprehension is the most elegant way to access information and work with those lists.

## Comprehensive Python List

Below is an example of the three ingredients needed to make a comprehensive list:

```python

my_new_list = [expression for item in list] 

```

The first ingredient needed is the expression that you want to carry out in your list inside of the brackets. The second ingredient is the object that you will want that expression to manipulate. This is the item inside the square brackets. The final ingredient is the list that you want to iterate through to make your new list from. That is the list in the square brackets. List comprehension is usually faster, more flexible, more compact and cleaner to organize your lists then for loops.

## Diving Deeper into List Creation

Lets get into the steps and ways to create lists properly using multiple methods within list comprehension. The first step we will want to do is identify the method you will want to use.

The following example is with the range() method. The first x records the numbers in range. The second x represents each items in the range list created. The final piece is the number of items being saved in the digits list.

```python

# construct a basic list using range() and list comprehensions 
# syntax 
# [ expression for item in list ] 
digits = [x for x in range(10)] 

print(digits) 

# Output: 
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9] 

```

Below is a creation of a list using two methods. One is a for loop and the other is list comprehension. The for loop is far less efficient as it takes more lines of code to execute the same expression.

```python

# create a list using a for loop 
squares = []

for x in range(10): 
    # raise x to the power of 2 
    squares.append(x**2) 

print(squares) 

```

```python

# create a list using list comprehension 
squares = [x**2 for x in range(10)] 

print(squares) 

# Output for both is the same: 
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81] 

```

Now we multiple every element in our list by 3 using list comprehension.

```python

# create a list with list comprehensions 
multiples_of_three = [ x*3 for x in range(10) ] 

print(multiples_of_three) 

# Output: 
[0, 3, 6, 9, 12, 15, 18, 21, 24, 27] 

```

Adding filters to list comprehension is one way to make it more flexible since the code will accomplish more tasks at the same time. For example, assigning only the even number in a range to a list.

```python

even_numbers = [ x for x in range(1,20) if x % 2 == 0] 

# Output: 
[2, 4, 6, 8, 10, 12, 14, 16, 18] 

```

With string data types, an example of list comprehension in action is this.

```python

# a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
print(letters)

# Output: 
['E', 'L', 'F', 'T', 'E', 'S'] 

```

This will create a list of the first letter of the authors names. The next example will show you how to target the specific letters in a list and assign them individually to another list.

```python

# use list comprehension to print the letters in a string 
letters = [ letter for letter in "20,000 Leagues Under The Sea"] 

print(letters) 

# Output: 
['2', '0', ',', '0', '0', '0', ' ', 'L', 'e', 'a', 'g', 'u', 'e', 's', ' ', 'U', 'n', 'd', 'e', 'r', ' ', 'T', 'h', 'e', ' ', 'S', 'e', 'a'] 

```

Changing from upper case to lower case in list comprehension.

```python

lower_case = [ letter.lower() for letter in ['A','B','C'] ] 
upper_case = [ letter.upper() for letter in ['a','b','c'] ] 
print(lower_case, upper_case) 

# Output: 
['a', 'b', 'c'] ['A', 'B', 'C'] 

```

The isdigit() method will return a list of numbers from a list that has a mix of numbers and letters.

```python

# user data entered as name and phone number 
user_data = "Elvis Presley 987-654-3210" 
phone_number = [ x for x in user_data if x.isdigit()] 

print(phone_number) 

# Output: 
['9', '8', '7', '6', '5', '4', '3', '2', '1', '0'] 

```

One of my favorite Maya Angelou quotes can be used for an example of parsing a file in list comprehension. In this example, I have a file that I created with her quote in a .txt file.

```python

"Do the best you can until you know better. 
Then when you know better, do better." 

- Maya Angelou, November 16, 2015 

# open the file in read-only mode 

file = open("quotes.txt", 'r') 
poem = [ line for line in file ] 
for line in poem: 
    print(line) 

# Output: 
Do the best you can until you know better. 

Then when you know better, do better. 

- Maya Angelou, November 16, 2015 

```

List comprehension gives you additional freedom to write your own functions and add filters to your own code to generate lists with more specific data. This is accomplished in the example below.

```python

# list comprehension with functions 
# create a function that returns a number doubled 
def double(x): 
    return x*2 

nums = [double(x) for x in range(1,10)] 
print(nums) 

# Output: 
[2, 4, 6, 8, 10, 12, 14, 16, 18] 

# add a filter so we only double even numbers 
even_nums = [double(x) for x in range(1,10) if x%2 == 0] 
print(even_nums) 

# Output: 
[4, 8, 12, 16] 

# additional logic to specify different values for return 
nums = [x+y for x in [1,2,3] for y in [10,20,30]] 
print(nums) 

# Output: 
[11, 21, 31, 12, 22, 32, 13, 23, 33] 

```

Ultimately, what is list comprehension? It is a superpower!

## Things I want to know more about

How I can potentially refactor my data structures and algorithms code using list comprehension.

## Resources

[List Comprehensions in Python](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)

[Maya Angelou Quote](https://www.facebook.com/MayaAngelou/photos/a.485196574795/10153989278579796)

## Links

- >[Advanced Software Development](README.md)

- >[Parsing Example](quotes.txt)
