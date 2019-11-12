
## Class: 

Being object oriented language almost all the code is implemented using a special construst called classed.Classed usuallu use to keep related things together.

What is class?
A class is a code template for creating objects. Objects have member variables and have behaviour associated with them. In python a class is created by the keyword class.

An object is created using the constructor of the class. This object will then be called the instance of the class. In Python we create instances in the following manner

How to create a class?

Below is an exampls of class with no functionalities

>>> class Birds:
...     pass
... 
>>> birds = Birds()
>>> print(birds)

Classes are of no use unless it has functionalities. Functionalities can be set by using attributes and methods. For example, you can define a class Snake, which has one attribute name and one method change_name. The method change name will take in an argument new_name along with the keyword self.

Example:
Setting 'name' attribute to a class:
>>> class Birds:
...     name = "python"

>>> instantiate the class Snake and assign it to variable snake
>>> birds = Birds()

>>> access the class attribute name inside the class Snake.
>>> print(birds.name)
python

Setting method of the class:

>>> class Birds:
...     name = "python"
...     
...     def change_name(self, new_name): # note that the first argument is self
...         self.name = new_name # access the class attribute with the self keyword
...

Reference:
https://www.hackerearth.com/practice/python/object-oriented-programming/classes-and-objects-i/tutorial/



## Method:

Python Method

Method is called by its name, but it is associated to an object (dependent).
A method is implicitly passed the object on which it is invoked.
It may or may not return any data.
A method can operate on the data (instance variables) that is contained by the corresponding class
Basic Method Structure in Python :

 Basic Python method  
class class_name 
    def method_name () : 
        ...... 
        # method body 
        ......  


## Unit testing:

Unit testing is basic level of testing where individual part of the module is tested.This is used to validate that each unit of the software performs as designed.
The unittest test framework is python’s xUnit style framework.

Basic Test Structure :
unittest defines tests by the following two ways :

Manage test “fixtures” using code.
test itself.

import unittest 
  
class SimpleTest(unittest.TestCase): 
  
     Returns True or False.  
    def test(self):         
        self.assertTrue(True) 
  
if __name__ == '__main__': 
    unittest.main()


Outcomes Possible :
There are three types of possible test outcomes :

OK – This means that all the tests are passed.
FAIL – This means that the test did not pass and an AssertionError exception is raised.
ERROR – This means that the test raises an exception other than AssertionError.


Basic terms useful for unit testing:
Basic terms used in the code :

assertEqual() – This statement is used to check if the result obtained is equal to the expected result.
assertTrue() / assertFalse() – This statement is used to verify if a given statement is true or false.
assertRaises() – This statement is used to raise a specific exception.

Reference:
https://www.geeksforgeeks.org/unit-testing-python-unittest/


## CSV files:

A CSV file (Comma Separated Values file) is a type of plain text file that uses specific structuring to arrange tabular data. Because it’s a plain text file, it can contain only actual text data—in other words, printable ASCII or Unicode characters.

Example:
column 1 name,column 2 name, column 3 name
first row data 1,first row data 2,first row data 3
second row data 1,second row data 2,second row data 3
...

Reference:
https://realpython.com/python-csv/


## Don't repeat yourself

The DRY or “Don’t Repeat Yourself” principle is a software development practice aimed at reducing repetition of information. 
Example: name = 'Allen'
people_i_like = ['Allen', 'Kiyara', 'Yana']
if name in people_i_like:
    print 'yay!'
