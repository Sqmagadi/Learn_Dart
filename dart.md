# Dart
Dart is an open-source, client-optimized, object-oriented programming language built by google to build apps fast for many platforms like android, iOS, web, desktop, etc. Dart is a strongly typed language, which means that the compiler will detect any errors in the code before the code is compiled.

## Dart Features
- Free and open-source.
- Object-oriented programming language.
- Used to develop android, iOS, web, and desktop apps fast.
- Can compile to either native code or javascript.
- Offers modern programming features like null safety and asynchronous programming.
- You can even use Dart for servers and backend.


### Code Editor 
The best code editor is VS Code if you want to run the dart program from a computer or laptop. You can download the dart extension from VS Code and start coding. 

You can also use other code editors such as **intelij**

For practice you can use **Dartpad**

### Dart History
- Google developed Dart in 2011 as an alternative to javascript.
- Dart 1.0 was released on November 14, 2013.
- Dart 2.0 was released in August 2018.
- Dart 3.0 was released in May 2023.
- Dart gained popularity in recent days because of flutter.


# Dart Installation
You can install Dart on Windows, Mac, and Linux or run it from the browser.

### Steps:

1. Download Dart SDK from here.
2. Copy dart-sdk folder to your C drive.
3. Add C:\dart-sdk\bin to your environment variable. Watch the video below to be more clear.
4. Open the command prompt and type dart --version to check it.
5. Install VS Code and Add Dart Extension.


# Basic Dart Program

### Steps To Create Dart Project

1. Open folder location on command prompt/terminal.
2. Type dart create project_name (For E.g. dart create first_app)
3. Type cd first_app
4. Type code . to open project with visual studio code
5. To check the main dart file go to bin/first_app.dart and edit your code.

Once you have installed the Dart SDK, you can create a new Dart project. This can be done using an IDE (Integrated Development Environment) such as Visual Studio Code or IntelliJ.

Name your file with a `.dart` extension

`myapp.dart`

6. Write the Program

```
void main() { 
   print("Hello World!"); 
}
```

- This is a simple dart program that prints *Hello World* on screen.
- **void main()**is the starting point where the execution of your program begins.
- Every program starts with a **main** function.
- The curly braces **{}** represent the beginning and the ending of a block of code.
- **print(“Hello World!”);** prints Hello World! on screen.
- Each code statement must end with a semicolon (**;**).


7. Run Dart Project
First, open the project location on the command/terminal and run the project with this command.

`dart run`

# Comments in Dart

Comments are a great way to enhance the readability of your Dart code and make it easier to understand. In Dart, there are two types of comments: **single-line** and **multi-line** comments.

*Single-line Comments*

Single-line comments start with two forward slashes (`//`). Everything after the two forward slashes is ignored by the compiler. 

```
void main() {
// declaring variables
String name = "John"; 
   
// printing variables value   
print("Name is $name");
}
```

*Multi-line Comments*

Multi-line comments start with a forward slash and an asterisk (`/*`) and end with an asterisk and a forward slash (`*/`). Anything between the starting and ending delimiters is ignored by the compiler. 

```
void main() {
// declaring variables
String name = "John"; 

/* String address = "Kenya";  
num age = 20; 
num height = 5.9;
bool isMarried = false;  */
   
// printing variables value   
print("Name is $name");
}
```

# VARIABLES IN DART

Variables are containers used to store value in the program. There are different types of variables where you can keep different kinds of values. 

```
// here variable name contains value John.
var name = "John"; 
```

### Variable Types

1. String: For storing text value. E.g. “John” [Must be in quotes]
2. int: For storing integer value. E.g. 10, -10, 8555 [Decimal is not included]
3. double: For storing floating point values. E.g. 10.0, -10.2, 85.698 [Decimal is included]
4. num: For storing any type of number. E.g. 10, 20.2, -20 [both int and double]
5. bool: For storing true or false. E.g. true, false [Only stores true or false values]
6. var: For storing any value. E.g. ‘Bimal’, 12, ‘z’, true

### Syntax

`type variableName = value;`

Example 1: Using Variables In Dart

```
void main() {
// declaring variables
String name = "John";
String address = "USA";  
num age = 20; // used to store any types of numbers 
num height = 5.9;
bool isMarried = false;
   
// printing variables value   
print("Name is $name");
print("Address is $address");
print("Age is $age");
print("Height is $height");
print("Married Status is $isMarried");
}
```

### Rules For Creating Variables In Dart
- Variable names are case sensitive, i.e., a and A are different.
- A variable name can consist of letters and alphabets.
- A variable name cannot start with a number.
- Keywords are not allowed to be used as a variable name.
- Blank spaces are not allowed in a variable name.
- Special characters are not allowed except for the underscore (_) and the dollar ($) sign.

### Dart Constant

Constant is the type of variable whose value never changes. In programming, changeable values are mutable and unchangeable values are immutable. Sometimes, you don’t need to change the value once declared. Like the value of PI=3.14, it never changes. To create a constant in Dart, you can use the const keyword.

```
void main(){
const pi = 3.14;
pi = 4.23; // not possible  
print("Value of PI is $pi");
}
```

### Naming Convention For Variables In Dart
It is a good habit to follow the naming convention. In Dart Variables, the variable name should start with lower-case, and every second word’s first letter will be upper-case like num1, fullName, isMarried, etc. Technically, this naming convention is called *lowerCamelCase*.

```
Naming Convention Example
// Not standard way
var fullname = "John Doe";
// Standard way
var fullName = "John Doe";
const pi = 3.14;
```