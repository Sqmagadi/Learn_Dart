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


CONSTRUCTOR IN DART
Introduction
targets

In this section, you will learn about constructor in Dart programming language and how to use constructors with the help of examples. Before learning about the constructor, you should have a basic understanding of the class and object in dart.

Constructor In Dart
A constructor is a special method used to initialize an object. It is called automatically when an object is created, and it can be used to set the initial values for the object’s properties. For example, the following code creates a Person class object and sets the initial values for the name and age properties.

Person person = Person("John", 30);
targets

Without Constructor
If you don’t define a constructor for class, then you need to set the values of the properties manually. For example, the following code creates a Person class object and sets the values for the name and age properties.

Person person = Person();
person.name = "John";
person.age = 30;
targets

Things To Remember
The constructor’s name should be the same as the class name.
Constructor doesn’t have any return type.
Syntax
class ClassName {
  // Constructor declaration: Same as class name
  ClassName() {
    // body of the constructor
  }
}
targets

 Info
Note: When you create a object of a class, the constructor is called automatically. It is used to initialize the values when an object is created.

Example 1: How To Declare Constructor In Dart

In this example below, there is a class Student with three properties: name, age, and rollNumber. The class has one constructor. The constructor is used to initialize the values of the three properties. We also created an object of the class Student called student.

class Student {
  String? name;
  int? age;
  int? rollNumber;

  // Constructor
  Student(String name, int age, int rollNumber) {
    print(
        "Constructor called"); // this is for checking the constructor is called or not.
    this.name = name;
    this.age = age;
    this.rollNumber = rollNumber;
  }
}

void main() {
  // Here student is object of class Student.
  Student student = Student("John", 20, 1);
  print("Name: ${student.name}");
  print("Age: ${student.age}");
  print("Roll Number: ${student.rollNumber}");
}
targets

 Show Output
 Info
Note: The this keyword is used to refer to the current instance of the class. It is used to access the current class properties. In the example above, parameter names and class properties of constructor Student are the same. Hence to avoid confusion, we use the this keyword.

Example 2: Constructor In Dart

In this example below, there is a class Teacher with four properties: name, age, subject, and salary. Class has one constructor for initializing the values of the properties. Class also contain method display() which is used to display the values of the properties. We also created 2 objects of the class Teacher called teacher1 and teacher2.

class Teacher {
  String? name;
  int? age;
  String? subject;
  double? salary;

  // Constructor
  Teacher(String name, int age, String subject, double salary) {
    this.name = name;
    this.age = age;
    this.subject = subject;
    this.salary = salary;
  }
  // Method
  void display() {
    print("Name: ${this.name}");
    print("Age: ${this.age}");
    print("Subject: ${this.subject}");
    print("Salary: ${this.salary}\n"); // \n is used for new line
  }
}

void main() {
  // Creating teacher1 object of class Teacher
  Teacher teacher1 = Teacher("John", 30, "Maths", 50000.0);
  teacher1.display();

  // Creating teacher2 object of class Teacher
  Teacher teacher2 = Teacher("Smith", 35, "Science", 60000.0);
  teacher2.display();
}
targets

 Show Output
 Info
Note: You can create many objects of a class. Each object will have its own copy of the properties.

Example 3: Constructor In Dart
In this example below, there is a class Car with two properties: name and price. The class has one constructor for initializing the values of the properties. The class also contains method display(), which is used to display the values of the properties. We also created an object of the class Car called car.

 class Car {
  String? name;
  double? price;

  // Constructor
  Car(String name, double price) {
    this.name = name;
    this.price = price;
  }

  // Method
  void display() {
    print("Name: ${this.name}");
    print("Price: ${this.price}");
  }
}

void main() {
  // Here car is object of class Car.
  Car car = Car("BMW", 500000.0);
  car.display();
}
targets

 Show Output
Example 4: Constructor In Dart
In this example below, there is a class Staff with four properties: name, phone1, phone2, and subject and one method display(). Class has one constructor for initializing the values of only name, phone1 and subject. We also created an object of the class Staff called staff.

 class Staff {
  String? name;
  int? phone1;
  int? phone2;
  String? subject;

  // Constructor
  Staff(String name, int phone1, String subject) {
    this.name = name;
    this.phone1 = phone1;
    this.subject = subject;
  }

  // Method
  void display() {
    print("Name: ${this.name}");
    print("Phone1: ${this.phone1}");
    print("Phone2: ${this.phone2}");
    print("Subject: ${this.subject}");
  }
}

void main() {
  // Here staff is object of class Staff.
  Staff staff = Staff("John", 1234567890, "Maths");
  staff.display();
}
targets

 Show Output
Example 5: Write Constructor Single Line
In the avobe section, you have written the constructor in long form. You can also write the constructor in short form. You can directly assign the values to the properties. For example, the following code is the short form of the constructor in one line.

class Person{
  String? name;
  int? age;
  String? subject;
  double? salary;

  // Constructor in short form
  Person(this.name, this.age, this.subject, this.salary);

  // display method
  void display(){
    print("Name: ${this.name}");
    print("Age: ${this.age}");
    print("Subject: ${this.subject}");
    print("Salary: ${this.salary}");
  }
}

void main(){
  Person person = Person("John", 30, "Maths", 50000.0);
  person.display();
}
targets

 Show Output
