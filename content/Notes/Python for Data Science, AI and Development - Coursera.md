---
tags:
  - python
  - datascience
  - automation
date: 2024-03-19
category:
  - note
author: miniMinn
banner: "[[Pasted image 20260625174058.png]]"
---
# 01.Python Data Structures

## About Lists and Tuples
A basic data structure and the methods commonly used in Python.
##### Tuples
An ordered sequence and immutable (fixed pair of data values).
```python
tup = ("Code", 10, 2.4)
tup_2 = ("Python", 2)

print(tup + tup_2) # Output: ('Code', 10, 2.4, 'Python', 2)
print(tup[1:3]) # Output: (10, 2.4)


# Nested tuple
tup = (12, 23, 36, 20, 51, 40, (200, 240, 100))

print(tup[6][0]) # Output: 200
```
##### Lists
Essentially used in python data structures and they are mutable.
```python
# Append method
lt = ["Code", 10, 2.4]
lt.append(["Python", 2]) # adding to the list as a single element

print(lt) # Output: ['Code', 10, 2.4, ['Python', 2]]

# Extend method
lt = ["Code", 10, 2.4]
lt.extend(["Python", 2]) # adding to the list one or multiple elements

print(lt) # Output: ['Code', 10, 2.4, 'Python', 2]


## Modifying Lists
lt = ["Code", 10, 2.4]

lt[0] = "Python" # Output: ["Python", 10, 2.4]
del(lt[2]) # Output: ["Python", 10]

## Converting string to list
data_seq = "Mike,12,2000"
list_seq = data_seq.split(',')

print(list_seq) # Output: ['Mike', '12', '2000']
```

### Methods used in Python Data Structure
##### `strip()`
It used to remove **leading** and **trailing** characters from a string.
```python
my_string = "--Hello World--"

print(my_string.strip("-")) # Output: Hello World
```

##### `copy()`
A method used to create a shallow copy of a list.
```python
my_list = [1, 2, 3, 4, 5]
new_list = my_list.copy() print(new_list)

# Output: [1, 2, 3, 4, 5]
```
##### `insert()`
Inserting an element in specific order.
```python
my_list = [1, 2, 3, 4, 5]
my_list.insert(2, 6)

# Output: [1, 2, 6, 3, 4, 5]
```

##### `pop()`
A method used to remove the element at the specified index.
```python
my_list = [10, 20, 30, 40, 50]
removed_element = my_list.pop() # Removes and returns the last element
print(removed_element)
# Output: 50

print(my_list) # Output: [10, 20, 30, 40]
```

##### `remove()`
A method used to removes the specified value in the list.
```python
my_list = [10, 20, 30, 40, 50]
my_list.remove(30) # Removes the element 30

print(my_list) # Output: [10, 20, 40, 50]
```

##### `reverse()`
A method used to reverse the order of elements in a list.
```python
my_list = [1, 2, 3, 4, 5]
my_list.reverse()

print(my_list) # Output: [5, 4, 3, 2, 1]
```

##### `sort()`
A method used to sort elements in the list.
```python
my_list = [5, 2, 8, 1, 9]
my_list.sort(reverse=True)

print(my_list) # Output: [9, 8, 5, 2, 1]
```

## Dictionaries
A dictionary consists of keys and values. It is helpful to compare a dictionary to a list. Instead of being indexed numerically like a list, dictionaries have keys. These keys are the keys that are used to access values within a dictionary.

> [!TIP] Example
> The best example of a dictionary can be accessing person's detais using the **social security number**.  
> Here the social security number which is a unique number will be the **key** and the details of the people will be the **values** associated with it.

Dictionaries in Python are an unordered, mutable, and indexed collection where each key is unique and maps to a value. Keys can only be strings, numbers, or tuples, but values can be any data type.

##### Creating a Dictionary
```python
Dict = {"key1": 1, "key2": "2", "key3": [3, 3], "key4": (4, 4), ('key5'): 5}
```
##### Modification:
```python
Dict.update({key: value}) # Add another key-value pair

Dict.clear() # Removing all key-value pairs

# Removing specific key-value pair
Dict.pop({key})
del Dict[key]
```
##### Retrieving: 
```python
Dict.keys() # Get all the keys in dictionary
Dict.values() # Get all the values in dictionary

list(Dict.keys()) # Dictionary as a list
Dict.copy() # Create a shallow copy

# Retrieves all key-value pairs as tuples and converts them into a list of tuples.
items_list
```

