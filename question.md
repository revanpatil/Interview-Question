1. Explain system.out.println()
2. What is variable length arguments ?
Ans : In Java, variable-length arguments allow a method to accept an arbitrary number of arguments of the same type. They are represented using an ellipsis (...) after the type in the method parameter list. Here's an example:

public static int sum(int... numbers) {
    int sum = 0;
    for (int n : numbers) {
        sum += n;
    }
    return sum;
}

3. What is difference between int i =9 or int i = 09?
Ans : In Java, an integer literal with a leading zero, such as int i = 09, is treated as an octal (base 8) number. Octal numbers are represented using the digits 0 through 7, so 09 is not a valid octal number and would result in a compilation error.

On the other hand, an integer literal without a leading zero, such as int i = 9, is treated as a decimal (base 10) number, which is the default base for integer literals in Java. This means that int i = 9 is a valid statement that initializes the integer variable i with the value 9.

4. What is difference between base class and Abstract class?
Ans : In object-oriented programming, a base class (also known as a superclass or parent class) is a class that serves as a starting point for other classes, from which they inherit properties and methods. An abstract class, on the other hand, is a special type of class that cannot be instantiated and serves as a blueprint for other classes to define and implement their own methods.

Here are some differences between a base class and an abstract class:

Instantiability: A base class can be instantiated and used to create objects, while an abstract class cannot be instantiated and can only be used as a superclass for other classes.

Method implementation: A base class can provide implementations for its methods, which can be inherited by its subclasses. An abstract class can define abstract methods (methods without an implementation) that its subclasses must implement.

Properties: A base class can define properties that its subclasses can inherit and use. An abstract class can also define properties, but they are not required to be implemented by its subclasses.

Role: A base class is primarily used to share common functionality among related classes, while an abstract class is used to define a template for its subclasses to follow.

In summary, a base class is a regular class that can be instantiated and provides a set of methods and properties for its subclasses to use, while an abstract class is a special type of class that cannot be instantiated and defines a set of abstract methods that its subclasses must implement.

5. What is difference between functional interface and abstract method ?
Ans : In Java, a functional interface is an interface that has exactly one abstract method. An abstract method is a method that is declared but not implemented in an abstract class or interface. Although they are related concepts, there are some differences between functional interfaces and abstract methods:

Purpose: A functional interface is used to represent a single unit of behavior, typically through the implementation of a lambda expression. An abstract method, on the other hand, is used to define a method that must be implemented by a subclass.

Method count: A functional interface has only one abstract method, while an abstract class or interface can have any number of abstract methods.

Inheritance: A functional interface can extend another interface or class, but it must have only one abstract method. An abstract class or interface can have any number of abstract methods and can also contain non-abstract methods and fields.

Annotations: A functional interface can be annotated with the @FunctionalInterface annotation, which indicates that it is intended to be used as a lambda expression. An abstract method does not have this annotation.

Java 8 and later: The concept of functional interfaces was introduced in Java 8, along with lambda expressions and method references. Abstract methods have been a part of Java since its inception.

In summary, a functional interface is an interface with a single abstract method, used to represent a unit of behavior through a lambda expression, while an abstract method is a method declared but not implemented in an abstract class or interface, used to define a method that must be implemented by a subclass.
