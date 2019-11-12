# Design patterns from gang of four

Providing solutions to common software design problems are known as **Design Patterns**. Gang of four has explained about twenty-three design patterns which includes

**Creational Patterns**

- Abstract factory
- Builder
- Factory Method
- Prototype
- Singleton

**Structural Patterns**

- Adpater
- Bridge
- composite
- Decorator
- Facade
- Flyweight
- Proxy

**Behavioural Patterns**

- Chain of responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- Observer
- State
- Strategy
- Template Method
- Visitor

Reference <http://www.blackwasp.co.uk/gofpatterns.aspx>

# Objects 

**Objects** are single entity that encapsulate variables and functions. These variables and functions are obtained by objects through class.

Below is a very basic class:

     class MyClass:
    variable = "apple"
    def function(self):
        print("This is a message inside the class.")

To assign this class to an object we will do,

     class MyClass:
    variable = "apple"
    def function(self):
        print("This is a message inside the class.")
    myobjectx = MyClass()

To access the object variable :

    class MyClass:
    variable = "apple"
    def function(self):
        print("This is a message inside the class.")
    myobjectx = MyClass()
    myobjectx.variable

Reference <https://www.learnpython.org/en/Classes_and_Objects>

# Exception

During the execution of the program if an error occurs it is known as **Exception**. An exception generated by python can be handled when an error occurs to avoid the program to crash.

If you feel that your code is gonna produce an error then you can use exception handling.

**Exception Error:**

- **IO Error** : If the file cannot be opened.

        except IOError:
        print('An error occurred trying to read the file')

- **Import Error** : When the module is not found by the python.

        except ImportError:
        print('NO module found')

- **Value Error** : When a function receives an argument which has an inappropriate value but the right type.

        except ValueError:
        print('Non-numeric data found in the file')

- **Keyboard Interupt** : When the interupt key (Control-C or Delete) is hit.

        except KeyboardInterrupt:
        print('You cancelled the operation')

- **EOF Error** : When the built-in function (input() or raw_input()) hits the end-of-file condition without reading the data.

        except EOFError:
        print('Why did you do an EOF?')

Reference <https://www.pythonforbeginners.com/error-handling/exception-handling-in-python>

# Factory

Factory pattern is one of the best ways to create an object and it comes under the creational patterns list category. The method is called by the user in such a way that a string is passed and the return value as a new object is implemented through factory method. When a string is passed through a method it determines the type of object that is used in factory method.

    class Button(object):
      html = ""
      def get_html(self):
        return self.html
    class Image(Button):
      html = "<img></img>"
    class Input(Button):
      html = "<input></input>"
    class Flash(Button):
      html = "<obj></obj>"
    class ButtonFactory():
      def create_button(self, typ):
      targetclass = typ.capitalize()
      return globals()[targetclass]()
    button_obj = ButtonFactory()
    button = ['image', 'input', 'flash']
    for b in button:
       print button_obj.create_button(b).get_html()

The *button* is used to create the html tags and associated html page. The logic of the code is not accessed by the client. The output represents the creation of HTML page.

![Factory](https://www.tutorialspoint.com/python_design_patterns/images/factory_pattern.jpg)

Reference <https://www.tutorialspoint.com/python_design_patterns/python_design_patterns_factory.htm>

# Extend class

The class can be extended with the help of **Inheritance**. When a class uses code constructed within another class it is known as inheritance. In terms of biology, a child inherits certain traits from their parent.

Classes called *child classes* or *subclasses* inherit methods and variables from *parent classes* or *base classes*.

Since the Child subclass is inheriting from the Parent base class, the Child class can reuse the code of Parent, allowing the programmer to use few lines of code and also decrease redundancy.

Reference <https://www.digitalocean.com/community/tutorials/understanding-class-inheritance-in-python-3>

# Reading Files

You can create .txt file from Python and can also call .txt file in a "read mode"(r).

1 - Open file in *read mode*

     f=open("pia.txt", "r")

2 - The mode function in the code can be used to check whether the file is in open mode. If it shows yes then we can proceed.

     if f.mode == 'r':

3 - Use f.read to read file data and store it in variable content

	contents =f.read()

4 - print contents

Reference <https://www.guru99.com/reading-and-writing-files-in-python.html#3>