##### Verifying
```python
# Verify the key is in the dictionary
if 1 in Dict.values():
	...

if "Key1" in Dict.keys():
	...
```

## Sets
A set is an unordered collection of unique elements.
```python
set1 = {1,2,3,4,5,6,8,7,6,5,3,2,1,1}
print(set1) # Output: {1, 2, 3, 4, 5, 6, 7, 8}

set1.add(1) # Output still the same
set1.remove(1) # Output: {2, 3, 4, 5, 6, 7, 8}

# Verify an element in the set
1 in set1 # True
```

Set logic operations:
```python
set1 = {1,2,3,4,5}
set2 = {4,5,6,7,8}

intersection = set1.intersection(set2) # Output: {4,5}
difference = set1.difference(set2) # Output: {1,2,3}
union = set1.union(set2) # Output: {1,2,3,4,5,6,7,8}
```

`superset` and `subset`:

```python
set1 = {1,2,3,4,5}
set2 = {4,5}

issupertset = set1.issuperset(set2) # Output: True
issubset = set2.subset(set1) # Output: True
```

---
# 02.Programming Fundamentals



## Conditions and Branching
About logical comparisons `>, <, ==, !=, >=, <=...` and logic gates `AND, OR, NAND...`
Then, condition checking with `if, else, elif...`

---
## Loops
Modifying the list with `for` loop:
```python
colors = ["Yellow", "Red", "Cyan", "Blue", "Purple"]

def change_all_white():
	for i in range(0, len(colors)):
		colors[i] = "White"

change_all_white()
print(colors)
```

![[Pasted image 20250509161520.png|380]]

Iterate on both index and element value:
```python
# Loop through the list
students = ['Jake', 'Steve', 'Alex', 'Rina']

for i, student in enumerate(students):
	print(i, student)

## Output:
# 0 Jake
# 1 Steve
# 2 Alex
# 3 Rina
```

`while` loop:
```python
dates = [1982, 1980, 1973, 2000]

i = 0
year = dates[0]

while(year != 1973):    
    print(year)
    i += 1
    year = dates[i]
```

---
## Functions
Defining a function:
```python
def function_name():
	pass # Used to for no-operation statement
```

When the number of arguments to be used for a function, they can be packed into a **tuple**:
```python
def printAll(*args): # <-- Dynamic
	print("No of arguments:", len(args))

	for argument in args:
	print(argument)

printAll('Horsefeather','Adonis','Bone') # 3 arguments in output
printAll('Sidecar','Long Island','Mudslide','Carriage') # 4 arguments in output
```
#### Local and Global Variables 
Initialising variables:
```python
Global_var = "This is Global Variable."

def function_name():
	Local_var = "This is Local Variable."

	print(Global_var) # Accessable outside the function
	print(Local_var) # Only accessable inside the function
```

Initialising global variable in the function:
```python
# ERROR PROGRAM
album = "The BodyGuard"
def printer1(album):
    internal_var1 = "Thriller"
    print(album, "is an album")
    
printer1(album)
printer1(internal_var1) # This raises an error
```

The solution to access variable inside the function from entire program:
```python
# SOLUTION PROGRAM
album = "The BodyGuard"

def printer(album):
    global internal_var # <-- initialising as global variable
    internal_var= "Thriller"
    print(album,"is an album")

printer(album) 
printer(internal_var)
```

---
## Common <mark style="background: #FFF3A3A6;">Exceptions</mark> in Python

1. `ZeroDivisionError`: Division by zero is undefined in mathematics, causing an arithmetic error.
```python
result = 10 / 0
print(result) # Raises ZeroDivisionError
```

2. `ValueError`: An error occurs when an inappropriate value is used within the code, such as trying to convert a non-numeric `str` into `int`.
```python
num = int("ABC") # Raises ValueError
```

3. `FileNotFoundError`: Attempting to access a file that doesn't exists.
```python
with open("nonexistent_file.txt", "r") as file:
	content = file.read() # Raises FileNotFoundError
```

