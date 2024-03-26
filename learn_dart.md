# Dart

**Dart** is an open-source programming language developed by Google. It is used to create mobile, web and desktop applications. It is also used to develop server-side applications. Dart is a strongly typed language, which means that the compiler will detect any errors in the code before the code is compiled.
**Dart** is a programming language that is used to develop applications using the **Flutter** framework. 

*Flutter* is an open-source mobile application development framework that is built on top of the Dart programming language. It allows developers to build high-performance, visually attractive, and feature-rich mobile applications for Android, iOS, and web platforms.

The Dart language is object-oriented and supports features such as classes, interfaces, and mixins. It also includes a garbage collector to automatically free up memory used by objects that are no longer needed.

Flutter provides a set of pre-built widgets that can be used to create beautiful and responsive user interfaces. These widgets can be customized and combined to create complex UI elements such as buttons, forms, and dialog boxes


### Dart Features 
Dart also has several features that make it easier to learn and use compared to other languages. For example, it has a simple syntax and a flexible type system. It also has built-in support for asynchronous programming, which makes it easier to write code that runs concurrently. Below are interesting things about Dart:

- Free and open-source.
- Object-oriented programming language.
- Used to develop android, iOS, web, and desktop apps fast.
- Can compile to either native code or javascript.
- Offers modern programming features like null safety and asynchronous programming.
- You can even use Dart for servers and backend.


### Creating a basic Dart program
Creating a basic program in Dart that prints "Hello World" is a great way to get familiar with the Dart programming language. In this lesson, we will be walking through the steps to create a basic Dart program that prints "Hello World". 


Step 1: Create a New Dart Project

Once you have installed the Dart SDK, you can create a new Dart project. This can be done using an IDE (Integrated Development Environment) such as Visual Studio Code or IntelliJ, throughout this course we will be using VS Code. Once you have opened VS Code, you can create a new Dart project by selecting the “Open folder” option and select the folder where you want to store your dart program. 

Step 2: Write the Program

This is a simple dart program that prints Hello World on screen. Most programmers write the Hello World program as their first program.Lets do it!

Click the green play icon on the top right to run the program


void main() { 
   print("Hello World!"); 
}


Variables In Dart

Variables are containers used to store value in the program. There are different types of variables where you can keep different kinds of values. 

// here variable name contains value Ian.
var name = "Ian";

Variables Types In Dart
They are called data types. We will learn more about data types in the next lesson.
String: For storing text value. E.g. “Miriam” [Must be in quotes]
int: For storing integer value. E.g. 10, -10, 8555 [Decimal is not included]
double: For storing floating point values. E.g. 10.0, -10.2, 85.698 [Decimal is included]
num: For storing any type of number. E.g. 10, 20.2, -20 [both int and double]
bool: For storing true or false. E.g. true, false [Only stores true or false values]
var: For storing any value. E.g. ‘Bimal’, 12, ‘z’, true

Syntax to declare a variable

type variableName = value;

Dart variable Examples
In this example, you will learn how to declare variables and print their values.

void main() {
// declaring variables
String name = "John"; //must be in quotes
String address = "Kenya";  //must be in quotes
num age = 20; //whole numbers
num height = 5.9;//decimal numbers
bool isMarried = false; //boolean
   
// printing variables value   
print("Name is $name");
print("Address is $address");
print("Age is $age");
print("Height is $height");
print("Married Status is $isMarried");
}



Rules on declaring dart variables
Variable names are case sensitive, i.e., a and A are different.
A variable name can consist of letters and alphabets.
A variable name cannot start with a number.
Keywords are not allowed to be used as a variable name.
Blank spaces are not allowed in a variable name.
Special characters are not allowed except for the underscore (_) and the dollar ($) sign.

Comments in Dart

Comments are a great way to enhance the readability of your Dart code and make it easier to understand. In Dart, there are two types of comments: single-line and multi-line comments.

Single-line Comments

