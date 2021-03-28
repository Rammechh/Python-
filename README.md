# Python
Python Django Project
# Property Searching Project [Udemy Course link](https://cognizant.udemy.com/course/python-django-dev-to-deployment/l)
## Functionalities
  + Home - Latest Listings in Database will be listed in front page, Search Listing
  + About - Realtors are added, Seller of the month
  + Featured Listing - All property details, realtors for listing
  + Register - for new users
  + Login Page - For Sign in
  + User Dashboard
  + Admin Login - Publish, unpublish images, Realtors info, all site administration
---
## [Django](https://www.djangoproject.com/)
  + Django is a high-level Python Web framework
  + Used for Web development, Utilities, Automation, Machine Learning, data Analysis
  + Can use any db's(SQL, MongoDB, etc.,), Post grades (Powerful Relational Database) used in this project.
  + Each piece of functionality on website created called 'app'.
---
## Resource Links
  + [Complete Code Repo:](https://github.com/bradtraversy/btre_project)
  + [Python Download:](https://www.python.org)
  + [Django Official Site & Docs:](https://www.djangoproject.com)
  + [Visual Studo Code:](https://code.visualstudio.com)
  + [Download Git:](https://git-scm.com)
  + [Gitignore.io:](https://www.gitignore.io)
  + [Digital Ocean:- $10 free](https://m.do.co/c/5424d440c63a)
  + [Django Cheat Sheet:](https://gist.github.com/bradtraversy/0df61e9b306db3d61eb24793b6b7132d)
  + [Django Deploy Instructions:](https://gist.github.com/bradtraversy/cfa565b879ff1458dba08f423cb01d71)
  + [Original Deploy Article:](https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-18-04)
  + [Virtual Env Setup Doc:](https://docs.python.org/3/library/venv.html)
---
## VS Code
  + Install VS code
  + Set Environmental Varibales => View Advanced system setting in pc -> Advanced tab -> Environment Varibales -> Select Path(Edit) add New -> C:\Users\ram75\AppData\Local\Programs\Python\Python39\Scripts and C:\Users\ram75\AppData\Local\Programs\Python\Python39
  + Install Python in Extension of VS Code
  + Type 'python' in cmd to check.
  + Downloaded Sandbox starter files from course also attached here.
  + To Run in VS Code => python3 filename.py in terminal
  + Command palette => **Ctrl + Shift + p** -> select 'Python select Interpreter' -> select python 3. versions
---
## Python Fundamentals
  + **Comments**
      * Comments do not execute, when you run a program you will not see any indication of the comment there. Comments are in the source code for humans to read, not for computers to execute
      * '#' Single line Comment, 3 single quotes(''') or 3 double quotes(""") for multi line comment
      * Variables rules same as other language 1) Variable names are case sensitive (name and NAME are different variables) 2) Must start with a letter or an underscore 3) Can have numbers but can not start with one.

  + **Assignments and Print**
      *  1)) a=1(Int) 2) b=1.5(Float) 3) name='Ram'(String) 4) py_easy=True (Boolean Start with Caps 'T', 'F')
      * Multiple assignment -->  a,b,name,py_easy = (1, 1.5, 'Ram', True)
      * print(a, b, name, py_easy)
    
  + **Basic Math**
      * x=a+b
      * **Check Type** => print(type(x)) -> output: <class 'float'>
      * **Casting** => 1)a=str(a) 2)b=int(b)

  + **String**
      * name='Ram'
      * age=23
      * print('Hi, I am ' +name + ' and my age is' + str(age))
      * '+' --> Used for concatenation
      
  + **String Formatting**
      * 1) %-formatting --> It is verbose and leads to errors, like not displaying tuples or dictionaries correctly
 ___
      * name = "Ram"
      * age = 23
      * print("Hello, %s. You are %s." % (name, age))
      * Output : 'Hello Ram. You are 23.'
 ___
        2) #2: str.format() --> Code using str.format() is much more easily readable than code using %-formatting
 ___
      print("Hello, {}. You are {}.".format(name, age))
      print("Hello, {1}. You are {0}.".format(age, name))
 
      person = {'name': 'Ram', 'age': 23}
      print("Hello, {name}. You are {age}.".format(name=person['name'], age=person['age']))

      person = {'name': 'Ram', 'age': 23}
      print("Hello, {name}. You are {age}.".format(**person))
      
      **Output** : Hello, Ram. You are 23
___
        3) #3 F or f strings -->Also called “formatted string literals,” f-strings are string literals that have an f at the beginning and curly braces. for better readability
___
      print(f"Hello, {name}. You are {age}.")
      print(F"Hello, {name}. You are {age}.")
___
      * s="hello World" 

### Capitalize first letter
print(s.capitalize())

### Make all uppercase
print(s.upper())

### Make all lower
print(s.lower())

### Swap case
print(s.swapcase())

### Get length
print(len(s))

### Replace
print(s.replace('world', 'everyone'))

### Count
sub = "h"
print(s.count(sub))

### Starts with
print(s.startswith('hello'))

### Ends with
print(s.endswith('d'))

### Split into a list
print(s.split())

### Find position
print(s.find('r'))

### Is all alphanumeric
print(s.isalnum())

### Is all alphabetic
print(s.isalpha())

### Is all numeric
print(s.isnumeric())

---
## Lists
  + [Lists_In_depth](https://www.codementor.io/@sheena/python-lists-in-depth-lrtmk7w4q)
  + Lists are used to store multiple items in a single variable. Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
  + Index starts from 0 to n-1. To fetch last index can use a[-1].
  + Slice operator will be helpful a[0:3:1] can be used to fetch values accordingly. [start: end :step] --> [::-1] will fetch elements in reverse order.
  + **append** adds an element to the end of the list -> l.append('a')
  + **extend** is used to concatenate lists 
      * l=['a'] l.extend([1,2,3,4,5]) print(l) output: ['a', 1, 2, 3, 4, 5]
  + **in** is used to check if an element exists inside a list --> 'a' in l (True),  **not in** does the opposite --> 'b' not in l (True)
  + **sort()** basically works with the list itself. It modifies the original list in place. The return value is None. l.sort() original list will be changed. print(l.sort(reverse = True) 
  + **sorted()** works on any iterable that may include list, dictionary and so on. It returns another list and doesn't modify the original list. Sorted(l) original list will not be changed. print(sorted(L, reverse = True))
  + ReverseList --> l.reverse()
---
## Tuples
  + A Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
  + Can create using constructor a=tuple((1,2,3)) or a=(1,2,3)
  + Item deletin is not possibe. del a (will delete tuple)
---
## Sets
  + A Set is a collection which is unordered and unindexed. No duplicate members. s = {1,2,3}
  + Since it is unordered, you can't access elements by index.  s[1] -> will throw error ('set' object does not support indexing)
---
## Dictionary
  + A Dictionary is a collection which is unordered, changeable and indexed. No duplicate members.
  + Dictionaries map keys to values, You access individual values by key, not by index.
  + Dictionaries, like lists, are mutable
  + Using Constructor -> person = dict(first_name='John', last_name='Doe',age=30) or person = {'first_name': 'John', 'last_name': 'Doe', 'age': 30 }
  + Access keys & values -> print(person.keys()), print(person.values()) 
  + To get all items -> print(person.items())
---
## Functions
  + A function is a block of code which only runs when it is called. 
  + In Python, we do not use parentheses and curly brackets, we use indentation with tabs or spaces
  ___
def getSum(num1, num2):
  total = num1 + num2
  return total

numSum = getSum(2, 3)
  ___
