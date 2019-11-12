# Design patterns from gang of four

Providing solutions to common software design problems are known as Design Patterns. Gang of four has explained about twenty-three design patterns which includes

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

Reference < http://www.blackwasp.co.uk/gofpatterns.aspx >

# Objects 

**Objects** are single entity that encapsulate variables and functions. These variables and functions are obtained by objects through class.

Below is a very basic class:

     class MyClass:
    variable = "blah"
    def function(self):
        print("This is a message inside the class.")

To assign this class to an object we will do,

     class MyClass:
    variable = "blah"
    def function(self):
        print("This is a message inside the class.")
    myobjectx = MyClass()

To access the object variable :

    class MyClass:
    variable = "blah"
    def function(self):
        print("This is a message inside the class.")
    myobjectx = MyClass()
    myobjectx.variable

Reference <https://www.learnpython.org/en/Classes_and_Objects>