Example 6: Constructor With Optional Parameters
In the example below, we have created a class Employee with four properties: name, age, subject, and salary. Class has one constructor for initializing the all properties values. For subject and salary, we have used optional parameters. It means we can pass or not pass the values of subject and salary. The Class also contain method display() which is used to display the values of the properties. We also created an object of the class Employee called employee.

class Employee {
  String? name;
  int? age;
  String? subject;
  double? salary;

  // Constructor
  Employee(this.name, this.age, [this.subject = "N/A", this.salary=0]);

  // Method
  void display() {
    print("Name: ${this.name}");
    print("Age: ${this.age}");
    print("Subject: ${this.subject}");
    print("Salary: ${this.salary}");
  }
}

void main(){
  Employee employee = Employee("John", 30);
  employee.display();
}
targets

 Show Output
Example 7: Constructor With Named Parameters
In the example below, we have created a class Chair with two properties: name and color. Class has one constructor for initializing the all properties values with named parameters. The Class also contain method display() which is used to display the values of the properties. We also created an object of the class Chair called chair.

class Chair {
String? name;
String? color;

// Constructor
Chair({this.name, this.color});

// Method
void display() {
  print("Name: ${this.name}");
  print("Color: ${this.color}");
}
}

void main(){
Chair chair = Chair(name: "Chair1", color: "Red");
chair.display();
}
targets

 Show Output
Example 8: Constructor With Default Values
In the example below, we have created a class Table with two properties: name and color. Class has one constructor for initializing the all properties values with default values. The Class also contain method display() which is used to display the values of the properties. We also created an object of the class Table called table.

class Table {
  String? name;
  String? color;

  // Constructor
  Table({this.name = "Table1", this.color = "White"});

  // Method
  void display() {
    print("Name: ${this.name}");
    print("Color: ${this.color}");
  }
}

void main(){
  Table table = Table();
  table.display();
}
targets

 Show Output
Key Points
The constructor’s name should be the same as the class name.
Constructor doesn’t have any return type.
Constructor is only called once at the time of the object creation.
Constructor is called automatically when an object is created.
Constructor is used to initialize the values of the properties of the class.
Challenge
Create a class Patient with three properties name, age, and disease. The class has one constructor. The constructor is used to initialize the values of the three properties. Also, create an object of the class Patient called patient. Print the values of the three properties using the object.


DEFAULT CONSTRUCTOR IN DART
Default Constructor
The constructor which is automatically created by the dart compiler if you don’t create a constructor is called a default constructor. A default constructor has no parameters. A default constructor is declared using the class name followed by parentheses ().

Example 1: Default Constructor In Dart
In this example below, there is a class Laptop with two properties: brand, and price. Lets create constructor with no parameter and print something from the constructor. We also have an object of the class Laptop called laptop.

class Laptop {
  String? brand;
  int? price;

  // Constructor
  Laptop() {
    print("This is a default constructor");
  }
}

void main() {
  // Here laptop is object of class Laptop.
  Laptop laptop = Laptop();
}
 Show Output
 Info
Note: The default constructor is called automatically when you create an object of the class. It is used to initialize the instance variables of the class.

Example 2: Default Constructor In Dart

In this example below, there is a class Student with four properties: name, age, schoolname and grade. The default constructor is used to initialize the values of the school name. The reason for this is that the school name is the same for all the students. We also have an object of the class Student called student. The default constructor is called automatically when you create an object of the class.

class Student {
  String? name;
  int? age;
  String? schoolname;
  String? grade;

  // Default Constructor
  Student() {
    print(
        "Constructor called"); // this is for checking the constructor is called or not.
    schoolname = "ABC School";
  }
}

void main() {
  // Here student is object of class Student.
  Student student = Student();
  student.name = "John";
  student.age = 10;
  student.grade = "A";
  print("Name: ${student.name}");
  print("Age: ${student.age}");
  print("School Name: ${student.schoolname}");
  print("Grade: ${student.grade}");
}
 Show Output
Challenge

Try to create a class Person with two properties: name, and planet. Create a default constructor to initialize the values of the planet to earth. Create an object of the class Person, set the name to “Your Name” and print the name and planet.


PARAMETERIZED CONSTRUCTOR IN DART
Parameterized Constructor
Parameterized constructor is used to initialize the instance variables of the class. Parameterized constructor is the constructor that takes parameters. It is used to pass the values to the constructor at the time of object creation.

Syntax
class ClassName {
  // Instance Variables
  int? number;
  String? name;
  // Parameterized Constructor
  ClassName(this.number, this.name);
}
Example 1: Parameterized Constructor In Dart

In this example below, there is a class Student with three properties: name, age, and rollNumber. The class has one constructor. The constructor is used to initialize the values of the three properties. We also have an object of the class Student called student.

class Student {
  String? name;
  int? age;
  int? rollNumber;
  // Constructor
  Student(this.name, this.age, this.rollNumber);
}

