# CS4330 Final
Aaron Henry, Jack Murphy, and Landen Eagan

# Why was the language created?
# What problems was the language trying to address?
    1. Java- java tries to be a large scale OO language that everyone uses and can be used in multiple applications. It was designed to have as few implementation dependencies as possible. It is intended to let application developers “write once, run anywhere”.
    
    2. Swift- Swift tries to fix issues of many OOP languages and also offer apple developers a language optimized for the platform they are developing for.

# Is the language a reaction to a previous language or a replacement for another language?
    1. Java - java is more of an upgrade but The language derives its syntax from C and C++, but it has fewer low-level facilities than either of the
    
	2. Swift - This is a replacement of Objective-C, Swift tries to take its core concepts. It tries to make is safer and also line up with the Apples Cocoa framework (touch frameworks).

# Instance reference name in data type (class) this? Self?
    1. Java - uses 'this', it is used a lot in setter methods to disambiguate variable references. also when you want to pass the current class instance as an argument to a method.
    
    2. Swift - uses 'self' but they recomend that you do not use 'self'  when possible.
# Properties
# Getters and setters…write your own or built in?
	1. Java- in java you have to build your own getters and setters
	2. Swift- in swift you have to create your own getters and setters
# Backing variables?
	1. Java- allows backing variables
	2. Swift- backing is not used directly
# Computed properties?
	1. Java - allows computed properties
	2. Swift - allows computed properties

# Comparisons of references and values How are values compared? (i.e. comparing two strings)
	1. Java- there are “compare” interfaces that take the strings and compare them, als you can use the basic == or != to compare the value.
	2. 
	2. Swift-  you can compare with == and != but you can also use the equatable protocol.


# Null/nil references Does the language have features for handling null/nil references?
	1. Java- null, a special null value is assigned to the reference of the variable.
	2. Swift  - nil, swift uses optional to handle nils, basically if its nil it looks over that part as if its not there.

# Procedural programming, Does the language support procedural programming?
	1. Java - Yes
	2. Swift - Yes 
# Functional programming, Does the language support functional programming?
	1. Java - yes, this can be seen in lambdas.
	2. Swift - it is not fully functional but it takes parts of functional programing.

# Name spaces, How are name spaces implemented? , How are name spaces used?
    1. Java- Java uses packages as it’s namespace. These packages are more private areas that may hold things such as classes. This way they can be grouped together conveniently and they won’t collide with other identically named classes in different packages.
    
    2. Swift- Every module represents a namespace in Swift. This means you cannot have two classes with the same name in one target. This way, the two class names will not collide. You could also make a wrapper for the classes by nesting them in different structs.
# Types, What types does the language support?
    1. Java- Java supports boolean, byte, char, short, int, long, float, and double.

    2. Swift- Swift supports bool, char, unsigned char, short, unsigned short, int, unsigned int, long, unsigned long, long long, unsigned long long, wchart_t, char16_t, char32_t, float, and double.

# Are both reference and value types supported?
    1. Java- Java supports value and reference types.
    2. Swift- Swift supports value and reference types.
# Can new value types be created?
    1. Java- No, you may only use the preset primitive data types.
    2. Swift- No, you many only use the preset primitive data types.
# Inheritance / extension
    1. Java- In Java classes can be derived from other classes. This means that they inherit the fields and methods from the original classes. This is done using the “extends” keyword.
    2. Swift- In Swift classes can also be derived from other classes. This is done using the “:” symbol.
# Memory management, How is it handled? How does it work?
    1. Java- In Java objects reside in an area called the heap. The new objects are placed in what’s called the “nursery” where the are more easily found. Eventually they will be moved to the old space by the garbage collector to make more room in the nursery for new objects. The reason behind this is freeing short lived objects is much faster than the old, long lived objects. Then eventually when the old space is full, it will be freed by the garbage collector.

    2. Swift- Swift uses automatic reference counting to manage it’s memory. Every time you create a new instance of a class, memory will be allocated for that instance. Then once the instance is no longer needed it will be freed.
# Garbage collection?
    1. Java- Java has a garbage collector.
    2. Swift- Swift does not have a garbage collector.
# Automatic reference counting?
    1. Java- Java does not use automatic reference counting.
    2. Swift- Swift does use automatic reference counting.
# Errors and exception handling
    1. Java- Java handles it errors in three categories. They are user error, programmer error, and failure of physical resources. These will return error codes that may be used to find the problem.  

    2. Swift- Swifts errors are represented by values of types that conform to the Error protocol. Then surrounding code will be responsible for using the error code to correct the problem, try an alternative approach, or inform the user of failure.
# Singleton, How is a singleton implemented?
    1. Java- A singleton is implemented by using the getInstance() method. This will always either create an instance initially or return the created instance after if has already been created.

    2. Swift- They can be implemented by defining a global variable, but this is unsafe. The proper way to do it is to use a static property and to have a private initializer.

# Can it be made thread-safe?
    1. Java- Yes it can be made thread safe. One example of how to do this is creating the instance variable at the time of class loading.
    2. Swift- Yes it can be made thread safe by using the second method described in how a swift singleton is implemented.
 
# Unique features
    1. Java being an older language maintains fewer and fewer unique features every day, but it does gain new open source libraries everyday, adding new features to the language. 

    2. Swift, on the other hand, is a new language and has new features with it. Swift has added closures unified with function pointers, tuples and multiple return values, generics, fast and concise iteration over a range, structs that support methods, extensions, protocols, and functional programming patterns.
# Classes
    1. Java- When defining a class in Java you require an access modifier. Java also requires your entire program to run within a class. When creating an instance of a class in java you are required to use “new” before the type. When initializing an object in Java values can be assigned either to zero, to a default value, or assigned within a constructor which is called at the moment of creation. Objects in Java are automatically destructed by the garbage collector.

    2. Swift-No access modifier required. Does not require your program to run within a class. When creating an instance of a class in Swift you do not need to include anything before the type. When initializing an object in Swift nearly all of the same is true as is in Java, the syntax only changes from being “nameOfClass(parameters){}” to “init(parameters){}”. Swift also allows for multiple inits to be present. Swift also automatically destructed through automatic reference counting, but you can add an initializer to your code to remove unused objects.
# Interfaces/protocols
    Swift implements nearly all of the features of a Java interface with a few exceptions
    Swift protocols can specify properties that must be implemented
    Swift protocols need to deal with value/reference through the use of the “mutating” keyword
    You can combine protocols at any point with the “protocol<>” keyword.
    Swift protocols can be implemented by structs and classes.
# Reflection
    1. Java -  Reflection makes it possible to inspect classes, interfaces, fields and methods at runtime, without knowing the names of the classes

    2. Swift - in languages like swift Reflection usually isn’t used, but with swift you are allowed limited things such as it allows you to look at an objects properties without modifying them. 

# Lambda expressions, closures, or functions as types
#### Closures(Swift) vs. Lambdas(Java)
    Closures may capture non constant variables
    Closures support shorthand argument names
#### Functional type(Swift) vs. functional interfaces(Java)
    Functional interfaces allow declaration of additional methods (e.g. java.util.Comparator that defines a bunch of methods for comparator building)

# Implementation of listeners and event handlers
    1. Java - they are also created in classes, you need to link them to an object (usually visible i.e a button), this can be done with javaFX.

    2. Swift - Uses cocoa to handle all of the events and listeners, they can be made in “Event classes” 

# Multithreading
    1. Java - Java allows for users to create as many threads as need be through the use of the runnable interface which contains the run() method. By using this you can then create objects implementing that method within a thread.

    2. Swift - Swift allows for asynchronous code execution which basically acts as multithreading.



