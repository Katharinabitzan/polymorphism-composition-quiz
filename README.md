# polymorphism-composition-quiz

#Polymorphism

##What does the word 'polymorphism' mean?

The word ‘polymorphism’ is defined as the “condition of occuring in several different forms”.

##What does it mean when we apply polymorphism to OO design? Give a simple Java example.

 In programming, this means that an object can occur or be presented in different forms other than its own class. For example, a class named “Car” can implement the interface “IDrive”, and can then occur as an instance of the interface or as an instance of the Car class. In other words, it is the concept that objects of different types can be accessed through the same interface, although each type can provide its own implementation of this interface.

##What can we use to implement polymorphism in Java?

Interfaces can be used to implement polymorphism in Java. Inheritance can also be used to implement polymorphism in java, and some writers argue that because all objects extend the class Object, all objects are already polymorphic.

There are two types of polymorphism: 

1. Static polymorphism: This is when multiple methods within the same class are implementeted that take different parameters either in number or type of parameter,. This is method overloading, and usually overloaded methods provide different but similar functionality.

2. Dynamic polymorphism: This is when a method of a superclass is overriden by the subclass. 

##How many 'forms' can an object take when using polymorphism?

Unlimited. 

##Give an example of when you could use polymorphism.

Eg. when creating a car rental app. Each vehicle would have a different class, but would implement the same interface: IBookable.  A customer would not have to interact with the classes themselves when performing methods such as booking, but instead could interact with the IBookable interface. 

#Composition

##What do we mean by 'composition' in reference to object-oriented programming?

In OO programming, composition describes a class that references one or more objects of other classes in instance variables. It is a way of expressing relationships between objects, “has-a” relationships.

##When would you use composition? Provide a simple example in Java.

When modelling a volleyball team for example, there may be different classes exisiting for the different positions eg. “Setter” class, “Spiker” class.  There might also be a class “Substitute Player”. All of these would have an interface “IPlayable”, and so the volleyball team can simply have a collection of Iplayable objects rather than individual classes, and without the need for using the superclass.

##What is/are the advantage(s) of using composition?

The advantage of composition is that it allows programmers to reuse code by modeling an “is-a” association eg. an Object is another Object, similarly to inherhitance, but without the rigidity of inherhitance. Therefore code can be reused but also differentiated. This allows for stronger encapsulation and makes it easier to maintain.

##When an object is destroyed, what happens to all the objects it is composed of?

When an object is destroyed, the objects that it is composed or contained by that object are also destroyed. 
