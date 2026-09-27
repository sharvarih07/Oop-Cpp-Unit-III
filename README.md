# Oop-Cpp-Unit-III
OOPs in C++ — Unit III

This repository contains C++ programs demonstrating important Object-Oriented Programming (OOP) concepts from Unit III. The examples focus mainly on function overloading, operator overloading, inheritance, runtime polymorphism, virtual functions, abstract classes, virtual destructors, object slicing, and small polymorphism-based applications.

📚 Topics Covered

Function Overloading

Function Overloading for Area Calculation

Unary Operator Overloading

Prefix and Postfix Increment/Decrement Operators

Arithmetic Operator Overloading with Complex Numbers

Relational Operator Overloading

Friend and Non-Member Operator Overloading

Base-Class Pointer Without Virtual Function

Base-Class Pointer With Virtual Function

Base-Class Reference With Virtual Function

Abstract Classes and Pure Virtual Functions

Collection of Objects Using Base-Class Pointers

Virtual Destructors

Object Slicing

Runtime Polymorphism in a Payment Processing System

Employee Payroll Mini-Project

📂 File Structure

oops-cpp-unit-III/
│
├── 01_functionoverloading.cpp
├── 02_areacalculator.cpp
├── 03_unaryminusoperator.cpp
├── 04_Prefix and Postfix Increment.cpp
├── 05_Complex Number + Operator.cpp
├── 06_Relational Operator.cpp
├── 07_Friend  Non-Member Operator.cpp
├── 08_Base Pointer Without Virtual Function.cpp
├── 09_Base Pointer With Virtual Function.cpp
├── 10_Base Reference With Virtual Function.cpp
├── 11_Abstract Class.cpp
├── 12_Collection of Shape Pointers.cpp
├── 13_Virtual Destructor.cpp
├── 14_Object Slicing.cpp
├── 15_Payment Processing System.cpp
├── 16_Employee Payroll Mini-Project.cpp
└── main.cpp

Note: Each numbered .cpp file contains its own main() function and is intended to be compiled and executed separately.

📝 Program Descriptions

01 — Function Overloading

Demonstrates compile-time polymorphism using multiple add() functions with different parameter lists.

Examples include:

Adding two integers

Adding two doubles

Adding three integers

Joining two strings

02 — Area Calculator

Demonstrates function overloading through different calculateArea() functions for:

Square

Rectangle

Circle

Triangle

03 — Unary Minus Operator

Demonstrates unary operator overloading by overloading the - operator for a Balance class.

04 — Prefix and Postfix Increment

Demonstrates operator overloading for:

Prefix ++

Postfix ++

Prefix --

Postfix --

The program also shows the difference between prefix and postfix behavior.

05 — Complex Number Operators

Demonstrates arithmetic operator overloading for a Complex class.

Implemented operators:

+ for addition

- for subtraction

06 — Relational Operators

Demonstrates relational operator overloading using a Distance class.

Implemented operators:

>

==

07 — Friend / Non-Member Operators

Demonstrates how a friend function can access private members of a class while implementing non-member operator overloads.

Implemented operators:

+

-

08 — Base Pointer Without Virtual Function

Demonstrates the behavior of a base-class pointer when the member function is not virtual.

This example helps explain why runtime polymorphism does not occur without a virtual function.

09 — Base Pointer With Virtual Function

Demonstrates runtime polymorphism using:

Base-class pointer

Virtual function

Function overriding

The example contains:

Animal

Dog

Cat

Cow

10 — Base Reference With Virtual Function

Demonstrates runtime polymorphism using a base-class reference.

The Shape class is used as a common interface for:

Rectangle

Circle

11 — Abstract Class

Demonstrates an abstract class using a pure virtual function:

virtual double area() const = 0;

The example implements:

Rectangle

Triangle

12 — Collection of Shape Pointers

Demonstrates storing different derived objects in a collection through base-class pointers.

It uses:

