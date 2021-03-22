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

