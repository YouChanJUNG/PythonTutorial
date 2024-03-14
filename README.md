### Python Syntax
## Python Indentation
if 5 > 2:
  print("Five is greater than two!")
  
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 
        
## Python Variables
x = 5
y = "Hello, World!"

## Comments
#This is a comment.
print("Hello, World!")

### Python Comments
## Creating a Comment
#This is a comment
print("Hello, World!")

print("Hello, World!") #This is a comment

#print("Hello, World!")
print("Cheers, Mate!")

## Multiline Comments
#This is a comment
#written in
#more than just one line
print("Hello, World!")

"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")

### Python Variables
Variables 변수는 데이터 값을 저장하기 위한 컨테이너입니다.

## Creating Variables

x = 5
y = "John"
print(x)
print(y)

x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)

## Casting

x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

## Get the Type
x = 5
y = "John"
print(type(x))
print(type(y))

## Single or Double Quotes?
x = "John"
# is the same as
x = 'John'

## Case-Sensitive
a = 4
A = "Sally"
#A will not overwrite a

### Python - Variable Names
## Variable Names
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"

## Camel Case
myVariableName = "John"

## Pascal Case
MyVariableName = "John"

## Snake Case
my_variable_name = "John"

### Python Variables - Assign Multiple Values
## Many Values to Multiple Variables
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)

## One Value to Multiple Variables
x = y = z = "Orange"
print(x)
print(y)
print(z)

## Unpack a Collection
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)

### Python - Output Variables
## Output Variables
x = "Python is awesome"
print(x)

x = "Python"
y = "is"
z = "awesome"
print(x, y, z)

x = "Python "
y = "is "
z = "awesome"
print(x + y + z)

x = 5
y = 10
print(x + y)

x = 5
y = "John"
print(x, y)

### Python - Global Variables
## Global Variables
x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()

x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)


## The global Keyword
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)

x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)

### Python Data Types
## Built-in Data Types
프로그래밍에서 데이터 유형은 중요한 개념입니다.

Text Type:	str
Numeric Types:	int, float, complex
Sequence Types:	list, tuple, range
Mapping Type:	dict
Set Types:	set, frozenset
Boolean Type:	bool
Binary Types:	bytes, bytearray, memoryview
None Type:	NoneType

## Getting the Data Type
x = 5
print(type(x))

## Setting the Data Type
Python에서는 변수에 값을 할당할 때 데이터 유형이 설정됩니다.

### Python Numbers
## Python Numbers
Python에는 세 가지 숫자 유형이 있습니다.

int
float
complex

x = 1    # int
y = 2.8  # float
z = 1j   # complex

print(type(x))
print(type(y))
print(type(z))

## Int
x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))

## Float
x = 1.10
y = 1.0
z = -35.59

print(type(x))
print(type(y))
print(type(z))

x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))

## Complex
x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))

## Type Conversion
x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))

## Random Number
import random

print(random.randrange(1, 10))

### Python Casting
## Specify a Variable Type
x = int(1)
y = int(2.8)
z = int("3")
print(x)
print(y)
print(z)

x = float(1)
y = float(2.8)
z = float("3")
w = float("4.2")
print(x)
print(y)
print(z)
print(w)

x = str("s1")
y = str(2)
z = str(3.0)
print(x)
print(y)
print(z)

### Python Strings
## Strings
#You can use double or single quotes:

print("Hello")
print('Hello')

## Assign String to a Variable
a = "Hello"
print(a)

## Multiline Strings
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)

a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)

## Strings are Arrays
a = "Hello, World!"
print(a[1])

## Looping Through a String
for x in "banana":
  print(x)

## String Length
a = "Hello, World!"
print(len(a))

## Check String
txt = "The best things in life are free!"
print("free" in txt)

txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")

## Check if NOT
txt = "The best things in life are free!"
print("expensive" not in txt)

txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.")

### Python - Slicing Strings
## Slicing
b = "Hello, World!"
print(b[2:5])

