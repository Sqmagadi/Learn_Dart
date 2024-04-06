OOP In Dart
Object-oriented programming (OOP) is a programming method that uses objects and their interactions to design and program applications. It is one of the most popular programming paradigms and is used in many programming languages, such as Dart, Java, C++, Python, etc.

targets

In OOP, an object can be anything, such as a person, a bank account, a car, or a house. Each object has its attributes (or properties) and behavior (or methods). For example, a person object may have the attributes name, age and height, and the behavior walk and talk.


Advantages
It is easy to understand and use.
It increases reusability and decreases complexity.
The productivity of programmers increases.
It makes the code easier to maintain, modify and debug.
It promotes teamwork and collaboration.
It reduces the repetition of code.
Features Of OOP
Class
Object
Encapsulation
Inheritance
Polymorphism
Abstraction
 Info
Note: The main purpose of OOP is to break complex problems into smaller objects. You will learn all these OOPs features later in this dart tutorial.

Key Points
Object Oriented Programming (OOP) is a programming paradigm that uses objects and their interactions to design and program applications.
OOP is based on objects, which are data structures containing data and methods.
OOP is a way of thinking about programming that differs from traditional procedural programming.
OOP can make code more modular, flexible, and extensible.
OOP can help you to understand better and solve problems.


Class In Dart
In object-oriented programming, a class is a blueprint for creating objects. A class defines the properties and methods that an object will have. For example, a class called Dog might have properties like breed, color and methods like bark, run.

Declaring Class In Dart
You can declare a class in dart using the class keyword followed by class name and braces {}. It’s a good habit to write class name in PascalCase. For example, Employee, Student, QuizBrain, etc.

Syntax
class ClassName {
// properties or fields
// methods or functions
}
In the above syntax:

The class keyword is used for defining the class.
ClassName is the name of the class and must start with capital letter.
Body of the class consists of properties and functions.
Properties are used to store the data. It is also known as fields or attributes.
Functions are used to perform the operations. It is also known as methods.
Example 1: Declaring A Class In Dart

In this example below, there is class Animal with three properties: name, numberOfLegs, and lifeSpan. The class also has a method called display, which prints out the values of the three properties.

class Animal {
  String? name;
  int? numberOfLegs;
  int? lifeSpan;

  void display() {
    print("Animal name: $name.");
    print("Number of Legs: $numberOfLegs.");
    print("Life Span: $lifeSpan.");
  }
}
 Info
Note: This program will not print anything because we have not created any object of the class. You will learn about the object later. The ? is used for null safety. You will also learn about null safety later.

Example 2: Declaring A Person Class In Dart

In this example below, there is class Person with four properties: name, phone, isMarried, and age. The class also has a method called displayInfo, which prints out the values of the four properties.

class Person {
  String? name;
  String? phone;
  bool? isMarried;
  int? age;

  void displayInfo() {
    print("Person name: $name.");
    print("Phone number: $phone.");
    print("Married: $isMarried.");
    print("Age: $age.");
  }
}
Example 3: Declaring Area Class In Dart
In this example below, there is class Area with two properties: length and breadth. The class also has a method called calculateArea, which calculates the area of the rectangle.

class Area {
  double? length;
  double? breadth;

  double calculateArea() {
    return length! * breadth!;
  }
}
Example 4: Declaring A Student Class In Dart
In this example below, there is class Student with three properties: name, age, and grade. The class also has a method called displayInfo, which prints out the values of the three properties.

class Student {
  String? name;
  int? age;
  int? grade;

  void displayInfo() {
    print("Student name: $name.");
    print("Student age: $age.");
    print("Student grade: $grade.");
  }
}
Key Points
The class is declared using the class keyword.
The class is a blueprint for creating objects.
The class body consists of properties and methods.
The properties are also known as fields, attributes, or data members.
The methods are also known as behaviors, or member functions.
Challenge
Create a class Book with three properties: name, author, and price. Also, create a method called display, which prints out the values of the three properties.


Object In Dart
In object-oriented programming, an object is a self-contained unit of code and data. Objects are created from templates called classes. An object is made up of properties(variables) and methods(functions). An object is an instance of a class.

For example, a bicycle object might have attributes like color, size, and current speed. It might have methods like changeGear, pedalFaster, and brake.

 Info
Note: To create an object, you must create a class first. It’s a good practice to declare the object name in lower case.

Instantiation

In object-oriented programming, instantiation is the process of creating an instance of a class. In other words, you can say that instantiation is the process of creating an object of a class. For example, if you have a class called Bicycle, then you can create an object of the class called bicycle.

Declaring Object In Dart
Once you have created a class, it’s time to declare the object. You can declare an object by the following syntax:

