NULL SAFETY IN DART
Null Safety
Null safety is a feature in the Dart programming language that helps developers to avoid null errors. This feature is called Sound Null Safety in dart. This allows developers to catch null errors at edit time.

Advantage Of Null Safety
Write safe code.
Reduce the chances of application crashes.
Easy to find and fix bugs in code.
 Info
Note: Null safety avoids null errors, runtime bugs, vulnerabilities, and system crashes which are difficult to find and fix.

Example 1: Using Null In Variables

In the example below, the variable age is a int type. If you pass a null value to this variable, it will give an error instantly.

void main() { 
   int age = null; // give error
}
 Show Output
Problem With Null
Programmers do have a lot of difficulties while handling null values. They forget that there are null values, so the program breaks. In real world null mostly acts as time bomb for programmers, which is ready to break the program.

 Info
Note: Common cause of errors in programming generally comes from not correctly handling null values.

Non-Nullable By Default

In Dart, variables and fields are non-nullable by default, which means that they cannot have a value null unless you explicitly allow it.

int productid = 20; // non-nullable
int productid = null; // give error
How To Declare Null Value
With dart sound null Safety, you cannot provide a null value by default. If you are 100% sure to use it, then you can use ? operator after the type declaration.

// Declaring a nullable variable by using ?
String? name;
This declares a variable name, which can be null or a string.

How To Assign Values To Nullable Variables
You can assign a value to nullable variables just like any other variable. However, you can also assign null to them.

void main(){
// Declaring a nullable variable by using ?
String? name;
// Assigning John to name
name = "John";
// Assigning null to name
name = null;
}
 Show Output
How To Use Nullable Variables
You can use nullable variables in many ways. Some of them are shown below:

You can use if statement to check whether the variable is null or not.
You can use ! operator, which returns null if the variable is null.
You can use ?? operator to assign a default value if the variable is null.
void main(){
// Declaring a nullable variable by using ?
String? name;
// Assigning John to name
name = "John";
// Assigning null to name
name = null;
// Checking if name is null using if statement
if(name == null){
print("Name is null");
}
// Using ?? operator to assign a default value
String name1 = name ?? "Stranger";
print(name1);
// Using ! operator to return null if name is null
String name2 = name!;
print(name2);
}
 Show Output
Example 2: Define List Of Nullable Items
You can also store null in list values. In this example, the items is a list of nullable integers. It can contain null values as well as integers.

void main() {
  // list of nullable ints
  List<int?> items = [1, 2, null, 4];
  print(items);
}
 Show Output
Example 3: Null Safety In Dart Functions
In this example, the function printAddress has a parameter address which is a String type. If you pass a null value to this function, it will give a edit-time error.

void printAddress(String address) {
  print(address);
}

void main() {
  printAddress(null); // give error
}
 Show Output
Example 4: Define Function With Nullable Parameter
If you are 100% sure, then you can use ? for the type declaration. In this example, the function printAddress has a parameter address, which is a String? type. You can pass both null and string values to this function.

// address is a nullable string
void printAddress(String? address) {
  print(address);
}
void main() {
  // Passing null to printAddress
  printAddress(null); // Works
}
 Show Output
Example 5: Null Safety In Dart Class
In the example, the class Person has a parameter name, which is a String type. If you pass a null value to this class, it will give a compile-time error.

class Person {
  String name;
  Person(this.name);
}

void main() {
  Person person = Person(null); // give error
}
 Show Output
Example 6: Define Null To Class Property
In this example, the class Person has a parameter name, which is a String? type. You can pass both null and string values to this class. To define a nullable property in a class, you can use the ? operator after the type.

class Person {
  String? name;
  Person(this.name);
}

void main() {
  Person person = Person(null); // Works
}
 Show Output
Example 7: Working With Nullable Class Properties
In the example below, the Profile class has two nullable properties: name and bio. The printProfile method prints the name and bio of the profile. If the name or bio is null, it prints a default value instead.

class Profile {
  String? name;
  String? bio;

  Profile(this.name, this.bio);

  void printProfile() {
    print("Name: ${name ?? "Unknown"}");
    print("Bio: ${bio ?? "None provided"}");
  }
}

void main() {
  // Create a profile with a name and bio
  Profile profile1 = Profile("John", "Software engineer and avid reader");
  profile1.printProfile();

  // Create a profile with only a name
  Profile profile2 = Profile("Jane", null);
  profile2.printProfile();

  // Create a profile with only a bio
  Profile profile3 = Profile(null, "Loves to travel and try new foods");
  profile3.printProfile();

  // Create a profile with no name or bio
  Profile profile4 = Profile(null, null);
  profile4.printProfile();
}
 Show Output
Important Point In Dart Null Safety
Null means no value.
Common error in programming is caused due to null.
Dart 2.12 introduced sound null Safety to solve null problems.
Non-nullable type is confirmed never to be null.
 Info
Note: Sometimes you heard word like NNBD. It is Non-Nullable By Default, which means you can’t assign null to a variable by default.


TYPE PROMOTION IN DART
Type Promotion In Dart
Type promotion in dart means that dart automatically converts a value of one type to another type. Dart does this when it knows that the value is of a specific type.

