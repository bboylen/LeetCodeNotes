# Object Oriented Programming
The most popular programming paradigm. Relies on the concept of **classes** and **objects**. 

A class is an abstract blueprint used to create specific, concrete objects. Often represent categories like a `Dog` or `Cat` that share **attributes**. Classes define what attributes an instance of this type will have, but not the value.

Classes also contain functions called **methods** that are only available to objects of that class. 

Class templates are used as a blueprint to create individual **objects**. These represent specific examples of the abstract class, like `myCar` or `goldenRetriever`.

### Benefits of OOP
- OOP models complex things as reproducible, simple structures
- Reusable, OOP objects can be used across programs
- Allows for class-specific behavior through polymorphism
- Easier to debug, classes often contain all applicable information to them
- Secure, protects information through encapsulation

## Four Pillars of OOP
### Abstraction
Abstraction is the concept of object-oriented programming that "shows" only essential attributes and "hides" unnecessary information. Decouples user from underlying **implementation**. Not to be confused with encapsulation which is used to hide data essentially. Basically, abstraction means simple things like objects, classes and variables represent more complex underlying code and data.

### Encapsulation
Restrict access of properties and methods of class to whatever is calling. Objects can not access this state directly, instead, they can only invoke a list of public functions. In order to communicate with the object, you need to utilize the methods provided.

### Inheritance
The ability of one object to acquire some or all of another object. Reusability is a major advantage. "Is-a-type-of" relationship

### Polymorphism
Gives a way to use a class exactly like its parent so there is no confusion with mixing types. Each child subclass keeps its own functions/methods as they are.