Syntax
ClassName objectName = ClassName();
Example 1: Declaring An Object In Dart
In this example below, there is class Bycycle with three properties: color, size, and currentSpeed. The class has two methods. One is changeGear, which changes the gear of the bicycle, and display method prints out the values of the three properties. We also have an object of the class Bycycle called bicycle.

    class Bicycle {
      String? color;
      int? size;
      int? currentSpeed;
    
      void changeGear(int newValue) {
        currentSpeed = newValue;
      }
    
      void display() {
        print("Color: $color");
        print("Size: $size");
        print("Current Speed: $currentSpeed");
      }
    }

    void main(){
        // Here bicycle is object of class Bicycle. 
        Bicycle bicycle = Bicycle();
        bicycle.color = "Red";
        bicycle.size = 26;
        bicycle.currentSpeed = 0;
        bicycle.changeGear(5);
        bicycle.display();
    }
 Show Output
 Info
Note: Once you create an object, you can access the properties and methods of the object using the dot(.) operator.

Example 2: Declaring Animal Class Object In Dart

In this example below there is class Animal with three properties: name, numberOfLegs, and lifeSpan. The class also has a method called display, which prints out the values of the three properties. We also have an object of the class Animal called animal.

class Animal {
      String? name;
      int? numberOfLegs;
      int? lifeSpan;
    
      void display() {
        print("Animal name: $name.");
        print("Number of Legs: $numberOfLegs.");
        print("Life Span: $lifeSpan.");
      }
    }

    void main(){
        // Here animal is object of class Animal. 
        Animal animal = Animal();
        animal.name = "Lion";
        animal.numberOfLegs = 4;
        animal.lifeSpan = 10;
        animal.display();
    }
 Show Output
Example 3: Declaring Car Class Object In Dart
In this example below there is class Car with three properties: name, color, and numberOfSeats. The class also has a method called start, which prints out the message “Car Started”. We also have an object of the class Car called car.

class Car {
  String? name;
  String? color;
  int? numberOfSeats;

  void start() {
    print("$name Car Started.");
  }
}

void main(){
    // Here car is object of class Car. 
    Car car = Car();
    car.name = "BMW";
    car.color = "Red";
    car.numberOfSeats = 4;
    car.start();

    // Here car2 is another object of class Car.
    Car car2 = Car();
    car2.name = "Audi";
    car2.color = "Black";
    car2.numberOfSeats = 4;
    car2.start();
}
 Show Output
Key Points
The main method is the program’s entry point, so it is always needed to see the result.
The new keyword can be used to create a new object, but it is unnecessary.
Challenge
Create a class Camera with properties: name, color, megapixel. Create a method called display which prints out the values of the three properties. Create two objects of the class Camera and call the method display.


CLASS AND OBJECTS IN DART
What is Class
targets

A class is a blueprint for creating objects. A class defines the properties and methods that an object will have. If you want to learn more about class in Dart, you can read class in dart.

What is Object
An object is an instance of a class. You can create multiple objects of the same class. If you want to learn more about an object in Dart, you can read object in dart.


Example Of A Class & Object In Dart
In this example below there is class Animal with three properties: name, numberOfLegs, and lifeSpan. The class also has a method called display, which prints out the values of the three properties.

class Animal {
  String? name;
  int? numberOfLegs;
  int? lifeSpan;

  void display() {
    print("Animal name: $name.");
    print("Number of Legs: $numberOfLegs.");
    print("Life Span: $lifeSpan.");
  }
}

void main(){
  // Here animal is object of class Animal. 
  Animal animal = Animal();
  animal.name = "Lion";
  animal.numberOfLegs = 4;
  animal.lifeSpan = 10;
  animal.display();
}
targets

 Show Output
Example 2: Find Area Of Ractangle Using Class and Objects

In this example below there is class Rectangle with two properties: length and breadth. The class also has a method called area, which calculates the area of the rectangle.

class Rectangle{
  //properties of rectangle
  double? length;
  double? breadth;
  
  //functions of rectangle
  double area(){
    return length! * breadth!;
  }
}

void main(){
  //object of rectangle created
  Rectangle rectangle = Rectangle();
  
  //setting properties for rectangle
  rectangle.length=10;
  rectangle.breadth=5;
  
  //functions of rectangle called
  print("Area of rectangle is ${rectangle.area()}.");
}
targets

 Show Output
 Info
Note: Here ! is used to tell the compiler that the variable is not null. If you don’t use !, then you will get an error. You will learn more about it in null safety later.

Example 3: Find Simple Interest Using Class and Objects
In this example below there is class SimpleInterest with three properties: principal, rate, and time. The class also has a method called interest, which calculates the simple interest.

class SimpleInterest{
  //properties of simple interest
  double? principal;
  double? rate;
  double? time;
  
  //functions of simple interest
  double interest(){
    return (principal! * rate! * time!)/100;
  }
}
void main(){
  //object of simple interest created
  SimpleInterest simpleInterest = SimpleInterest();
  
  //setting properties for simple interest
  simpleInterest.principal=1000;
  simpleInterest.rate=10;
  simpleInterest.time=2;
  
  //functions of simple interest called
  print("Simple Interest is ${simpleInterest.interest()}.");
}
targets

 Show Output
Challenge
Create class Home with properties name, address, numberOfRooms. Create a method called display which prints out the values of the properties. Create an object of the class Home and set the values of the properties. Call the method display to print out the values of the properties.