4. `AttributeError`: An error occurs when an attribute or method are used incorrectly.
```python
text = "Example"
length = text.countTheLengthLOL() # Raises AttributeError
```

## Handling Exceptions

Python has `try and except` built-in tool to handle and manage exceptions to prevent the program from crashing.

Example of `try-except`:
```python 
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: Cannot divide by zero")
```

Example of `try-except-finally`:
```python
A = 1

try:
    B = int(input("Please enter a number to divide A"))
    A = A/B
except ZeroDivisionError:
    print("0 division is undefined")
except ValueError:
    print("Only numbers accepted")
except:
    print("Something went wrong")
else:
    print("success A=",A)
finally:
	print("Process Completed")
```

---
## Classes and Objects
##### Creating a `Class`
First step to create a class is giving a **name**. Then, determine all the data that make up that class, which are **attributes** (as variables).

`__init__` is a **constructor** (special method) used to initialise a the object. The `self` contains all the attributes in the set.  The class parent will always be `object` (for this course).

```python
# Importing a lib for graphical visualisation
import matplotlib.pyplot as plt
  

class Circle(object):

	# Constructor
	def __init__(self, radius=3, color='blue'):
		self.radius = radius
		self.color = color

	# Method
	def add_radius(self, r):
		self.radius = self.radius + r
		return(self.radius)

	# Method
	def drawCircle(self):
		plt.gca().add_patch(plt.Circle((0, 0),radius=self.radius,fc=self.color))
		plt.axis('scaled')
		plt.show()
```

Creating a **Blue Circle**:
```python
# Creating a Blue circle, then, output.
Blue_Circle = Circle(4, "blue")
Blue_Circle.drawCircle()
```

Listing out the object's methods:
```python
print(dir(Blue_Circle))

# Output:
# ['__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__'...
```

---
## A `TextAnalyzer` practical lab from the module

```python
class TextAnalyzer(object):
    
    def __init__ (self, text):
        # remove punctuation
        formattedText = text.replace('.','').replace('!','').replace('?','').replace(',','')
        
        # make text lowercase
        formattedText = formattedText.lower()
        
        self.fmtText = formattedText
        
    def freqAll(self):        
        # split text into words
        wordList = self.fmtText.split(' ')
        
        # Create dictionary
        freqMap = {}
        for word in set(wordList): # use set to remove duplicates in list
            freqMap[word] = wordList.count(word)
        
        return freqMap
    
    def freqOf(self,word):
        # get frequency map
        freqDict = self.freqAll()
        
        if word in freqDict:
            return freqDict[word]
        else:
            return 0
```

Retrieving the `fmtText` of feedback_1:
```python
feedback_1 = "Your product is good, but there's something I want to suggest? the reliability is good but not enough!"  
analyzed_text = TextAnalyzer(feedback_1)  
  
print(analyzed_text.fmtText)
```

---

# 03.Working with Data in Python

## Reading and Writing Files with `Open`
Python's `open` function creates an object and access to data within the text file.
	- **File Path**: the location of the file to be opened.
	- **Mode**: the purpose of opening the file (`r` for reading, `w` for writing and `a` for appending).

```python
file = open('file.txt', 'r') # opening the file in read mode
```

---
#### Using `with` Statement
The `with` statement is used in most Python operations as it is a best practice when working with file, which ensures the file are properly closed after operation.
	- `with` is good for **automatic resource management**.

```python
with open('file.txt', 'r') as file:
	# Code...
```

Reading entire content:
```python
# to read with a function
def read_file(path):  
    with open(path, 'r') as file:  
        content = file.read()  
        return content  
  
print(read_file('file.txt'))
```

#### Reading Line-by-Line with `readline()`
`readline()` method provides to read the files line by line, and store each line as 

```python
line_1 = file.readline('file.txt', 'r')
line_2 = file.readline('file.txt', 'r')
```

Using with `while` loop:
```python
while True:
	line = file.readline('file.txt', 'r')

	# Break when there're no more lines in file.txt
	if not line: 
		break
		
	print(content)
```

Checking specific value:
```python
line_2 = file.readline('file.txt', 'r')

if 'important' in line_2:
	# Code...
```