## Slice From the Start
b = "Hello, World!"
print(b[:5])

## Slice To the End
b = "Hello, World!"
print(b[2:])

## Negative Indexing
b = "Hello, World!"
print(b[-5:-2])

### Python - Modify Strings
## Upper Case
a = "Hello, World!"
print(a.upper())

## Lower Case
a = "Hello, World!"
print(a.lower())

## Remove Whitespace
a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"

## Replace String
a = "Hello, World!"
print(a.replace("H", "J"))

## Split String
이 split()메서드는 지정된 구분 기호 사이의 텍스트가 목록 항목이 되는 목록을 반환합니다.
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']

### Python - String Concatenation
## String Concatenation
a변수 와 변수를 b변수로 병합 c:

a = "Hello"
b = "World"
c = a + b
print(c)

a = "Hello"
b = "World"
c = a + " " + b
print(c)

### Python - Format - Strings
## String Format
format()문자열에 숫자를 삽입하려면 다음 메서드를 사용하세요.

age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))

인덱스 번호를 사용하여 {0}인수가 올바른 자리 표시자에 배치되었는지 확인할 수 있습니다.

quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))

### Python - Escape Characters
## Escape Character
txt = "We are the so-called \"Vikings\" from the north."
print(txt) 

## Escape Characters
Other escape characters used in Python:
\'	Single Quote	
\\	Backslash	
\n	New Line	
\r	Carriage Return	
\t	Tab	
\b	Backspace	
\f	Form Feed	
\ooo	Octal value	
\xhh	Hex value

### Python - String Methods
## String Methods
Method	Description
capitalize()	Converts the first character to upper case
casefold()	Converts string into lower case
center()	Returns a centered string
count()	Returns the number of times a specified value occurs in a string
encode()	Returns an encoded version of the string
endswith()	Returns true if the string ends with the specified value
expandtabs()	Sets the tab size of the string
find()	Searches the string for a specified value and returns the position of where it was found
format()	Formats specified values in a string
format_map()	Formats specified values in a string
index()	Searches the string for a specified value and returns the position of where it was found
isalnum()	Returns True if all characters in the string are alphanumeric
isalpha()	Returns True if all characters in the string are in the alphabet
isascii()	Returns True if all characters in the string are ascii characters
isdecimal()	Returns True if all characters in the string are decimals
isdigit()	Returns True if all characters in the string are digits
isidentifier()	Returns True if the string is an identifier
islower()	Returns True if all characters in the string are lower case
isnumeric()	Returns True if all characters in the string are numeric
isprintable()	Returns True if all characters in the string are printable
isspace()	Returns True if all characters in the string are whitespaces
istitle()	Returns True if the string follows the rules of a title
isupper()	Returns True if all characters in the string are upper case
join()	Joins the elements of an iterable to the end of the string
ljust()	Returns a left justified version of the string
lower()	Converts a string into lower case
lstrip()	Returns a left trim version of the string
maketrans()	Returns a translation table to be used in translations
partition()	Returns a tuple where the string is parted into three parts
replace()	Returns a string where a specified value is replaced with a specified value
rfind()	Searches the string for a specified value and returns the last position of where it was found
rindex()	Searches the string for a specified value and returns the last position of where it was found
rjust()	Returns a right justified version of the string
rpartition()	Returns a tuple where the string is parted into three parts
rsplit()	Splits the string at the specified separator, and returns a list
rstrip()	Returns a right trim version of the string
split()	Splits the string at the specified separator, and returns a list
splitlines()	Splits the string at line breaks and returns a list
startswith()	Returns true if the string starts with the specified value
strip()	Returns a trimmed version of the string
swapcase()	Swaps cases, lower case becomes upper case and vice versa
title()	Converts the first character of each word to upper case
translate()	Returns a translated string
upper()	Converts a string into upper case
zfill()	Fills the string with a specified number of 0 values at the beginning