void main(){
    // Here student is object of class Student. 
    Student student = Student("John", 20, 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
 Show Output
Example 2: Parameterized Constructor With Named Parameters In Dart

In this example below, there is a class Student with three properties: name, age, and rollNumber. The class has one constructor. The constructor is used to initialize the values of the three properties. We also have an object of the class Student called student.

class Student {
  String? name;
  int? age;
  int? rollNumber;

  // Constructor
  Student({String? name, int? age, int? rollNumber}) {
    this.name = name;
    this.age = age;
    this.rollNumber = rollNumber;
  }
}

void main(){
    // Here student is object of class Student. 
    Student student = Student(name: "John", age: 20, rollNumber: 1);
    print("Name: ${student.name}");
    print("Age: ${student.age}");
    print("Roll Number: ${student.rollNumber}");
}
 Show Output
Example 3: Parameterized Constructor With Default Values In Dart
In this example below, there is class Student with two properties: name, and age. The class has parameterized constructor with default values. The constructor is used to initialize the values of the two properties. We also have an object of the class Student called student.

class Student {
  String? name;
  int? age;

  // Constructor
  Student({String? name = "John", int? age = 0}) {
    this.name = name;
    this.age = age;
  }
}

void main(){
    // Here student is object of class Student. 
    Student student = Student();
    print("Name: ${student.name}");
    print("Age: ${student.age}");
}
 Show Output
 Info
Note: In parameterized constructor, at the time of object creation, you must pass the parameters through the constructor which initialize the variables value, avoiding the null values.


NAMED CONSTRUCTOR IN DART
Named Constructor In Dart
targetsIn most programming languages like java, c++, c#, etc., we can create multiple constructors with the same name. But in Dart, this is not possible. Well, there is a way. We can create multiple constructors with the same name using named constructors.

 Info
Note: Named constructors improves code readability. It is useful when you want to create multiple constructors with the same name.

Example 1: Named Constructor In Dart

In this example below, there is a class Student with three properties: name, age, and rollNumber. The class has two constructors. The first constructor is a default constructor. The second constructor is a named constructor. The named constructor is used to initialize the values of the three properties. We also have an object of the class Student called student.

class Student {
  String? name;
  int? age;
  int? rollNumber;

  // Default Constructor
  Student() {
    print("This is a default constructor");
  }

  // Named Constructor
  Student.namedConstructor(String name, int age, int rollNumber) {
    this.name = name;
    this.age = age;
    this.rollNumber = rollNumber;
  }
}

void main() {
  // Here student is object of class Student.
  Student student = Student.namedConstructor("John", 20, 1);
  print("Name: ${student.name}");
  print("Age: ${student.age}");
  print("Roll Number: ${student.rollNumber}");
}
targets

 Show Output
Example 2: Named Constructor In Dart

In this example below, there is class Mobile with three properties name, color, and price. The class has one method display which prints out the values of the three properties. We also have an object of the class Mobile called mobile. There is also constructor Mobile which takes all the three properties as parameters. Named constructor Mobile.namedConstructor is used to create an object of the class Mobile with name, color and optional price. The default value of the price is 0. If the price is not passed, then the default value is used.

class Mobile {
  String? name;
  String? color;
  int? price;

  Mobile(this.name, this.color, this.price);
  // here Mobile() is a named constructor
  Mobile.namedConstructor(this.name, this.color, [this.price = 0]);

  void displayMobileDetails() {
    print("Mobile name: $name.");
    print("Mobile color: $color.");
    print("Mobile price: $price");
  }
}

void main() {
  var mobile1 = Mobile("Samsung", "Black", 20000);
  mobile1.displayMobileDetails();
  var mobile2 = Mobile.namedConstructor("Apple", "White");
  mobile2.displayMobileDetails();
}
targets

 Show Output
Example 3: Named Constructor In Dart
In this example below, there is a class Animal with two properties name and age. The class has three constructors. The first constructor is a default constructor. The second and third constructors are named constructors. The second constructor is used to initialize the values of name and age, and the third constructor is used to initialize the value of name only. We also have an object of the class Animal called animal.

class Animal {
  String? name;
  int? age;

  // Default Constructor
  Animal() {
    print("This is a default constructor");
  }

  // Named Constructor
  Animal.namedConstructor(String name, int age) {
    this.name = name;
    this.age = age;
  }

  // Named Constructor
  Animal.namedConstructor2(String name) {
    this.name = name;
  }
}
void main(){
  // Here animal is object of class Animal.
  Animal animal = Animal.namedConstructor("Dog", 5);
  print("Name: ${animal.name}");
  print("Age: ${animal.age}");

  Animal animal2 = Animal.namedConstructor2("Cat");
  print("Name: ${animal2.name}");
}
targets

 Show Output
Example 4: Real Life Example Of Named Constructor In Dart
In this example below, there is a class Person with two properties name and age. The class has three constructors. The first is a parameterized constructor which takes two parameters name and age. The second and third constructors are named constructors. Second constructor fromJson is used to create an object of the class Person from a JSON. The third fromJsonString is used to create an object of the class Person from a JSON string. We also have an object of the class Person called person.

import 'dart:convert';

class Person {
  String? name;
  int? age;

  Person(this.name, this.age);

  Person.fromJson(Map<String, dynamic> json) {
    name = json['name'];
    age = json['age'];
  }

  Person.fromJsonString(String jsonString) {
    Map<String, dynamic> json = jsonDecode(jsonString);
    name = json['name'];
    age = json['age'];
  }
}

void main() {
// Here person is object of class Person.
  String jsonString1 = '{"name": "Bishworaj", "age": 25}';
  String jsonString2 = '{"name": "John", "age": 30}';

  Person p1 = Person.fromJsonString(jsonString1);
  print("Person 1 name: ${p1.name}");
  print("Person 1 age: ${p1.age}");

  Person p2 = Person.fromJsonString(jsonString2);
  print("Person 2 name: ${p2.name}");
  print("Person 2 age: ${p2.age}");
}
targets

 Show Output
Challenge
Try to create a class Car with three properties name, color, and price and one method display which prints out the values of the three properties. Create a constructor, which takes all 3 parameters. Create a named constructor which takes two parameters name and color. Create an object of the class from both the constructors and call the method display.


Constant Constructor In Dart
Constant constructor is a constructor that creates a constant object. A constant object is an object whose value cannot be changed. A constant constructor is declared using the keyword const.

 Info
Note: Constant Constructor is used to create a object whose value cannot be changed. It Improves the performance of the program.

Rule For Declaring Constant Constructor In Dart
All properties of the class must be final.
It does not have any body.
Only class containing const constructor is initialized using the const keyword.
Example 1: Constant Constructor In Dart

In this example below, there is a class Point with two final properties: x and y. The class also has a constant constructor that initializes the two properties. The class also has a method called display, which prints out the values of the two properties.

class Point {
  final int x;
  final int y;

  const Point(this.x, this.y);
}

void main() {
  // p1 and p2 has the same hash code.
  Point p1 = const Point(1, 2);
  print("The p1 hash code is: ${p1.hashCode}");

  Point p2 = const Point(1, 2);
  print("The p2 hash code is: ${p2.hashCode}");
  // without using const
  // this has different hash code.
  Point p3 = Point(2, 2);
  print("The p3 hash code is: ${p3.hashCode}");

  Point p4 = Point(2, 2);
  print("The p4 hash code is: ${p4.hashCode}");
}
targets

 Show Output
 Info
Note: Here p1 and p2 has the same hash code. This is because p1 and p2 are constant objects. The hash code of a constant object is the same. This is because the hash code of a constant object is computed at compile time. The hash code of a non-constant object is computed at run time. This is why p3 and p4 have different hash code.

Example 2: Constant Constructor In Dart

In this example below, there is a class Student with three properties: name, age, and rollNumber. The class has one constant constructor. The constructor is used to initialize the values of the three properties. We also have an object of the class Student called student.

class Student {
  final String? name;
  final int? age;
  final int? rollNumber;

  // Constant Constructor
  const Student({this.name, this.age, this.rollNumber});
}

void main() {
  // Here student is object of Student.
  const Student student = Student(name: "John", age: 20, rollNumber: 1);
  print("Name: ${student.name}");
  print("Age: ${student.age}");
  print("Roll Number: ${student.rollNumber}");
}
targets

 Show Output
Example 3: Constant Constructor With Named Parameters In Dart
In this example below, there is a class Car with three properties: name, model, and price. The class has one constructor. The constructor is used to initialize the values of the three properties. We also have an object of the class Car called car.

class Car {
  final String? name;
  final String? model;
  final int? price;

  // Constant Constructor
  const Car({this.name, this.model, this.price});
}

void main() {
  // Here car is object of class Car.
  const Car car = Car(name: "BMW", model: "X5", price: 50000);
  print("Name: ${car.name}");
  print("Model: ${car.model}");
  print("Price: ${car.price}");
}
targets

 Show Output
Benefits Of Constant Constructor In Dart
Improves the performance of the program.
Challenge
Create a class Customer with three properties: name, age, and phone. The class should have one constant constructor. The constructor should initialize the values of the three properties. Create an object of the class Customer and print the values of the three properties.


ENCAPSULATION IN DART
Introduction
In this section, you will learn about encapsulation in Dart programming language with examples. Encapsulation is one of the important concepts of object-oriented programming. Before learning about dart encapsulation, you should have a basic understanding of the class and object in dart.

Encapsulation In Dart
In Dart, Encapsulation means hiding data within a library, preventing it from outside factors. It helps you control your program and prevent it from becoming too complicated.

What Is Library In Dart?

By default, every .dart file is a library. A library is a collection of functions and classes. A library can be imported into another library using the import keyword.

How To Achieve Encapsulation In Dart?
Encapsulation can be achieved by:

Declaring the class properties as private by using underscore(_).
Providing public getter and setter methods to access and update the value of private property.
 Info
Note: Dart doesn’t support keywords like public, private, and protected. Dart uses _ (underscore) to make a property or method private. The encapsulation happens at library level, not at class level.

Getter and Setter Methods
Getter and setter methods are used to access and update the value of private property. Getter methods are used to access the value of private property. Setter methods are used to update the value of private property.


Example 1: Encapsulation In Dart
In this example, we will create a class named Employee. The class will have two private properties _id and _name. We will also create two public methods getId() and getName() to access the private properties. We will also create two public methods setId() and setName() to update the private properties.

class Employee {
  // Private properties
  int? _id;
  String? _name;

// Getter method to access private property _id
  int getId() {
    return _id!;
  }
// Getter method to access private property _name
  String getName() {
    return _name!;
  }
// Setter method to update private property _id
  void setId(int id) {
    this._id = id;
  }
// Setter method to update private property _name
  void setName(String name) {
    this._name = name;
  }
  
}

void main() {
  // Create an object of Employee class
  Employee emp = new Employee();
  // setting values to the object using setter
  emp.setId(1);
  emp.setName("John");

  // Retrieve the values of the object using getter
  print("Id: ${emp.getId()}");
  print("Name: ${emp.getName()}");
}
 Show Output
Private Properties
Private property is a property that can only be accessed from same library. Dart does not have any keywords like private to define a private property. You can define it by prefixing an underscore (_) to its name.

Example 2: Private Properties In Dart
In this example, we will create a class named Employee. The class has one private property _name. We will also create a public method getName() to access the private property.

class Employee {
  // Private property
  var _name;

  // Getter method to access private property _name
  String getName() {
    return _name;
  }

  // Setter method to update private property _name
  void setName(String name) {
    this._name = name;
  }
}

void main() {
  var employee = Employee();
  employee.setName("Jack");
  print(employee.getName());
}
 Show Output
Why Aren’t Private Properties Private?
In the main method, if you write the following code, it will compile and run without any error. Let’s see why it is happening.

class Employee {
  // Private property
  var _name;

  // Getter method to access private property _name
  String getName() {
    return _name;
  }

  // Setter method to update private property _name
  void setName(String name) {
    this._name = name;
  }
}

void main() {
  var employee = Employee();
  employee._name = "John"; // It is working, but why?
  print(employee.getName());
}
 Show Output
Reason
The reason is that using underscore (_) before a variable or method name makes it library private not class private. It means that the variable or method is only visible to the library in which it is declared. It is not visible to any other library. In simple words, library is one file. If you write the main method in a separate file, this will not work.

Solution
To see private properties in action, you must create a separate file for the class and import it into the main file.

Read-only Properties
You can control the properties’s access and implement the encapsulation in the dart by using the read-only properties. You can do that by adding the final keyword before the properties declaration. Hence, you can only access its value, but you cannot change it.

 Info
Note: Properties declared with the final keyword must be initialized at the time of declaration. You can also initialize them in the constructor.

class Student {
  final _schoolname = "ABC School";

  String getSchoolName() {
    return _schoolname;
  }
}

void main() {
  var student = Student();
  print(student.getSchoolName());
  // This is not possible
  //student._schoolname = "XYZ School";
}
 Show Output
 Info
Note: You can also define getter and setter using get and set keywords. For more see this example below.

How To Create Getter and Setter Methods?
You can create getter and setter methods by using the get and set keywords. In this example below, we have created a class named Vehicle. The class has two private properties _model and _year. We have also created two getter and setter methods for each property. The getter and setter methods are named model and year. The getter and setter methods are used to access and update the value of the private properties.

class Vehicle {
  String _model;
  int _year;

  // Getter method
  String get model => _model;

  // Setter method
  set model(String model) => _model = model;

  // Getter method
  int get year => _year;

  // Setter method
  set year(int year) => _year = year;
}

void main() {
  var vehicle = Vehicle();
  vehicle.model = "Toyota";
  vehicle.year = 2019;
  print(vehicle.model);
  print(vehicle.year);
}
 Show Output
 Info
Note: In dart, any identifier like (class, class properties, top-level function, or variable) that starts with an underscore _ it is private to its library.

Why Encapsulation Is Important?
Data Hiding: Encapsulation hides the data from the outside world. It prevents the data from being accessed by the code outside the class. This is known as data hiding.

Testability: Encapsulation allows you to test the class in isolation. It will enable you to test the class without testing the code outside the class.

Flexibility: Encapsulation allows you to change the implementation of the class without affecting the code outside the class.

Security: Encapsulation allows you to restrict access to the class members. It will enable you to limit access to the class members from the code outside the library.

Video

GETTER IN DART
Getter In Dart
Getter is used to get the value of a property. It is mostly used to access a private property’s value. Getter provide explicit read access to an object properties.

Syntax
return_type get property_name {
  // Getter body
}
 Info
Note: Instead of writing { } after the property name, you can also write => (fat arrow) after the property name.

Example 1: Getter In Dart

In this example below, there is a class named Person. The class has two properties firstName and lastName. There is getter fullName which is responsible to get full name of person.

class Person {
  // Properties
  String? firstName;
  String? lastName;

  // Constructor
  Person(this.firstName, this.lastName);

  // Getter
  String get fullName => "$firstName $lastName";
}

void main() {
  Person p = Person("John", "Doe");
  print(p.fullName);
}
 Show Output
Example 2: Getter In Dart

In this example below, there is a class named NoteBook. The class has two private properties _name and _prize. There are two getters name and price to access the value of the properties.

class NoteBook {
  // Private properties
  String? _name;
  double? _prize;

  // Constructor
  NoteBook(this._name, this._prize);

  // Getter method to access private property _name
  String get name => this._name!;

  // Getter method to access private property _prize
  double get price => this._prize!;
}

void main() {
  // Create an object of NoteBook class
  NoteBook nb = new NoteBook("Dell", 500);
  // Display the values of the object
  print(nb.name);
  print(nb.price);
}
 Show Output
 Info
Note: In the above example, a getter name and price are used to access the value of the properties _name and _prize.

Example 3: Getter In Dart With Data Validation
In this example below, there is a class named NoteBook. The class has two private properties _name and _prize. There are two getters name and price to access the value of the properties. If you provide a blank name, then it will return No Name.

class NoteBook {
  // Private properties
  String _name;
  double _prize;

  // Constructor
  NoteBook(this._name, this._prize);

  // Getter to access private property _name
  String get name {
    if (_name == "") {
      return "No Name";
    }
    return this._name;
  }

  // Getter to access private property _prize
  double get price {
    return this._prize;
  }
}

void main() {
  // Create an object of NoteBook class
  NoteBook nb = new NoteBook("Apple", 1000);
  print("First Notebook name: ${nb.name}");
  print("First Notebook price: ${nb.price}");
  NoteBook nb2 = new NoteBook("", 500);
  print("Second Notebook name: ${nb2.name}");
  print("Second Notebook price: ${nb2.price}");
}
 Show Output
Example 4: Getter In Dart
In this example below, there is a class named Doctor. The class has three private properties _name, _age and _gender. There are three getters name, age, and gender to access the value of the properties. It has map getter to get Map of the object.

class Doctor {
// Private properties
  String _name;
  int _age;
  String _gender;

// Constructor
  Doctor(this._name, this._age, this._gender);

// Getters
  String get name => _name;
  int get age => _age;
  String get gender => _gender;

// Map Getter
  Map<String, dynamic> get map {
    return {"name": _name, "age": _age, "gender": _gender};
  }
}

void main() {
// Create an object of Doctor class
  Doctor d = Doctor("John", 41, "Male");
  print(d.map);
}
 Show Output
Why Is Getter Important In Dart?
To access the value of private property.
To restrict the access of data members of a class.


Setter In Dart
Setter is used to set the value of a property. It is mostly used to update a private property’s value. Setter provide explicit write access to an object properties.

Syntax
set property_name (value) {
  // Setter body
}
 Info
Note: Instead of writing { } after the property name, you can also write => (fat arrow) after the property name.

Example 1: Setter In Dart

In this example below, there is a class named NoteBook. The class has two private properties _name and _prize. There are two setters name and price to update the value of the properties. There is also a method display to display the value of the properties.

class NoteBook {
  // Private Properties
  String? _name;
  double? _prize;

  // Setter to update private property _name
  set name(String name) => this._name = name;

  // Setter to update private property _prize
  set price(double price) => this._prize = price;

  // Method to display the values of the properties
  void display() {
    print("Name: ${_name}");
    print("Price: ${_prize}");
  }
}

void main() {
  // Create an object of NoteBook class
  NoteBook nb = new NoteBook();
  // setting values to the object using setter
  nb.name = "Dell";
  nb.price = 500.00;
  // Display the values of the object
  nb.display();
}
 Show Output
 Info
Note: In the above example, a setter name and price are used to update the value of the properties _name and _prize.

Example 2: Setter In Dart With Data Validation

In this example, there is a class named NoteBook. The class has two private properties _name and _prize. If the value of _prize is less than 0, we will throw an exception. There are also two setters name and price to update the value of the properties. The class also has a method display() to display the values of the properties.

class NoteBook {
  // Private properties
  String? _name;
  double? _prize;

  // Setter to update the value of name property
  set name(String name) => _name = name;

  // Setter to update the value of price property
  set price(double price) {
    if (price < 0) {
      throw Exception("Price cannot be less than 0");
    }
    this._prize = price;
  }

  // Method to display the values of the properties
  void display() {
    print("Name: $_name");
    print("Price: $_prize");
  }
}

void main() {
  // Create an object of NoteBook class
  NoteBook nb = new NoteBook();
  // setting values to the object using setter
  nb.name = "Dell";
  nb.price = 250;

  // Display the values of the object
  nb.display();
}
 Show Output
 Info
Note: It is generally best to not allow the user to set the value of a field directly. Instead, you should provide a setter method that can validate the value before setting it. This is very important when working on large and complex programs.

Example 3: Setter In Dart
In this example, there is a class named Student. The class has two private properties _name and _classnumber. We will also create two setters name and classnumber to update the value of the properties. The classnumber setter will only accept a value between 1 and 12. The class also has a method display() to display the values of the properties.

class Student {
  // Private properties
  String? _name;
  int? _classnumber;

  // Setter to update the value of name property
  set name(String name) => this._name = name;

  // Setter to update the value of classnumber property
  set classnumber(int classnumber) {
    if (classnumber <= 0 || classnumber > 12) {
      throw ('Classnumber must be between 1 and 12');
    }
    this._classnumber = classnumber;
  }

  // Method to display the values of the properties
  void display() {
    print("Name: $_name");
    print("Class Number: $_classnumber");
  }
}
void main() {
  // Create an object of Student class
  Student s = new Student();
  // setting values to the object using setter
  s.name = "John Doe";
  s.classnumber = 12;

  // Display the values of the object
  s.display();

  // This will generate error
  //s.setClassNumber(13);
}
 Show Output
Why Is Setter Important?
It is used to set the value of a private property.
It is also used for data validation.
It gives you better control over the data.


GETTER AND SETTER IN DART
Introduction
In this section, you will learn about Getter and Setter in dart with the help of examples.

Getter And Setter
Getter and Setter provide explicit read and write access to an object properties. In dart, get and set are the keywords used to create getter and setter. Getter read the value of property and act as accessor. Setter update the value of property and act as mutator.

 Info
Note: You can use same name for getter and setter. But, you can’t use same name for getter, setter and property name.

Use Of Getter and Setter
Validate the data before reading or writing.
Restrict the read and write access to the properties.
Making the properties read-only or write-only.
Perform some action before reading or writing the properties.
Example 1: Getter And Setter In Dart

In this example below, there is a class named Student with three private properties _firstName, _lastName and _age. There are two getters fullName and age to get the value of the properties. There are also three setters firstName, lastName and age to update the value of the properties. If age is less than 0, it will throw an error.

class Student {
  // Private Properties
  String? _firstName;
  String? _lastName;
  int? _age;

  // Getter to get full name
  String get fullName => this._firstName! + " " + this._lastName!;

  // Getter to read private property _age
  int get age => this._age!;

  // Setter to update private property _firstName
  set firstName(String firstName) => this._firstName = firstName;

  // Setter to update private property _lastName
  set lastName(String lastName) => this._lastName = lastName;

  // Setter to update private property _age
  set age(int age) {
    if (age < 0) {
      throw new Exception("Age can't be less than 0");
    }
    this._age = age;
  }
}

void main() {
  // Create an object of Student class
  Student st = new Student();
  // setting values to the object using setter
  st.firstName = "John";
  st.lastName = "Doe";
  st.age = 20;
  // Display the values of the object
  print("Full Name: ${st.fullName}");
  print("Age: ${st.age}");
}
 Show Output
Example 2: Getter And Setter In Dart

In this example below, there is a class named BankAccount with one private property _balance. There is one getter balance to read the value of the property. There are methods deposit and withdraw to update the value of the _balance.

class BankAccount {
  // Private Property
  double _balance = 0.0;

  // Getter to read private property _balance
  double get balance => this._balance;

  // Method to deposit money
  void deposit(double amount) {
    this._balance += amount;
  }

  // Method to withdraw money
  void withdraw(double amount) {
    if (this._balance >= amount) {
      this._balance -= amount;
    } else {
      throw new Exception("Insufficient Balance");
    }
  }
}

void main() {
  // Create an object of BankAccount class
  BankAccount account = new BankAccount();
  // Deposit money
  account.deposit(1000);
  // Display the balance
  print("Balance after deposit: ${account.balance}");
  // Withdraw money
  account.withdraw(500);
  // Display the balance
  print("Balance after withdraw: ${account.balance}");
}
 Show Output
When To Use Getter And Setter
Use getter and setter when you want to restrict the access to the properties.
Use getter and setter when you want to perform some action before reading or writing the properties.
Use getter and setter when you want to validate the data before reading or writing the properties.
Don’t use getter and setter when you want to make the properties read-only or write-only.

INHERITANCE IN DART
Introduction
In this section, you will learn inheritance in Dart programming and how to define a class that reuses the properties and methods of another class.

Inheritance In Dart
Inheritance is a sharing of behaviour between two classes. It allows you to define a class that extends the functionality of another class. The extend keyword is used for inheriting from parent class.

 Info
Note: Whenever you use inheritance, it always create a is-a relation between the parent and child class like Student is a Person, Truck is a Vehicle, Cow is a Animal etc.

Dart supports single inheritance, which means that a class can only inherit from a single class. Dart does not support multiple inheritance which means that a class cannot inherit from multiple classes.


Syntax
class ParentClass {
  // Parent class code
}

class ChildClass extends ParentClass {
  // Child class code
}
In this syntax, ParentClass is the super class and ChildClass is the sub class. The ChildClass inherits the properties and methods of the ParentClass.

Terminology
Parent Class: The class whose properties and methods are inherited by another class is called parent class. It is also known as base class or super class.

Child Class: The class that inherits the properties and methods of another class is called child class. It is also known as derived class or sub class.


Example 1: Inheritance In Dart
In this example, we will create a class Person and then create a class Student that inherits the properties and methods of the Person class.

class Person {
  // Properties
  String? name;
  int? age;

  // Method
  void display() {
    print("Name: $name");
    print("Age: $age");
  }
}
// Here In student class, we are extending the
// properties and methods of the Person class
class Student extends Person {
  // Fields
  String? schoolName;
  String? schoolAddress;

  // Method
  void displaySchoolInfo() {
    print("School Name: $schoolName");
    print("School Address: $schoolAddress");
  }
}

void main() {
  // Creating an object of the Student class
  var student = Student();
  student.name = "John";
  student.age = 20;
  student.schoolName = "ABC School";
  student.schoolAddress = "New York";
  student.display();
  student.displaySchoolInfo();
}
 Show Output
Advantages Of Inheritance In Dart
It promotes reusability of the code and reduces redundant code.
It helps to design a program in a better way.
It makes code simpler, cleaner and saves time and money on maintenance.
It facilitates the creation of class libraries.
It can be used to enforce standard interface to all children classes.
Example 2: Inheritance In Dart
In this example, here is parent class Car and child class Toyota. The Toyota class inherits the properties and methods of the Car class.

class Car{
  String color;
  int year;

  void start(){
    print("Car started");
  }  
}

class Toyota extends Car{
  String model;
  int price;

  void showDetails(){
    print("Model: $model");
    print("Price: $price");
  }
}

void main(){
  var toyota = Toyota();
  toyota.color = "Red";
  toyota.year = 2020;
  toyota.model = "Camry";
  toyota.price = 20000;
  toyota.start();
  toyota.showDetails();
}
 Show Output
Types Of Inheritance In Dart
Single Inheritance - In this type of inheritance, a class can inherit from only one class. In Dart, we can only extend one class at a time.

Multilevel Inheritance - In this type of inheritance, a class can inherit from another class and that class can also inherit from another class. In Dart, we can extend a class from another class which is already extended from another class.

Hierarchical Inheritance - In this type of inheritance, parent class is inherited by multiple subclasses. For example, the Car class can be inherited by the Toyota class and Honda class.

Multiple Inheritance - In this type of inheritance, a class can inherit from multiple classes. Dart does not support multiple inheritance. For e.g. Class Toyota extends Car, Vehicle {} is not allowed in Dart.

Example 3: Single Inheritance In Dart
In this example below, there is super class named Car with two properties name and price. There is sub class named Tesla which inherits the properties of the super class. The sub class has a method display to display the values of the properties.

class Car {
  // Properties
  String? name;
  double? price;
}

class Tesla extends Car {
  // Method to display the values of the properties
  void display() {
    print("Name: ${name}");
    print("Price: ${price}");
  }
}

void main() {
  // Create an object of Tesla class
  Tesla t = new Tesla();
  // setting values to the object
  t.name = "Tesla Model 3";
  t.price = 50000.00;
  // Display the values of the object
  t.display();
}
 Show Output
Example 4: Multilevel Inheritance In Dart
In this example below, there is super class named Car with two properties name and price. There is sub class named Tesla which inherits the properties of the super class. The sub class has a method display to display the values of the properties. There is another sub class named Model3 which inherits the properties of the sub class Tesla. The sub class has a property color and a method display to display the values of the properties.

class Car {
// Properties
String? name;
double? price;
}

class Tesla extends Car {
// Method to display the values of the properties
void display() {
  print("Name: ${name}");
  print("Price: ${price}");
}
}

class Model3 extends Tesla {
// Properties
String? color;

// Method to display the values of the properties
void display() {
  super.display();
  print("Color: ${color}");
}
}

void main() {
// Create an object of Model3 class
Model3 m = new Model3();
// setting values to the object
m.name = "Tesla Model 3";
m.price = 50000.00;
m.color = "Red";
// Display the values of the object
m.display();
}
 Show Output
 Info
Note: Here super keyword is used to call the method of the parent class.

Example 5: Multilevel Inheritance In Dart
In this example below, there is class named Person with two properties name and age. There is sub class named Doctor with properties listofdegrees and hospitalname. There is another subclass named Specialist with property specialization. The sub class has a method display to display the values of the properties.

class Person {
  // Properties
  String? name;
  int? age;
}

class Doctor extends Person {
  // Properties
  List<String>? listofdegrees;
  String? hospitalname;

  // Method to display the values of the properties
  void display() {
    print("Name: ${name}");
    print("Age: ${age}");
    print("List of Degrees: ${listofdegrees}");
    print("Hospital Name: ${hospitalname}");
  }
}

class Specialist extends Doctor {
  // Properties
  String? specialization;

  // Method to display the values of the properties
  void display() {
    super.display();
    print("Specialization: ${specialization}");
  }
}

void main() {
  // Create an object of Specialist class
  Specialist s = new Specialist();
  // setting values to the object
  s.name = "John";
  s.age = 30;
  s.listofdegrees = ["MBBS", "MD"];
  s.hospitalname = "ABC Hospital";
  s.specialization = "Cardiologist";
  // Display the values of the object
  s.display();
}
 Show Output
Example 6: Hierarchical Inheritance In Dart
In this example below, there is class named Shape with two properties diameter1 and diameter2. There is sub class named Rectangle with method area to calculate the area of the rectangle. There is another subclass named Triangle with method area to calculate the area of the triangle.

class Shape {
  // Properties
  double? diameter1;
  double? diameter2;
}

class Rectangle extends Shape {
  // Method to calculate the area of the rectangle
  double area() {
    return diameter1! * diameter2!;
  }
}

class Triangle extends Shape {
  // Method to calculate the area of the triangle
  double area() {
    return 0.5 * diameter1! * diameter2!;
  }
}

void main() {
  // Create an object of Rectangle class
  Rectangle r = new Rectangle();
  // setting values to the object
  r.diameter1 = 10.0;
  r.diameter2 = 20.0;
  // Display the area of the rectangle
  print("Area of the rectangle: ${r.area()}");

  // Create an object of Triangle class
  Triangle t = new Triangle();
  // setting values to the object
  t.diameter1 = 10.0;
  t.diameter2 = 20.0;
  // Display the area of the triangle
  print("Area of the triangle: ${t.area()}");
}
 Show Output
Key Points
Inheritance is used to reuse the code.
Inheritance is a concept which is achieved by using the extends keyword.
Properties and methods of the super class can be accessed by the sub class.
Class Dog extends class Animal{} means Dog is sub class and Animal is super class.
The sub class can have its own properties and methods.
Why Dart Does Not Support Multiple Inheritance?
Dart does not support multiple inheritance because it can lead to ambiguity. For example, if class Apple inherits class Fruit and class Vegetable, then there may be two methods with the same name eat. If the method is called, then which method should be called? This is the reason why Dart does not support multiple inheritance.

What’s problem Of Copy Paste Instead Of Inheritance?
If you copy the code from one class to another class, then you will have to maintain the code in both the classes. If you make any changes in one class, then you will have to make the same changes in the other class. This can lead to errors and bugs in the code.

Does Inheritance Finished If I Learned Extending Class?
No, there is a lot more to learn about inheritance. You need to learn about Constructor Inheritance, Method Overriding, Abstract Class, Interface and Mixin etc. You will learn about these concepts in the next chapters.