> [!IMPORTANT]  **Never Forget** to Close the File
> `file.close()` ensures to properly close the file after reading the contents in the file, as it helps not to waste any resources.
> 
> Or, `file.closed` method can be used to check if the file is closed.

#### Indented Reading (Optional)
`seek()` method reads at specific position in the file (like a cursor). The position is specified in bytes, so you'll need to know the byte offset of the characters you want to read:
```python
file.seek(10) # Move to the 11th byte (0-based index)
```

 `read()` method with an argument specifies the number of characters to read from current position:
```python
characters = file.read(5) # Read the next 5 characters
characters = file.readline(10) # It doesn't read past the end of line  
```

#### Writing Files with `write()`
`write()` method with `w` mode overwrites an existing or a new file. But with `a` (append) mode add new contents to the existing file:
```python
with open('file2.txt', 'w') as write_file:
	# Code...
```


#### Syntax and use cases when working with files in Python:

|Mode|Syntax|Description|
|---|---|---|
|‘r’|`'r'`|Read mode. Opens an existing file for reading. Raises an error if the file doesn't exist.|
|‘w’|`'w'`|Write mode. Creates a new file for writing. Overwrites the file if it already exists.|
|‘a’|`'a'`|Append mode. Opens a file for appending data. Creates the file if it doesn't exist.|
|‘x’|`'x'`|Exclusive creation mode. Creates a new file for writing but raises an error if the file already exists.|
|‘rb’|`'rb'`|Read binary mode. Opens an existing binary file for reading.|
|‘wb’|`'wb'`|Write binary mode. Creates a new binary file for writing.|
|‘ab’|`'ab'`|Append binary mode. Opens a binary file for appending data.|
|‘xb’|`'xb'`|Exclusive binary creation mode. Creates a new binary file for writing but raises an error if it already exists.|
|‘rt’|`'rt'`|Read text mode. Opens an existing text file for reading. (Default for text files)|
|‘wt’|`'wt'`|Write text mode. Creates a new text file for writing. (Default for text files)|
|‘at’|`'at'`|Append text mode. Opens a text file for appending data. (Default for text files)|
|‘xt’|`'xt'`|Exclusive text creation mode. Creates a new text file for writing but raises an error if it already exists.|
|‘r+’|`'r+'`|Read and write mode. Opens an existing file for both reading and writing.|
|‘w+’|`'w+'`|Write and read mode. Creates a new file for reading and writing. Overwrites the file if it already exists.|
|‘a+’|`'a+'`|Append and read mode. Opens a file for both appending and reading. Creates the file if it doesn't exist.|
|‘x+’|`'x+'`|Exclusive creation and read/write mode. Creates a new file for reading and writing but raises an error if it already exists.|

---
## Pandas
An open-source software library for data manipulation and analysis used in Python.

Pandas offer 2 primary data structures:
	1. **DataFrame**: The 2-dimensional and size-mutable data structure with labelled axes *rows & columns*.
	2. **Series**: The 1-dimensional labelled array *a single column or row*.

**Data Import and Export**: Pandas makes easy to read data from various sources *SQL databases, spreadsheets, ...* and export them in these format.

Importing **Pandas** library to access to its pre-built classes and functions:
```python
import pandas as pd

# Now we can access to Pandas' pre-bult classes and functions
# E.g.:
# - read_csv()
# - Series()
# - DataFrame
# ...
```

*csv: comma separated file, df: data frame*

Data frame loading:
```python
print(pd.read_csv(csv_file))
```

Series loading:
```python
data = [12,42,82,4,22,182,11]

print(pd.Series(data))
```

---
Accessing data by label:
```python
print(s[2]) # Access the element with label 2 (value 30)`
```

Accessing by position:
```python
print(s.iloc[3]) # Access the element at position 3 (value 40)`
```

Accessing multiple elements:
```python
print(s[1:4]) # Access a range of elements by label`
```

---
Useful **Pandas**'s functionalities:
- **values**: Returns the Series data as a NumPy array.
- **index**: Returns the index (labels) of the Series.
- **shape**: Returns a tuple representing the dimensions of the Series.
- **size**: Returns the number of elements in the Series.
- **mean(), sum(), min(), max()**: Calculate summary statistics of the data.
- **unique(), nunique()**: Get unique values or the number of unique values.
- **sort_values(), sort_index()**: Sort the Series by values or index labels.
- **isnull(), notnull()**: Check for missing (NaN) or non-missing values.
- **apply()**: Apply a custom function to each element of the Series.

---
Creating **DataFrames** from dictionaries:
```python
pentest_info = {
                'IP': ['192.168.20.1', '192.158.23.1', '192.168.21.3'],
                'Ports': [2,4,1],
                'Admin': ['admin001', 'admin002', 'admin003']
                }