std::vector<std::unique_ptr<Shape>>

The collection contains:

Rectangle

Circle

Triangle

This example combines:

Abstract classes

Virtual functions

Runtime polymorphism

Smart pointers

STL vector

13 — Virtual Destructor

Demonstrates why a base class should have a virtual destructor when objects may be deleted through a base-class pointer.

The example uses:

Base

Derived

and demonstrates the destructor call order.

14 — Object Slicing

Demonstrates object slicing when a derived object is passed to a function by value as a base-class object.

It compares:

Passing by value

Passing by reference

Passing by pointer

This illustrates why references and pointers are commonly used for polymorphic behavior.

15 — Payment Processing System

A small runtime-polymorphism example using an abstract Payment class.

Payment methods included:

Card Payment

UPI Payment

Net Banking

Wallet Payment

The processPayment() function works with the base-class interface.

16 — Employee Payroll Mini-Project

A small OOP-based payroll application demonstrating runtime polymorphism.

Employee types:

Permanent Employee

Contract Employee

Freelance Employee

The program:

Stores employees using std::unique_ptr

Calculates salary polymorphically

Prints individual pay slips

Calculates total payroll

🧠 Main OOP Concepts Demonstrated

1. Compile-Time Polymorphism

Function and operator overloading allow the compiler to select the appropriate function based on the arguments.

Examples:

add(10, 20);
add(2.5, 3.7);

and:

first + second;

2. Runtime Polymorphism

Runtime polymorphism is demonstrated using virtual functions and inheritance.

Example:

Animal* animal = &dog;
animal->sound();

The appropriate overridden function is selected at runtime.

3. Inheritance

Derived classes extend or specialize the behavior of base classes.

Examples include:

Animal
├── Dog
├── Cat
└── Cow

and:

Employee
├── PermanentEmployee
├── ContractEmployee
└── FreelanceEmployee

4. Abstract Classes

Abstract classes define a common interface using pure virtual functions.

Example:

virtual double area() const = 0;

5. Virtual Functions

Virtual functions enable dynamic dispatch and runtime polymorphism.

6. Virtual Destructors

A virtual destructor ensures proper destruction when a derived object is deleted through a base-class pointer.

7. Smart Pointers

The project uses:

std::unique_ptr

to manage dynamically allocated polymorphic objects safely.

8. STL Vector

The payroll and shape examples use:

std::vector

to store collections of objects.

🛠️ Requirements

You need a C++ compiler supporting modern C++ features.

Recommended:

GCC / G++

Clang

Microsoft Visual C++

C++14 or later

Because the project uses std::make_unique, compiling with C++14 or later is recommended.

▶️ How to Compile and Run

Using G++

Open a terminal inside the project directory.

For example:

g++ -std=c++14 "01_functionoverloading.cpp" -o program

Run:

Windows

program.exe

Linux / macOS

./program

You can replace the filename with any of the numbered .cpp programs.

For example:

g++ -std=c++14 "16_Employee Payroll Mini-Project.cpp" -o payroll

Then run:

payroll

⚠️ Important Notes

Each numbered source file is a separate executable example.

Do not compile all .cpp files together because most of them contain their own main() function.

main.cpp is only a basic Hello World program and is separate from the numbered OOP examples.

Some filenames contain spaces, so use quotation marks around the filename when compiling from a terminal.

The programs are educational examples intended to demonstrate individual OOP concepts.

🎯 Learning Objectives

After studying these programs, you should be able to understand and implement:

Function overloading

Operator overloading

Unary and binary operators

Friend functions

Inheritance

Function overriding

Virtual functions

Runtime polymorphism

Base-class pointers and references

Abstract classes

Pure virtual functions

Virtual destructors

Object slicing

Smart pointers

STL vectors

Basic OOP application design

👨‍💻 Project

Project: OOPs in C++ — Unit III
Language: C++
Type: Educational / Academic Programs
Focus: Object-Oriented Programming and Polymorphism
