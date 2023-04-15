# IMPORTANT DEFINITIONS AND CONCEPTS
+ Aliasing, i.e., two variables are bound to the same address.
> this is when two pointers have the same pointer 
> changing one changes the other
+ Programming language categories: Imperative, + Object-oriented,  Functional and Logic programming languages.
> ![](https://cdn.discordapp.com/attachments/328403690383867906/1096748121037492325/what-is-imperative-programming1.png)

+ Keywords vs. reserved words. A keyword is a word in a programming language that has a special meaning in certain contexts. A reserved word cannot be used as a name for a variable.
> The keywords const and goto are reserved, even though they are not currently used
+ Attributes of a variable: Name, Address, Value, Type.
>
+ Static variables cannot implement recursion.
>
+ Arrays: Static vs. Fixed-stack dynamic vs. Stack-dynamic vs. Fixed heap-dynamic vs. Heap-dynamic.
>
+ Reference types vs. pointers, i.e., pointers allow arithmetic operations on them; reference type variables do not.
>
+ Dangling pointers, i.e., a pointer that contains an address that has been deallocated.
>
+ Activation record of a subprogram. It needs to include local variables, parameters, dynamic link, and return address.
>

+ Abstract data types – A tool for data abstraction
>
+ Friend classes. Some languages do not have this concept because it can be implemented by alternative means. For example, Java provides packages and package scope.
>
+ Assignment for stack-dynamic objects. This is problematic because the variable a might not have enough space to store an object that is of a subclass.
>
+ Dynamically bound methods in languages. Default vs. explicit language construction. For example, C++ requires that the method is declared virtual.
>
+ Key features of an object-oriented languages. Abstract data types, inheritance, and dynamic binding of method calls to methods.
>
+ Virtual method table (vtable). It contains pointers to all dynamically bound methods.
>
+ Lazy evaluation. It means that an expression is evaluated if and only if its value is needed to compute the overall result.
>
+ Java threads. You create a Java thread by extending the Thread class, override run(), and call start().
>

+ Method synchronization in Java. A synchronized method that is called through a specific object must complete its execution before any other synchronized method can run on that object.
>
+ Referential transparency. An expression is called referentially transparent if it can be replaced with its corresponding value (and vice-versa) without changing the program's behavior, i.e., if the value of the expression is independent of the context it is executed in.
>
+ Polymorphic functions. The function has one implementation that works for all types.
>
+ Overloaded functions. The function works for a lot of (but not necessarily all) types but has a different implementation each time.
>
+ Underlying computational model of imperative languages. Von Neumann model.
>
+ Underlying computational model of functional languages. Lambda calculus.
>
+ Underlying computational model of logic languages. First-order predicate calculus and resolution.
>
+ Cut operator in logic languages. The purpose of the cut is to allow the programmer to make programs more efficient by cutting whole branches in the search tree of the proof attempt.
>
---