info_df = pd.DataFrame(pentest_info)
```

Accessing rows specifically:
```python
# Show multiple columns with the label
print(info_df[['IP', 'Ports']])

# Show Admin colum and row 2 only
print(info_df[['Admin']].iloc[2])
```

---
#### `loc()` and `iloc()` Functions
`loc()` is label-based that we have to pass the name of row or column.
	`loc[row_label, column_label]`

`iloc()` is indexed-based that we have to pass an integer index to select specific row/column.
	 `iloc[row_index, column_index]`

```python
# Sample Data
sheet = {
        'Student': ['David', 'Samuel', 'Terry', 'Evan'],
        'Age': [27, 24, 22, 32],
        'Country': ['UK', 'Canada', 'China', 'USA'],
        'Course': ['Python', 'C++', 'Machine Learning', 'Web Development'],
        'Marks': [85, 72, 89, 76]
        }

df = pd.DataFrame(sheet)
```

```python
# first row and the first column
df.iloc[0, 0]

# first row and the third column
df.iloc[0, 2]

# first row and salary column
df.loc[0, 'Course']
```

#### Slicing
```python
# slicing with indexes
df.iloc[0:2, 0:3]

# Output:
#   Student  Age
# 0   David   27
# 1  Samuel   24
# 2   Terry   22


# slicing with name
df.loc[0:3, 'Student':'Country']

# Output:
#   Student  Age Country
# 0   David   27      UK
# 1  Samuel   24  Canada
# 2   Terry   22   China
# 3    Evan   32     USA
```

---
## Numpy
A Python library that is commonly used for working with arrays, linear algebra, and matrices. *Numerical Python*: an open-source project.
The array object in **Numpy** is called **ndarray**, it provides lots of supportive functions to easily work with ndarray.

```python
import numpy as np

# Creating numpy array
a = np.array([1,2,3,4])

# Check version
print(np.__version__)
```

We can define steps in slicing by `arr[start:end:step]`.

Using a list as a argument and assign `1000` to corresponding particular indexes:
```python
arr = np.array([1,2,3,4,5,6,7,8,9,10])
select = [0,2,5,7]

arr[select] = 1000
```

```python
# Get the number of elements in an array
arr.size 

# Get the number of dimensions in an array
arr.ndim

# Geting shape (tuple of integers indicating the size of the array in each dimension)
arr.shape
```

Numpy statistical functions:
`arr.mean`: finding mean value
`arr.std`: standard deviation
`arr.max()`: finding the largest value in an array
`arr.min()`: finding the smallest value in an array

Array basic operations:
```python
import numpy as np

a = np.array([1,4,2])
b = np.array([4,3,1])

# Basic operations
np.add(a,b)
np.multiply(a,b)
np.divide(a,b)
np.subtract(a,b)
```

More operations:
```python
# Dot operation
np.dot(a,b) # It does multiplication first, then sum all values.

# Adding Constant (adding a value to each elements in the array)
a + 1 # This adds 1 to each elements in an array

# Calculating the sin of each elements
np.sin(a)
```

```python
# Linspace: returns evenly spaced numbers over a specified interval.
np.linspace(start, stop, num=int)
```

---
#### 2 Dimensional Arrays
This note include useful information about basic operations of matrix.

Getting the information of arrays:
```python
import numpy as np

a = np.array([
    [11,12,13],
    [21,22,23],
    [31,32,33]
])

print(a.size) # number of elements in the array: 9
print(a.ndim) # number of dimenions: 2
print(a.shape) # number of rows and column: (3, 3)
```

Accessing elements:
```python
a[0][1] # first row, and second column
a[0][1:4] # first row, and second to third columns
```

matrix multiplication is *dot operation* `numpy.dot()`

---

# 04.APIs and Data Collection

## Simple APIs
APIs are just like functions, no need to know how it works, just only input and output. An essential type of API is **REST API** that application programs use it access resources via internet.

```python
# Pandas is an API and not even written in Python
import pandas as pd