How Type Promotion Works In Dart?
Types Promotion in Dart works in the following ways:

Promoting from general types to specific subtypes.
Promoting from nullable types to non-nullable types.
Example 1: Promoting From General Types To Specific Subtypes

In this example, the variable name is declared as an Object. The Object class doesn’t have a .length property. Variable name gets promoted from Object to String so that you can access the .length property of the String class.

void main(){
Object name = "Pratik";
// print(name.length) will not work because Dart doesn't know that name is a String

if(name is String) {
// name promoted from Object to String
  print("The length of name is ${name.length}");
}
}
 Show Output
Example 2: Type Promotion In Dart
In this example, the variable result is declared as a String. In both if and else blocks, the variable result is assigned a value of type String. Therefore, the variable result is automatically promoted to a non-nullable type String.

void main(){
// result is a String
String result;
// result is promoted to a non-nullable type String
if(DateTime.now().hour < 12) {
  result = "Good Morning";
} else {
  result = "Good Afternoon";
}
// display the result
print("Result is $result");
print("Length of result is ${result.length}");
}
 Show Output
Example 3: Type Promotion With Nullable To Non-Nullable Type

In Dart, you can also throw an exception if the variable is null. In this example, method printLength, takes a String type parameter. If the parameter is null, then it will throw an exception.

// method to print the length of the text
void printLength(String? text){
    if(text == null) {
        throw Exception("The text is null");
    }
    print("Length of text is ${text.length}");
}
// main method
void main() {
    printLength("Hello");
}
 Show Output
Example 4: Type Promotion With Nullable Type To Non-Nullable Type
In this example, the variable value contains a value of type String or null. The variable value is promoted to a non-nullable type String in the if block. If the variable value is null, then the else block is executed.

// importing dart:math library
import 'dart:math';
// creating a class DataProvider
class DataProvider{
    // creating a method stringorNull
    String? get stringorNull => Random().nextBool() ? "Hello" : null;

    // creating a method myMethod
    void myMethod(){
        String? value = stringorNull;
        // checking if value String or not
        if(value is String){
            print("The length of value is ${value.length}");
        }else{
            print("The value is not string.");
        }

    }
}
// main method
void main() {
    DataProvider().myMethod();
}
 Show Output
 Info
Note: The output of the above example is random. It can be either The length of value is 5 or The value is not string.


LATE KEYWORD IN DART
Late Keyword In Dart
targets

In dart, late keyword is used to declare a variable or field that will be initialized at a later time. It is used to declare a non-nullable variable that is not initialized at the time of declaration.

Example 1: Late Keyword In Dart
In this example, name variable is declared as a late variable. The name variable is initialized in the main method.

// late variable
late String name;

void main() {
  // assigning value to late variable
  name = "John";
  print(name);
}
targets

 Show Output
When you put late infront of a variable declearation, you tell Dart the following:

Don’t assign that variable a value yet.
You will assign value later.
You will make sure the variable has a value before you use it.
 Info
Note: The late keyword is contract between you and Dart. You are telling Dart that you will assign a value to the variable before you use it. If you don’t assign a value to the variable before you use it, Dart will throw an error.

Example 2: Late Keyword In Dart
In this example, there is Person class with a name field. The name field is declared as a late variable.

class Person {
  // late variable
  late String name;

  void greet() {
    print("Hello $name");
  }
}

void main() {
  Person person = Person();
  // late variable is initialized here
  person.name = "John";
  person.greet();
}
targets

 Show Output
Usecase of Late Keyword In Dart

Dart late keyword has two use cases:

Declaring a non-nullable variable or field that is not initialized at the point of declaration.
Lazy initialization of a variable or field.
What Is Lazy Initialization
Lazy initialization is a design pattern that delays the creation of an object, the calculation of a value, or some other expensive process until the first time you need it.

 Info
Note: Using late means dart doesn’t initialize value right away, it only initializes when you access it for the first time. This is also called lazy loading.

Example 3: Late Keyword In Dart
In this example, the provideCountry function is not called when the value variable is declared. The provideCountry function is called only when the value variable is used. Lazy initialization is used to avoid unnecessary computation.

// function
String provideCountry() {
  print("Function is called");
  return "USA";
}

void main() {
  print("Starting");
  // late variable
  late String value = provideCountry();
  print("End");
  print(value);
}
targets

Guess the output before clicking on the Show Output button. If you remove the late keyword from the value variable, the provideCountry function will be called when the value variable is declared.


 Show Output
Example 4: Late Keyword In Class
In this example, the heavyComputation function is called when the description variable is used. If you remove the late keyword from the description variable, the heavyComputation function will be called when the Person class is instantiated.

// Person class
class Person {
  final int age;
  final String name;
  late String description = heavyComputation();

// constructor
  Person(this.age, this.name) {
    print("Constructor is called");
  }
// method
  String heavyComputation() {
    print("heavyComputation is called");
    return "Heavy Computation";
  }
}