Single-line comments start with two forward slashes (//). Everything after the two forward slashes is ignored by the compiler. For example:


Multi-line Comments

Multi-line comments start with a forward slash and an asterisk (/*) and end with an asterisk and a forward slash (*/). Anything between the starting and ending delimiters is ignored by the compiler. For example:


 Data Types In Dart

Learning Objectives

1. To understand what data type is
2. To understand different data types in DART programming
3. Be able to code with the different data types
A data type is an attribute of data which tells the compiler or interpreter how the programmer intends to use the data.
Dart supports the following data types:
1. Number
2. Strings
3. Boolean
4. Lists
5. Maps
6. Runes
7. Null

Numbers
When you need to store numeric value on dart, you can use either int or double. Both int and double are subtypes of num. Int stores whole numbers while double stores decimal numbers.


void main() {
// Declaring Variables  
int num1 = 100; // without decimal point.
double num2 = 130.2; // with decimal point.
num num3 = 50;
num  num4 = 50.4;  

// For Sum   
num sum = num1 + num2 + num3 + num4;
   
// Printing Info   
print("Num 1 is $num1");
print("Num 2 is $num2");  
print("Num 3 is $num3");  
print("Num 4 is $num4");  
print("Sum is $sum");  
   
}


String
String helps you to store text data in your program. You can use single or double quotes to store string in dart.

void main() {
// Declaring Values     
String schoolName = "Powerlearn Project Academy";
String address = "AFRICA";   

// Printing Values
print("My School name is $schoolName and the address is $address");   
}


Booleans
In Dart, boolean holds either true or false value. You can write the bool keyword to define the boolean data type. You can use boolean if the answer is true or false. Consider the answer to the following questions:
Are you asleep?
Is the door open?
Does a cat fly?
Are you older than your father?
These all are yes/no questions. Its a good idea to store them in boolean.

void main() {
bool isMarried = true;
print("Married Status: $isMarried");
}


Lists
Dart List is similar to an array, which is the ordered collection of the objects. If you want to store multiple values without creating multiple variables, you can use a list.

void main() {
List<String> names = ["John", "James", "Peter"];
print("Value of names is $names");
print("Value of names[0] is ${names[0]}"); // index 0
print("Value of names[1] is ${names[1]}"); // index 1
print("Value of names[2] is ${names[2]}"); // index 2


print(names);
}


Maps
A map is a dynamic collection that represents a set of values ​as key-value pairs. Keys and values ​in the
map can be of any type.

void main() {
// Creating a Map with String keys and int values
Map<String, int> ages = {'Alice': 30,
'Bob': 25,
'Charlie': 35,
};
print("Ages of students: $ages");
}

Runes
A rune can be defined as an integer used to represent any Unicode code point. As a Dart string is a simple sequence of UTF-16 code units, 32-bit Unicode values in a string are represented using a special syntax.

void main() {
  // Define a string with runes
  String runesString = "Runes in Dart: \u{1F600} \u{1F64B} \u{1F680}";

  // Print the string
  print(runesString);

  //
}


Functions in Dart

 Functions are the block of code that performs a specific task. They are created when some statements are repeatedly occurring in the program. The function helps reusability of the code in the program.

Function Advantages
Avoid Code Repetition
Easy to divide the complex program into smaller parts
Helps to write a clean code
Syntax of a function
returntype functionName(parameter1,parameter2, ...){
// function body
}

Return type: It tells you the function output type. It can be void, String, int, double, etc. If the function doesn’t return anything, you can use void as the return type.
Function Name: You can name functions by almost any name. Always follow a lowerCamelCase naming convention like void printName().
Parameters: Parameters are the input to the function, which you can write inside the bracket (). Always follow a lowerCamelCase naming convention for your function parameter.

Example 1: Function That Prints Name
This is a simple program that prints name using function. The name of function is printName().


// writing function outside main function.
void printName(){
  print("My name John James");
}
// this is our main function.
void main(){
  printName();
}


Example 2: Function To Find Sum of Two Numbers
This function finds the sum of two numbers. Here, the function accepts two parameters. i.e., num1 and num2, and the return type is void.

void add(int num1, int num2){
  int sum = num1 + num2;
   print("The sum is $sum");
}

void main(){
  add(10, 20);
}


Key Points
In dart function are also objects.
You should follow the lowerCamelCase naming convention while naming function.
You should follow the lowerCamelCase naming convention while naming function parameters.

Types Of Functions
Functions are the block of code that performs a specific task. Here are different types of functions:
No Parameter And No Return Type
Parameter And No Return Type
No Parameter And Return Type
Parameter And Return Type

Function With No Parameter And No Return Type
In this function, you do not pass any parameter and expect no return type. Here is an example of it:

void main() {
  printName();
}

void printName() {
  print("My name is John James.");
}


Function With Parameter And No Return Type

In this function, you do pass the parameter and expect no return type. Here is an example of it:

Here printName(String name) is a function which welcome person

void main() {
  printName("John");
}

void printName(String name) {
  print("Welcome, ${name}.");
}


In this program, printName(String name) is the function which has keyword void. It means it has no return type, and the pair of parentheses is not empty but this time that suggests it to accept an parameter.

Function With No Parameter And Return Type
In this function, you do not pass any parameter but expect return type. Here is an example of it:
Here InstructorName() is a function which returns Instructor's name. In the entire program, anyone can use this function to find the name of the Instructor

void main() {
// Function With No Parameter & Return Type
  String name = InstructorsName();
  print("The Name from function is $name.");
}
String InstructorsName() {
  return "Allan Lenkaa";
}


In this program, InstructorsName() is the function which has String keyword before function name, means it return String value, and the empty pair of parentheses suggests that there is no parameter that is passed to the function.

Function With Parameter And Return Type
In this function, you do pass the parameter and also expect return type. Here is an example of it:

// this function add two numbers
int add(int a, int b) {
  int sum = a + b;
  return sum;
}

void main() {
  int num1 = 10;
  int num2 = 20;

  int total = add(num1, num2);
  print("The sum is $total.");
}

In this program, int add(int a, int b) is the function with int as the return type, and the pair of parenthesis has two parameters, i.e., a and b.


THE TYPES OF FUNCTIONS DISCUSSED

The code snippets below indicate all the functions. Use the comments as your guidelines.

// parameter and return type
int add(int a, int b) {
  var total;
  total = a + b;
  return total;
}

// parameter and no return type
void mul(int a, int b) {
  var total;
  total = a * b;
  print("Multiplication is : $total");
}

// no parameter and return type
String greet() {
  String greet = "Welcome";
  return greet;
}

// no parameter and no return type
void greetings() {
  print("Hello World!!!");
}

void main() {
  var total = add(2, 3);
  print("Total sum: $total");
  mul(2, 3);
  var greeting = greet();
  print("Greeting: $greeting");
  greetings();
}

Anonymous Functions 

In the previous lesson we introduced you to functions that are defined by using a function name like main(), fullName(). In this lesson we will talk about nameless functions or functions without a name. This type of function is known as an anonymous function, lambda, or closure. An anonymous function behaves the same as a regular function, but it does not have a name with it. It can have zero or any number of arguments / parameters with an option type annotation.

Syntax 
Below is the syntax of the anonymous function

Example 1:
In this example, you will learn to use an anonymous function to print all list items. This function invokes each fruit without having a function name.


void main() {
  const fruits = ["Apple", "Mango", "Banana", "Orange"];

  fruits.forEach((fruit) {
    print(fruit);
  });
}

Example 2:
In this example, we will use an anonymous function to print all list items.

void main() {
  // list of cars
  List cars = ["BMW", "BENZ", "AUDI", "TOYOTA"];

  // iteration with anonymous function as a parameter
  cars.forEach((car) {
    print(car); // printing an item
  });
}


Arrow Function
If you want to declare a function in one line; In Dart we have a fat arrow function that can enable you. The function is represented by => symbol. 

Syntax 
Below is the syntax for the arrow function

Knowledge Panel 
Note: The arrow function is used to make your code short. => expr syntax is a shorthand for { return expr; }.

Example 1: Calculation of simple interest without Arrow Function
This program finds simple interest without using the arrow function.

// function that calculate interest
double calculateInterest(double principal, double rate, double time) {
  double interest = principal * rate * time / 100;
  return interest;
}

void main() {
  double principal = 5000;
  double time = 3;
  double rate = 3;

  double result = calculateInterest(principal, rate, time);
  print("The simple interest is $result.");
}


Example 1: Calculation of simple interest WITH Arrow Function
// arrow function that calculate interest
double calculateInterest(double principal, double rate, double time) =>
    principal * rate * time / 100;

void main() {
  double principal = 5000;
  double time = 3;
  double rate = 3;

  double result = calculateInterest(principal, rate, time);
  print("The simple interest is $result.");
}


Data Types in Dart Technical Assignment
This technical assignment requires the creation of a program using the Dart programming language. The program should demonstrate an understanding of data types in Dart. Implement the data types you have learned in the previous lesson.
Requirements
The program should demonstrate an understanding of data types in Dart, including int, double, String, List, and Map.
The program should include at least one example of each data type.
The program should include comments to explain each data type and its use.
The program should be tested for accuracy and performance.


Dart Functions Assignment

In this assignment, you will be tasked with writing several functions in Dart.

Task 1
Write a function called addTwo that takes two numbers as arguments and returns the sum of those two numbers.
Task 2
Write a function called subtractTwo that takes two numbers as arguments and returns the difference of those two numbers.
Task 3
Write a function called multiplyTwo that takes two numbers as arguments and returns the product of those two numbers.
Task 4
Write a function called divideTwo that takes two numbers as arguments and returns the quotient of those two numbers.
Task 5
Write a function called stringLength that takes an argument of type String and returns the length of that string.
Task 6
Write a function called getFirstElement that takes a list as an argument and returns the first element of that list.

Please submit your assignment by pushing your code to GitHub and sharing the link to
https://forms.gle/Cz9V6W7pgcciuSY7A


Control Flow
The control statements or flow of control statements are used to control the flow of Dart program. These statements are very important in any programming languages to decide whether other statement will be executed or not. The code statement generally runs in the sequential manner. We may require executing or skipping some group of statements based on the given condition, jumps to another statement, or repeat the execution of the statements.

Categories of Flow Statement
In Dart, Control flow statement can be categorized mainly in three following ways.
Decision-making statements
Looping statements
Jump statements

Decision-making Statements
Dart provides following types of Decision-making statement.
If Statement
Executes a block of code if a specified condition is true.

// if statement outputs depending on a certain conditional expression
void main() {
  var age = 30;
  if (age > 18) {
    print("Mariam is a voter in Kenya");
  }
  //print("Mariam is still young to vote");
}

If-else Statements
In Dart, the if-else statement is used to execute a block of code based on whether a condition is true or false. Here's the syntax:

void main() {
  var age = 20;
  if (age > 18) {
    print("Mariam is a voter in Kenya");
  } 
  else {
    print("Mariam is still young to vote");
  }
}


If else if Statement

In Dart, the if-else if-else statement allows you to evaluate multiple conditions and execute different blocks of code based on these conditions. Here's the syntax:

void main() {
  var age = 18;
  if (age > 18) {
    print("Mariam is a voter in Kenya");
  } else if (age == 18) {
    print("Mariam just became eligible to vote in Kenya");
  } else {
    print("Mariam is still young to vote");
  }
}

/*
If age is greater than 18, the statement "Mariam is a voter in Kenya" will be printed.
If age is exactly 18, the statement "Mariam just became eligible to vote in Kenya" will be printed.
If neither of the above conditions is met, the statement "Mariam is still young to vote" will be printed.
*/ 


Switch Case Statement

In Dart, the switch statement is used to evaluate an expression and execute different blocks of code based on matching cases. The syntax of the switch statement is as follows:


void main() {
  int i = 11;
  switch (i) {
    case 1:
      print("The value is 1");
      break;
    case 2:
      print("The value is 2 ");
      break;
    case 3:
      print("the value is 3");
      break;
    default:
      print("The value is out of range ");
      break;
  }
}
//The code checks the value of variable i using a switch statement and prints a message based on its value, defaulting to an "out of range" message if none match.


Looping Statements

Dart Loop is used to run a block of code repetitively for a given number of times or until matches the specified condition. Loops are essential tools for any programming language. It is used to iterate the Dart iterable such as list, map, etc. and perform operations for multiple times. A loop can have two parts - a body of the loop and control statements. The main objective of the loop is to run the code multiple times. Dart supports the following type of loops.
Dart for loop
The for loop is used when we know how many times a block of code will execute.

//The for loop is used when we know how many times a block of code will execute
void main()  
{  
    int num = 1;  
    for(num; num<=3; num++)           //for loop to print 1-10 numbers  
    {  
        print(num);     //to print the number  
    }  
} 
// The code prints numbers from 1 to 10 using a for loop in Dart.


Dart for…in loop
The for..in loop is similar to for loop but different in its syntax. It iterates through an object's properties. The Dart for..in loop accepts an expression as iterator and iterates through the elements one at a time in sequence. The variable var holds the values of the iteration. The for…in will execute until elements remain in iterators.

void main()  
{  
    var list1 = [10,20,30,40,50];  
    for(var i in list1)           //for..in loop to print list element  
    {  
        print(i);       //to print the number  
    }  
}  //The code iterates over elements in the list list1 using a for-in loop and prints each element.

Dart while loop
The while loop is used when the number of execution of a block of code is not known. It will execute as long as the condition is true. It initially checks the given condition then executes the statements that are inside the while loop. The while loop is mostly used to create an infinite loop.

void main()  
{  
    var a = 1;  
           var maxnum = 11;  
           while(a<maxnum){        // it will print until the expression return false  
                         print(a);  
                         a = a+1;                                  // increase value 1 after each iteration  
}  
} 
//The code prints numbers from 1 to 10 using a while loop in Dart.

Dart do-while loop
Dart do while loop executes a block of the statement first and then checks the condition. If the condition returns true, then the loop continues its iteration. It is similar to Dart while loop but the only difference is, in the do-while loop a block of statements inside the body of loop will execute at least once.

void main()  
{  
 var a = 1;  
 var maxnum = 10;  
do  
    {                
       print("The value is: ${a}");  
       a = a+1;        // adding 1 to variable a after every sequence                            
       }
       while(a<maxnum);  
} 
//The code iteratively prints the value of variable a until it reaches 10, using a do-while loop in Dart.


Object Oriented Programming 

ram applications.
OOP is based on objects, which are data structures containing data and methods.
OOP is a way of thinking about programming that differs from traditional procedural programming.
OOP can make code more modular, flexible, and extensible.
OOP can help you to understand better and solve problems.


Classes

In object-oriented programming, a class is a blueprint for creating objects. A class defines the properties and methods that an object will have. For example, a class called Dog might have properties like breed, color and methods like bark, run.

Declaring A class in Dart
In Dart programming, you can declare a class using the class keyword followed by the class name. Here's a simple example:

class Dog {
  // Properties/attributes
  String breed;
  String color;
  String origin;

  // Constructor
  Dog(this.breed, this.color,this.origin);

  // Methods/behaviours
  void bark() {
    print('Woof!');
  }

  void run() {
    print('The dog is running.');
  }
}

void main() {
  // Creating an instance of the Dog class/object
  var myDog = Dog('Labrador', 'Golden','Siberian');

  // Accessing properties/attributes/characteristics
  print('Breed: ${myDog.breed}');
  print('Color: ${myDog.color}');
  print('Origin:${myDog.origin}');

  // Calling methods
  myDog.bark();
  myDog.run();
}


Brief explanation
Class Declaration (class Dog { ... }):

We declare a class named Dog using the class keyword.
Properties (String breed; String color;):

Inside the Dog class, we declare two properties: breed and color, both of type String. These properties will hold information about the breed and color of the dog.
Constructor (Dog(this.breed, this.color);):

We define a constructor for the Dog class.
The constructor takes two parameters, breed and color, and assigns them to the respective properties.
This shorthand constructor syntax Dog(this.breed, this.color); automatically initializes the properties with the provided values when a Dog object is created.
Methods (void bark() { ... }, void run() { ... }):

Inside the Dog class, we define two methods:
bark(): This method prints "Woof!" to simulate the sound of a dog barking.
run(): This method prints "The dog is running." to simulate the action of a dog running.
Main Function (void main() { ... }):

We define the main() function, which serves as the entry point of the Dart program.
Inside the main() function:
We create an instance of the Dog class using the constructor: var myDog = Dog('Labrador', 'Golden');
We access the properties of the myDog instance and print out its breed and color.
We call the bark() and run() methods on the myDog instance to simulate the behaviors of the dog.



Example with a class Person and their details
In this example below, there is class Person with four properties: name, phone, isMarried, and age. The class also has a method called displayInfo, which prints out the values of the four properties.


class Person {
  // Properties
  String name;
  String phone;
  bool isMarried;
  int age;

  // Constructor
  Person(this.name, this.phone, this.isMarried, this.age);

  // Method to display information
  void displayInfo() {
    print('Name: $name');
    print('Phone: $phone');
    print('Marital Status: ${isMarried ? 'Married' : 'Single'}');
    print('Age: $age');
  }
}

void main() {
  // Creating an instance of the Person class
  var person = Person('John Doe', '+1234567890', true, 30);

  // Calling the displayInfo method to print information
  person.displayInfo();
}

Example with a class Area

class Area {
  // Properties
  double length;
  double width;

  // Constructor
  Area(this.length, this.width);

  // Method to calculate area
  double calculateArea() {
    return length * width;
  }
}

void main() {
  // Creating an instance of the Area class
  var rectangle = Area(5.0, 3.0);

  // Calculating and printing the area
  print('Area of the rectangle: ${rectangle.calculateArea()} square units');
}


In this example:

We declare a class Area with properties length and width.
We define a constructor to initialize these properties.
We define a method calculateArea() to compute the area of the rectangle.
In the main() function, we create an instance of Area called rectangle with length 5.0 units and width 3.0 units.
We then call the calculateArea() method on the rectangle object to calculate its area and print the result.

KEY POINTS ON CLASS

1. The class keyword is used to declare the class.
2. The class serves as an object creation template.
3. Methods and properties make up the class body.
4. The terms fields, attributes, and data members are other terms for the properties.
5. The behaviors or member functions are another name for the methods.

Objects in DART
Programming in Dart is object-oriented; everything is handled as an object. A variable or instance of a class that is used to access the properties of the class is called an object. State and behavior are two characteristics of an object. Let's say a man is an item with a name, age, and level of health as well as a behavior (running, walking, and sleeping). Programming objects have states and behaviors, much like real-world things do in theory. A class is a template from which an object is produced.

Example given

// Define a class representing an Animal
class Animal {
  // Properties
  String name;
  String species;

  // Constructor
  Animal(this.name, this.species);
  
  // Method to make the animal sound
  void makeSound() {
    print('$name (${species}) makes a sound.');
  }
}

void main() {
  // Creating instances (objects) of the Animal class
  var cat = Animal('Whiskers', 'Cat');
  var dog = Animal('Buddy', 'Dog');

  // Accessing properties and behaviors
  print('${cat.name} is a ${cat.species}.');
  cat.makeSound();

  print('${dog.name} is a ${dog.species}.');
  dog.makeSound();
}


n this Dart code, we have a class called Animal, which acts as a blueprint for creating objects that represent different animals. Each Animal object has properties like name and species, and it can perform actions using methods like makeSound(). In our program, we create two instances (objects) of the Animal class: one representing a cat and another representing a dog. We set specific values for the properties of each object, such as their names and species. Then, we use the objects to call the makeSound() method, simulating the animals making sounds. This example demonstrates how classes and objects work together to model real-world entities in code.


A deep dive
Modern applications basically all do the same thing: they give us (smart humans) a way to process and collaborate over large data sets. Some apps are about communication, like social media and email. Some are about organization, such as calendars and note taking. Some are simply digital interfaces into a part of the real world that's hard for programmers to navigate, like dating apps. But they all do the same thing. They give users a nice way to interact with data.

Data represents the real world. All data describes something real. That's what object-oriented programming is all about: it gives us a nice way to model our data after real-world objects. It takes data, which dumb computers like, and adds some abstraction so smart humans can impose our will onto the computers. It makes code easy to read, easy to reason about, and highly reusable.

When writing Dart code, you'll likely want to create separate classes for everything that can represent a real-world "thing." Thing is a carefully chosen word, because it's so vague. (This is a great example of something that would make a dumb computer explode but that a smart human can make some sense of.)

Consider if we were writing a point-of-sale (POS) system used to sell goods to customers. What kinds of classes do you think you'd need to represent "things" (or data)? What kind of "things" does a POS app need to know about? Perhaps we need classes to represent a Customer, Business, Employee, Product, and Money. Those are all classes that represent real-world things. But it gets a bit hairier from here.
Ponder some questions with me:
We may want a class for Transaction and Sale. In real life, a transaction is a process or event. Should this be represented with a function or a class?
If we're selling bananas, should we use a Product class and give it a property that describes what type of product it is? Or should we have a Banana class?
Should we define a top-level variable or a class that has only a single property? For instance, if we need to write a function that simply adds two numbers together, should we define a Math class with an add method, or just write the method as a static, global variable?
Ultimately, these decisions are up to you, the programmer. There is no single right answer.
My rule of thumb is, "When in doubt, make a new class." Recall those previous questions: should a transaction be represented by a function of Business or its own class? I'd say make it a class. And that brings me all the way back to why I used the vague word thing earlier. A thing isn't just a physical object; it can be an idea, an event, a logical grouping of adjectives, and so on. In this example, I would make a class that looks like this:
class TransactionEvent {
// properties and methods
}
And that might be it. It might have no properties and no methods. Creating classes for events makes the type safety of Dart that much more effective.

The bottom line is that you can (and, I'd argue, should) make a class that represents any "thing" that isn't obviously an action you can do or a word you'd use to describe some detail of a "thing." For instance, you (a human) can exchange money with someone. It makes sense to say "I exchange money." It doesn't make sense to say, "I transaction," even though a transaction is an idea. Having a Transaction class makes sense, but an ExchangeMoney class doesn't.

Object Oriented Programming in DART
Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

Components of OOP,
Constructor
A constructor in programming is a special method or function that is automatically called when an object is created.
Initializes the object's properties or performs any desired configuration.
Constructors are essential for creating class instances in object-oriented programming.
In Dart, constructors are defined with the same name as the class.
There are two main types of constructors in dart:

Default constructor: A default constructor is automatically created if no other constructor is specified.
No parameter required.
Initializes instance variables to their default values ​​(null for objects, 0 for integers, etc.
).

class MyDetails {
  // Default constructor
  MyDetails() {
    // Initialization code, if needed
  }
}

void main() {
  // Creating an instance of MyDetails using the default constructor
  var myDetails = MyDetails();
}

In this example:
The MyDetails class has a default constructor, which doesn't take any parameters.
Inside the constructor, you can add any initialization code if needed.
In the main() function, an instance of MyDetails named myDetails is created using the default constructor.


Parameterized Constructors: Parameterized constructors allow you to pass a value during object creation, allowing you to initialize instance variables with specific values.

// Define a class named Dog
class Dog {
  // Declare instance variables for name, age, and breed
  String name;
  int age;
  String breed;

  // Parameterized constructor for the Dog class
  Dog(this.name, this.age, this.breed);

  // Method/ function  to make the dog bark
  void bark() => print("$name barks!");
  
  // Method to simulate the dog eating
  void eat() => print("$name is eating.");
  
  // Method to simulate the dog sleeping
  void sleep() => print("$name is sleeping.");
}

// Main function
void main() {
  // Create an instance(an object) of the Dog class named myDog
  Dog myDog = Dog("Buddy", 3, "Labrador");
  
  // Print information about the dog (name, age, breed)
  print("Name: ${myDog.name}, Age: ${myDog.age}, Breed: ${myDog.breed}");
  
  // Call the bark method of the Dog class
  myDog.bark();
  
  // Call the eat method of the Dog class
  myDog.eat();
  
  // Call the sleep method of the Dog class
  myDog.sleep();
}

Object Oriented Programming Paradigm
Data Encapsulation
Data encapsulation is the process of keeping a class' implementation details hidden from the user through an object's functions.
How To Achieve Encapsulation In Dart
Encapsulation can be achieved by:
Declaring the class properties as private by using underscore(_).
Providing public getter and setter methods to access and update the value of private property.

Getter and Setter Methods
Getter and setter methods are used to access and update the value of private property. Getter methods are used to access the value of private property. Setter methods are used to update the value of private property.


Code sample


class Circle {

// Private variable

double _radius;
//double radius;



// Constructor

Circle(this._radius);



// Getter for the radius

double get radius => _radius;

// Setter for the radius with validation

set radius(double value) {

if (value > 0) {

_radius = value;

} else {

print('Invalid radius. It must be greater than 0.');

}

}



// Method to calculate the area

double calculateArea() {

return 3.14 * _radius * _radius;

}

}



void main() {

// Create an instance/object  of the Circle class

Circle myCircle = Circle(5.0);



// Access the radius using the getter

print('Initial Radius of the Circle: ${myCircle.radius}');



// Update the radius using the setter(for updates)

myCircle.radius = 7.0;



// Access the updated radius and calculate the area

print('Updated/New  Radius: ${myCircle.radius}');

print('Area: ${myCircle.calculateArea()}');

}


Explanation
The Circle class has a private variable _radius, which is not directly accessible from outside the class.
The constructor initializes the _radius variable.
Getter (get radius) allows external code to access the value of _radius.
Setter (set radius) provides controlled access to update the value of _radius with validation.
The calculateArea method demonstrates how methods can use the encapsulated data.


Inheritance
Generally speaking, inheritance is the process of gaining properties. OOP allows for the inheritance of properties from one object to another.
Code sample


//PARENT CLASS VEHICLE

class Vehicle {
//PROPERTIES OF THE VEHICLE
String brand;

int year;
// CONSTRUCTOR HAVING THE VEHICLE'S PROPERTIES
Vehicle(this.brand, this.year);

void displayInfo() {

print('Vehicle Information is : $year $brand');

}

}


//INHERITANCE BEGINS 
// Derived class (inherits from Vehicle)

class Car extends Vehicle {
// CHILD PROPERTIES
String model;
//CHILD CONSTRUCTOR 
Car(String brand, this.model, int year) : super(brand, year);


// method showing childs information
void displayCarInfo() {

print('Car Information is : $year $brand $model');

}

}



void main() {

// Create an instance/object  of the Car class

Car myCar = Car('Toyota', 'Camry', 2022);



// Access and display information using methods from both Vehicle and Car classes

myCar.displayInfo();

myCar.displayCarInfo();

}


The Vehicle class is the base class with instance variables brand and year, and a method displayInfo.
The Car class is the derived class that extends (inherits from) the Vehicle class. It adds an additional property model and a method displayCarInfo.
The Car constructor uses super to call the constructor of the base class (Vehicle).
The main function demonstrates creating an instance of the Car class and accessing methods from both the base and derived classes.


Polymorphism
Polymorphism is the practice of having many classes use the same method name while redefining it for the derived classes.

class Animal {

void makeSound() {

print('All animals have a sound');

}

}



// Derived class 1

class Dog extends Animal {

@override

void makeSound() {

print('Woof!');

}

}



// Derived class 2

class Cat extends Animal {

@override

void makeSound() {

print('Meows!');

}

}



void main() {

// Create instances/objects  of the derived classes

Animal genericAnimal = Animal();

Dog myDog = Dog();

Cat myCat = Cat();



// Polymorphism in action

// The same method is called on different types of objects

genericAnimal.makeSound(); // Output: Some generic animal sound

myDog.makeSound(); // Output: Woof!

myCat.makeSound(); // Output: Meow!

}


Explanation
The Animal class is the base class with a method makeSound.
The Dog and Cat classes are derived classes that override the makeSound method with their own implementations.
In the main function, instances of Animal, Dog, and Cat are created.
The makeSound method is called on each object, demonstrating polymorphism as the appropriate version of the method is invoked based on the actual type of the object.


Abstraction
Abstraction refers to the user’s interaction with just a subset of an object’s characteristics and operations. To access a complicated item, abstraction uses simpler, high-level techniques.
Simple items are used to show complexity.
Keep complicated information hidden from the user.
Simple classes are used to indicate complexity in abstraction. Encapsulation is an extension of abstraction.
Advantages of Abstraction
It simplifies the process of seeing things in their entirety.
Code duplication is avoided, and reusability is increased.
Because just the most necessary information is shown to the user, it helps to enhance the security of an application or software.


// Abstract class

abstract class Shape {

// Abstract method to calculate area

double calculateArea();

// Concrete method

void printInfo() {

print('This is a shape.');

}

}



// Concrete class 1

class Circle extends Shape {

double radius;



Circle(this.radius);



@override

double calculateArea() {

return 3.14 * radius * radius;

}

}



// Concrete class 2

class Rectangle extends Shape {

double width, height;



Rectangle(this.width, this.height);



@override

double calculateArea() {

return width * height;

}

}



void main() {

// Create instances of concrete classes

Circle myCircle = Circle(5.0);

Rectangle myRectangle = Rectangle(4.0, 6.0);



// Use the common interface provided by the abstract class

print('Circle Area: ${myCircle.calculateArea()}');

print('Rectangle Area: ${myRectangle.calculateArea()}');



// Concrete method from the abstract class

myCircle.printInfo();

myRectangle.printInfo();

}


Explanation
The Shape class is an abstract class with an abstract method calculateArea() and a concrete method printInfo().
The Circle and Rectangle classes are concrete classes that extend the Shape class and provide implementations for the abstract method.
In the main function, instances of Circle and Rectangle are created and used through the common interface provided by the Shape abstract class.


Factory Methods

In Dart, factory constructors or methods are used to provide alternative ways to create instances of a class. They are useful when you need to control the instantiation process or return an instance of a subclass.
Factory constructors do use the return key word.
You cannot refer to 'this' within the factory constructor.

import 'dart:math';

class Circle {
  double radius;

  Circle(this.radius);

  // Factory method to create circles with different radii
  factory Circle.create(double radius) {
    if (radius <= 0) {
      throw ArgumentError('Radius must be positive.');
    }
    return Circle(radius);
  }

  // Method to calculate the area of the circle
  double calculateArea() {
    return pi * radius * radius;
  }
}

void main() {
  // Creating circles using the factory method
  var circle1 = Circle.create(5);
  var circle2 = Circle.create(7.5);

  // Calculating and printing the area of each circle
  print('Area of Circle 1: ${circle1.calculateArea()}');
  print('Area of Circle 2: ${circle2.calculateArea()}');
}


Explanation:
1.Circle Class:
The Circle class represents a circle with a given radius.
It has an instance variable radius to store the radius of the circle.
The constructor Circle(this.radius) initializes the radius variable when an instance of Circle is created
2.Factory Method:
The Circle class contains a factory method create that takes a radius parameter.
It ensures that the radius is positive and then creates and returns a new instance of Circle with the given radius.
If the provided radius is not positive, it throws an ArgumentError.
3.Calculate Area Method:
The calculateArea() method calculates the area of the circle using the formula pi * radius * radius.
4.Main Function:
In the main() function:We create instances of Circle using the factory method Circle.create() with different radii.
We call the calculateArea() method on each circle instance to calculate and print its area.


Singletons


The singleton pattern is a pattern used in object-oriented programming which ensures that a class has only one instance and also provides a global point of access to it. Sometimes it's important for a class to have exactly one instance, or you might force your app into a weird state. For example, you only want one instance of a class that represents your local storage, or you may end up with two different sources of data, which are out of sync. For the same reason, an operating system should have exactly one file system.

The idea is that anywhere in your code that you call MyClass(), it will return the same instance of that class, with the same state, etc. Thanks to factory constructors, implementing the singleton pattern in Dart is not only possible, but simple and flexible.


class FileSystemManager {
  // Static final variable to hold the single instance of the class
  static final FileSystemManager _instance = FileSystemManager._internal();

  // Private constructor for initialization logic
  FileSystemManager._internal() {
    // Initialization logic here
    print("Singleton instance created.");
  }

  // Factory constructor ensures only one instance is returned
  factory FileSystemManager() {
    return _instance;
  }
  
  void openFile() {
    print("File opened.");
  }
  
  void writeFile() {
    print("File written.");
  }
}

void main() {
  // Creating instances of FileSystemManager
  FileSystemManager manager1 = FileSystemManager();
  FileSystemManager manager2 = FileSystemManager();

  // Both instances will reference the same singleton instance
  print(manager1.hashCode == manager2.hashCode); // Output: true

  // Using methods of FileSystemManager
  manager1.openFile(); // Output: File opened.
  manager2.writeFile(); // Output: File written.
}


1.Singleton Design Pattern:
The FileSystemManager class is implemented using the Singleton design pattern, which ensures that there is only one instance of the class throughout the application's lifecycle.
2.Static Instance Variable:
The _instance variable is declared as static and final, meaning it is associated with the class itself rather than with instances of the class. This variable holds the single instance of the FileSystemManager class.
3.Private Constructor:
The _internal constructor is private, indicated by the underscore _, meaning it can only be accessed from within the FileSystemManager class. This constructor is used for initialization logic and is called only once to create the singleton instance of the class.
4.Factory Constructor:
The FileSystemManager class provides a factory constructor that ensures only one instance of the class is returned. This factory constructor checks if _instance is null, and if so, it creates a new instance using the private _internal constructor. Otherwise, it returns the existing instance.
5.Usage:
In the main() function, two instances of FileSystemManager named manager1 and manager2 are created.
The hashCode comparison confirms that both manager1 and manager2 reference the same singleton instance, as expected in a Singleton pattern.
The openFile() and writeFile() methods of FileSystemManager are called on manager1 and manager2, respectively, demonstrating that both instances share the same behavior implemented by the singleton instance.


Mixins

Mixins are a way of reusing a class’s code in different class hierarchies. For example, you might have a class called Employee which has methods like clockIn. The code in those classes may be useful for both Bartender and Nurse. But, now imagine you're introducing a class called Doctor. You probably have some functionality on Nurse (such as a method called takeTemperature) that you'd like on Doctor, but not that you want to add to Employee. This is a great place to use a mixin called Medical.

class Employee {
void clockIn() {...}
}

mixin Medical {
int takeTemperature {...}
}



// use mixins on your classes via the `with` keyword
class Nurse extends Employee with Medical {}
class Doctor extends Employee with Medical {
performSurgery() {...}
}
class Bartender extends Employee {}
With this architecture, your bartender can 'clock in', but cannot 'takeTemperature'. Both Nurse and Doctor can do both, and the doctor can performSurgery.

Extension Methods

Extension methods are new as of Dart 2.7. They allow you to add functionality to existing libraries and classes. For example, you can add extra functionality to the Dart core String library, that are only available in your app.extension on DateTime {
  String get humanize {
    // you have access to the instance in extension methods via 'this' keyword. 
    return "${this.day}/${this.month}/${this.year}";
  }
}

void main() {
  final dateTime = DateTime.now();
  print(dateTime.humanize);
}


Advanced Object-Oriented Programming in Dart Challenge

This challenge is designed to assess a learner's understanding of advanced object-oriented programming in Dart.

The challenge is to create a program that meets the following requirements:
Create two classes, one for a student and one for a teacher.
The student class should have a name, age and grade level.
The teacher class should have a name, age, and the subject they teach.
Create a method in the student class that prints out the student's information.
Create a method in the teacher class that prints out the teacher's information.
Create a third class that creates a student and teacher object, and calls the methods to print out the information.

Once the challenge is completed, the solution should be pushed to GitHub and the link should be submitted to https://forms.gle/wve1Lbk1ab8igLgQ9


Dart Utilities

TOPIC: Assignment

Technical Assignment Challenge: Dart Utilities

This technical assignment challenge is designed to assess a learner's understanding of Dart utilities. The assignment should be pushed to GitHub and the solution should be submitted via a link.

The challenge consists of the following tasks:
1. Create a function that takes two numbers as input and returns the sum of those numbers.
2. Write a program that uses a for loop to print out the numbers from 1 to 10.
3. Create a program that uses a switch statement to check for different string values and output a response based on the value.
4. Create a program that uses a while loop to print out the numbers from 20 to 10.
5. Create a program that uses an if-else statement to check if a number is even or odd and output the result.
6. Create a program that takes a list of numbers as input and outputs the largest number in the list.
7. Write a program that uses a try-catch block to catch an exception and output an error message.