# When using this constructor, in API lingo this is an "instance"
df = pd.DataFrame({"AA":1234, "AB": 2234})
```

---
## REST APIs
REST APIs follow *Representational State Transfer* architecture style.
It communicate via HTTP message (usually containing a JSON file) that contains what operations we want the **service** or **resource** to perform in the message. Then API returns a response.

Example usage:
```python
from nba_api.stats.static import teams # a REST API
import pandas as pd # For better data visualization or management

# Data Collection Function
def one_dict(list_dict):
    keys=list_dict[0].keys()
    out_dict={key:[] for key in keys}
    for dict_ in list_dict:
        for key, value in dict_.items():
            out_dict[key].append(value)
    return out_dict

# Getting resources from NBA API
nba_teams = teams.get_teams()

# Better data format
df_nba_teams = pd.DataFrame(nba_teams)

print(df_nba_teams)
```

#### Overview of HTTP
*Hyper Text Transfer Protocol* consists of
	- **Scheme** the protocol: `http://`, `https://`...
	- **Internet Address**/**Base URL** the location: `www.github.com`...
	- **Route** the location on web server: `/images/photo.png`...
	
	Example: `http://www.ibm.com/images/photo.png`

My example code requesting:
```python
# importing requests lib for making web requests
import requests as req

# the web location
URL = "https://www.coursera.com"

# requesting 
req_status = req.get(URL)
print(req_status.status_code) # (200: OK)

if req_status.status_code == 200:
    print(req_status.headers)
```

**APIs** are good for automation, efficiency as it provides more functionalities and less human efforts. But, if APIs are poorly integrated, the application program will be vulnerable in data breaches.

#### `RandomUser` API
This section will be using `RandomUser` API to generate placeholders randomly for program testing purposes, such as random emails, users, address, title with these functions:
	- `get_login_sha()`
	- `get_full_name()`
	- `get_password()`
	- `get_username()`

```python
# Importing necessary libs
import pandas as pd # for data management
from randomuser import RandomUser as ru # for random data generation

# random 10 users generation
users = ru.generate_users(1)
df_users = pd.DataFrame(users)

print(df_users)
```

Using `get_somthing()` can generate the required parameters to construct a dataset:
```python
# retrivng each randomly genearted users' email and full names
for user in users:
    print(user, user.get_email(), user.get_full_name())
```

My useful code:
```python
# importing necessary libs
import pandas as pd # for data management
from randomuser import RandomUser as ru # for random data generation

# intializing an empty list
users = []

# randomly generating each users' username, email, and gender
for user in ru.generate_users(4):
	# first, organize a pair of data
    user_detail = {
        "Name": ru.get_username(user),
        "Email": ru.get_email(user),
        "Gender": ru.get_gender(user)
    }
	# then, append that pair into the empty list
    users.append(user_detail)

# formatting the data for better visulization
df_users = pd.DataFrame(users)
print(df_users)
```

Or, alternative code:
```python
import pandas as pd
from randomuser import RandomUser as ru

users = []

for user in ru.generate_users(4):
    user_detail = [ru.get_username(user), ru.get_email(user),ru.get_gender(user)]
    users.append(user_detail)

df_users = pd.DataFrame(users)
df_users.columns = ['Name', 'Email', 'Gender']

print(df_users)

```

---
#### Web Scraping
Beautiful Soup object is a Python library for pulling data out of HTML and XML files.

```python
from bs4 import BeautifulSoup # this module helps in web scrapping.
import requests  # this module helps us to download a web page
```

Scarping all images tags:
```python
for link in soup.find_all('img'):# in html image is represented by the tag <img>
    print(link)
    print(link.get('src'))
```

Working with JSON files:
```python
import json
person = {
    'first_name' : 'Mark',
    'last_name' : 'abc',
    'age' : 27,
    'address': {
        "streetAddress": "21 2nd Street",
        "city": "New York",
        "state": "NY",
        "postalCode": "10021-3100"
    }
}

with open('person.json', 'w') as f:  # writing JSON object
    json.dump(person, f)
```