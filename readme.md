# **Examples on "Strings" Methods In Python**
---
## Python String `Capitalize()`
This string method will return a copy of the string after capitalizing its first character. The rest of the characters will remain lower case. 

syntex=>string.Capitalize()





```python
a = "skill disk"
print(a.capitalize())
```
```
Output:
Skill disk
```         
## Python String `count()`
The count() method returns the number of times a specified value appears in the string.

syntex=>string.count(value, start, end)

* *value*-Required. A String. The string to value to search for
* *start*-Optional. An Integer. The position to start the search. Default is 0
* *end*-Optional. An Integer. The position to end the search. Default is the end of the string 
```
word = "hee mmm hee mmm" 
x=word.count('hee',3,15)
print(x)
``` 
```
Output:
1
```
```

word = "hee mmm hee mmm" 
x=word.count('hee')
print(x)
```
```
Output:
2
```
## Python String `find()`
The find() method finds the first occurrence of the specified value.

The find() method returns -1 if the value is not found.
Syntax=>string.find(value, start, end)
* *value*	Required. The value to search for
* *start*	Optional. Where to start the search. Default is 0
* *end*	Optional. Where to end the search. Default is to the end of the string
```
word_pos = "Hello, welcome to python."

x = word_pos.find("welcome")

print(x)
```
```
Output:
7
```
```
txt = "Hello, welcome to skill disk."

x = txt.find("e", 5, 10)

print(x)

```
```
Output:
8

```
## Python String `index()`
The index() method is almost the same as the find() method, the only difference is that the find() method returns -1 if the value is not found.wher as index method rises excepetion
```
txt = "Hello, welcome to my world."

print(txt.find("q"))
print(txt.index("q"))

```
```
Output:
-1
Traceback (most recent call last):
  File "demo_ref_string_find_vs_index.py", line 4 in <module>
    print(txt.index("q"))
ValueError: substring not found 
```
## Python String `format()`
The format() method formats the specified value(s) and insert them inside the string's placeholder.

The placeholder is defined using curly brackets: {} 

The format() method returns the formatted string.
```
a=20
b='my name is j and i am {}'
print(b.format(a))
```
```
output:
my name is j and i am 20
```
```
a=("i am learning python {} in {}")
b=3.9
c='skill disk'
print(a.format (b,c))

```
```
output:
i am learning python 3.9 in skill disk
```
## Python String `isupper()`
The isupper() method returns True if all the characters are in upper case, otherwise False.
**Note**:
Numbers, symbols and spaces are not checked, only alphabet characters.

Syntax=>string.isupper()

```
a = "Hello python!"
b = "hello #1"
c = "MY NAME IS J"

print(a.isupper())
print(b.isupper())
print(c.isupper())
```
```
Output:
False
False
True
```
## Python String `islower()`
The islower() method returns True if all the characters are in lower case, otherwise False.
Syntax=>string.islower()
```
a = "Hello world!"
b = "hello #1"
c = "mynameisj "

print(a.islower())
print(b.islower())
print(c.islower())
```
```
output:
False
True
False
```
## Python String `isalpha()`
The isalpha() method returns True if all the characters are alphabet letters (a-z).
Syntax=>string.isalpha()
```
a='sam'
print(a.isalpha())
```
```
output:
True
```
```
a='sam12'
print(a.isalpha())
```
```
output:
False
```
## Python String `isalnum()`
The isalnum() method returns True if all the characters are alphanumeric, meaning alphabet letter (a-z) and numbers (0-9).
Syntax=>string.isalnum()
```
a='sam12'
print(a.isalnum())
```
```
output:
True
```
```
a='sam12#'
print(a.isalnum())
```
```
output:
False
```
## Python String `upper()`
converts string into upper case
syntax=>isupper() 
```
a = "Hello sam"
x = a.upper()
print(x)
```
```
output:
HELLO SAM
```
## Python String `lower()`
```
a = "HELLO SAM"
x = a.lower()
print(x)
```
```
output:
hello sam
```
## Python String `replace()`
The replace() method replaces a specified phrase with another specified phrase.
syntax=>string.replace(oldvalue,newvalue,count)
```
a=('daic,traic,diode,zenerdiode ')
b=a.replace('aic','ooo',1)
print(b)
```
```
output:
dooo,traic,diode,zenerdiode
```
```
a=('daic,traic,diode,zenerdiode ')
b=a.replace('aic','ooo',1)
print(b)

```
```
output:
dooo,trooo,diode,zenerdiode 
```
## Python String `strip()`
The strip() method removes any leading (spaces at the beginning) and trailing (spaces at the end) characters (space is the default leading character to remove)
syntex=>string.strip(character)

```
txt = ",,,,,rrttgg.....banana....rrr"
x = txt.strip(",.grt")
print(x)
```
```
output:
....banana....
```
## Python String `rstrip()`

syntex=>string.rstrip(character)
```
txt = ",,,,,rrttgg.....banana....rrr"
x = txt.rstrip(",.grt")
print(x)
```
```
output:
,,,,,rrttgg.....banana....
```
## Python String `lstrip()`

syntex=>string.rstrip(character)
```
txt = ",,,,,rrttgg.....banana....rrr"
x = txt.lstrip(",.grt")
print(x)
```
```
outpt:
.....banana....rrr
```
## Python String `split()`
The split() method splits a string into a list.
syntax=>string.split(separator, maxsplit)

*separator*	Optional. Specifies the separator to use when splitting the string. By default any whitespace is a separator

*maxsplit*	Optional. Specifies how many splits to do. Default value is -1, which is "all occurrences"


```
txt = "apple#banana#cherry#orange"
x = txt.split("#")
print(x)
```
```
output:
['apple', 'banana', 'cherry', 'orange']
```
```
txt = "apple#banana#cherry#orange"
# setting the maxsplit parameter to 1, will return a list with 2 elements!
x = txt.split("#", 1)
print(x)
```
```
output:
['apple', 'banana#cherry#orange']
```  
## Python String `splitlines()`
The splitlines() method splits a string into a list. The splitting is done at line breaks.
```
a=('byappanhalli\ngreen line')
b=a.splitlines()
print(b)
```
```
output:
['byappanhalli', 'green line']
```
## Python String `swapcase()`
The swapcase() method returns a string where all the upper case letters are lower case and vice versa.
syntax=>string.swapcase()
```
a="my name IS SAM"
b=a.swapcase()
print(b)
```
```
output:
MY NAME is sam
```