void main() {
  // object of Person class
  Person person = Person(10, "John");
  print(person.name);
  print(person.description); 
}
targets

 Show Output
Example 5: Late Keyword In Class
In this example, the _getFullName function is called when the fullName variable is used. The firstName and lastName variables are initialized when the fullName variable is used.

class Person {
  // declaring late variables
  late String fullName = _getFullName();
  late String firstName = fullName.split(" ").first;
  late String lastName = fullName.split(" ").last;

// method
  String _getFullName() {
    print("_getFullName is called");
    return "John Doe";
  }
}
// main method
void main() {
  print("Start");
  Person person = Person();
  print("First Name: ${person.firstName}");
  print("Last Name: ${person.lastName}");
  print("Full Name: ${person.fullName}");
  print("End");
}
targets

 Show Output
 Info
Note: If you remove the late keyword from the fullName variable, the _getFullName function will be called when the Person class is instantiated.

Late Final Keyword In Dart
If you want to assign a value to a variable only once, you can use the late final keyword. This is useful when you want to initialize a variable only once.

Example 6: Late Final Keyword In Dart
In this example, there is class Student with a name field. The name field is declared as a late final variable. The name field is initialized in the Student constructor. The name field is assigned a value only once. If you try to assign a value to the name field again, you will get an error.

// Student class
class Student {
  // late final variable
  late final String name;

  // constructor
  Student(this.name);
}

void main() {
  // object of Student class
  Student student = Student("John");
  print(student.name);
  student.name = "Doe"; // Error
}
targets

 Show Output


NULL SAFETY EXERCISE
Null Safety Exercise
Practice these exercises to master dart null safety. To practice these exercises, click on Run Online button and solve the problem.

Exercise 1: Null Safety In Dart
In variable name age, assign a null value to it using ?.

// Try to assign a null value to age variable using ?
void main() {
  int age;
  age = null;
  print("Age is $age");
}
Exercise 2: Nullable Type Parameter For Generics

Try using ? to make the type parameter of List nullable.

// Try to make the type parameter of List nullable
void main() {
  List<int> items = [1, 2, null, 4];
  print(items);
}
Exercise 3: Null Assertion Operator (!)
Try using null assertion operator ! to print null if the variable is null.

// Try to use null assertion operator(!) to print null if the variable is null
void main() {
  String? name;
  name = null;
  String name1 = name;
  print(name1);
}
Exercise 4: Null Assertion Operator (!) For Generics

Try using null assertion operator ! to print null if the variable is null.

// Try to use null assertion operator(!) to print null if the variable is null
void main() {
  List<int?> items = [1, 2, null, 4];
 
  int firstItem = items.first;
  
  print(firstItem);
}
Exercise 5: Null Assertion Operator (!) For Generics
Try using null assertion operator ! to print null if the variable is null.

// Try to use null assertion operator(!) to print null if the variable is null
int? returnNullButSometimesNot() {
  return -5;
}

void main() {
 int result = returnNullButSometimesNot().abs();
 print(result);
}
**Exercise 6: Null Assertion Operator (!) **
Try using null assertion operator ! to print the length of the String or return null if the variable is null.

// Try to use null assertion operator(!) to print the length of the String or return null if the variable is null
int findLength(String? name) {
    // add null assertion operator here
  return name.length;
}

void main() {
  int? length = findLength("Hello");
  print("The length of the string is $length");
}
Exercise 7: Null Coalescing Operator (??)
If you want to assign a default value to a variable if it is null, you can use null coalescing operator ??.

Try using null coalescing operator ?? to assign a default value to Stranger if it is null.

// Try to use null coalescing operator(??) to assign a default value to Stranger if it is null
void main() {
  String? name;
  name = null;
  String name1 = name;
  print(name1);
}
Exercise 8: Type Promotion
Solve the error using type promotion:

// Try to solve the error using type promotion
Object name = "Mark";
print("The length of name is ${name.length}");
Exercise 9: Type Promotion
Solve the error using type promotion:

// Try to solve the error using type promotion
import 'dart:math';
class DataProvider{
    String? get stringorNull => Random().nextBool() ? "Hello" : null;

    void myMethod(){
        if(stringorNull is String){
            print("The length of value is ${stringorNull.length}");
        }else{
            print("The value is not string.");
        }

    }
}

void main() {
    DataProvider().myMethod();
}
Exercise 10: Late Keyword
Try using late keyword to solve the error:

// Try to solve the error using late keyword
class Person{
    String _name;

    void setName(String name){
        _name = name;
    }

    String get name => _name;
}

void main() {
    Person person = Person();
    person.setName("Mark");
    print(person.name);
}



Question For Practice 7
What is the purpose of the ? operator in Dart null safety?
Create a late variable named address, assign a US value to it and print it.
How do you declare a nullable type in Dart null safety?
Write a program in a dart to create an age variable and assign a null value to it using ?.
Write a function that accepts a nullable int parameter and returns 0 if the value is null using null coalescing operator ??.
Write a function named generateRandom() in dart that randomly returns 100 or null. Also, assign a return value of the function to a variable named status that can’t be null. Give status a default value of 0, if generateRandom() function returns null.