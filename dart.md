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

# DATA TYPES IN DART

Data types help you to categorize all the different types of data you use in your code. For e.g. numbers, texts, symbols, etc. The data type specifies what type of value will be stored by the variable. Each variable has its data type. Dart supports the following built-in data types :

1. Numbers
2. Strings
3. Booleans
4. Lists
5. Maps
6. Sets
7. Runes
9. Null
10. Built-In Types

In Dart language, there is the type of values that can be represented and manipulated. 

| |Data Type | Keyword |	Description |
| ----- | ---------- | ---------- | ---------- |
| 1. | Numbers |	int, double, num | It represents numeric values |
| 2. | Strings |	String | It represents a sequence of characters |
| 3. | Booleans | bool |	It represents Boolean values true and false |
| 4. | Lists |	List | It is an ordered group of items |
| 5. | Maps |	Map | It represents a set of values as key-value pairs |
| 6. | Sets |	Set | It is an unordered list of unique values of same types |
| 7. | Runes |	runes |	It represents Unicode values of String |
| 8. | Null |	null | It represents null value |


## 1. Numbers

When you need to store numeric value on dart, you can use either `int` or `double`. Both `int` and `double` are subtypes of `num`. You can use `num` to store both `int` or `double` value.

```
void main() {
// Declaring Variables  
int num1 = 100; // without decimal point.
double num2 = 130.2; // with decimal point.
num num3 = 50;
num  num4 = 50.4;  

// For Sum   
num sum = num1 + num2 + num3 + num4;
   
// Printing Info   
print("Num 1 is $num1");
print("Num 2 is $num2");  
print("Num 3 is $num3");  
print("Num 4 is $num4");  
print("Sum is $sum");  
   
} 
```

**Output**

```
Num 1 is 100
Num 2 is 130.2
Num 3 is 50
Num 4 is 50.4
Sum is 330.59999999999997
```


Round Double Value To 2 Decimal Places
The .toStringAsFixed(2) is used to round the double value upto 2 decimal places in dart. You can round to any decimal places by entering numbers like 2, 3, 4, etc.

void main() {
// Declaring Variables
double price = 1130.2232323233233; // valid.
print(price.toStringAsFixed(2));
}

**Output**

`1130.22` 

## 2. String
String helps you to store `text` data. You can store values like `I love dart`, `New York 2140` in String. You can use single or double quotes to store string in dart.

```
void main() {
// Declaring Values     
String schoolName = "Diamond School";
String address = "New York 2140";   

// Printing Values
print("School name is $schoolName and address is $address");   
}
```

**Output**

`School name is Diamond School and address is New York 2140`

#### Create A Multi-Line String In Dart
If you want to create a multi-line String in dart, then you can use `triple quotes` with either single or double quotation marks.

```
void main() {
// Multi Line Using Single Quotes   
String multiLineText = '''
This is Multi Line Text
with 3 single quote
I am also writing here.
''';
   
// Multi Line Using Double Quotes   
String otherMultiLineText = """
This is Multi Line Text
with 3 double quote
I am also writing here.
""";
   
// Printing Information   
print("Multiline text is $multiLineText");
print("Other multiline text is $otherMultiLineText");
} 
```

**Output**

```
Multiline text is This is Multi Line Text
with 3 single quote
I am also writing here.

Other multiline text is This is Multi Line Text
with 3 double quote
I am also writing here.
```

#### Special Character In String
| Special Character	| Work |
| ----- | ----- |
| \n |	New Line |
| \t |	Tab |


```
void main() {
   
// Using \n and \t   
print("I am from \nUS.");
print("I am from \tUS.");
}
```

**Output**

```
I am from 
US.
I am from 	US.
```

#### Create A Raw String In Dart
You can also create raw string in dart. Special characters won’t work here. You must write r after equal sign.

```
void main() {
// Set price value
num price = 10;
String withoutRawString = "The value of price is \t $price"; // regular String
String withRawString =r"The value of price is \t $price"; // raw String

print("Without Raw: $withoutRawString"); // regular result
print("With Raw: $withRawString"); // with raw result

}
```

**Output**

```
Without Raw: The value of price is 	 10
With Raw: The value of price is \t $price
```

## Type Conversion In Dart
In dart, type conversion allows you to convert one data type to another type. For e.g. to convert String to int, int to String or String to bool, etc.

1. Convert String To Int In Dart
You can convert String to int using int.parse() method. The method takes String as an argument and converts it into an integer.

```
void main() {
String strvalue = "1";
print("Type of strvalue is ${strvalue.runtimeType}");   
int intvalue = int.parse(strvalue);
print("Value of intvalue is $intvalue");
// this will print data type
print("Type of intvalue is ${intvalue.runtimeType}");
}
```

**Output**
```
Type of strvalue is String
Value of intvalue is 1
Type of intvalue is int
```

2. Convert String To Double In Dart
You can convert String to double using double.parse() method. The method takes String as an argument and converts it into a double.

```
void main() {
String strvalue = "1.1";
print("Type of strvalue is ${strvalue.runtimeType}");
double doublevalue = double.parse(strvalue);
print("Value of doublevalue is $doublevalue");
// this will print data type
print("Type of doublevalue is ${doublevalue.runtimeType}");
}
```

**Output**

```
Type of strvalue is String
Value of doublevalue is 1.1
Type of doublevalue is double
```

3. Convert Int To String In Dart
You can convert int to String using the toString() method. Here is example:

```
void main() {
int one = 1;
print("Type of one is ${one.runtimeType}");
String oneInString = one.toString(); 
print("Value of oneInString is $oneInString");
// this will print data type
print("Type of oneInString is ${oneInString.runtimeType}");
}
```

**Output**

```
Type of one is int
Value of oneInString is 1
Type of oneInString is String
```

4. Convert Double To Int In Dart
You can convert double to int using the toInt() method.

```
void main() { 
   double num1 = 10.01;
   int num2 = num1.toInt(); // converting double to int

  print("The value of num1 is $num1. Its type is ${num1.runtimeType}");
  print("The value of num2 is $num2. Its type is ${num2.runtimeType}");
}
```

**Output**

```
The value of num1 is 10.01. Its type is double
The value of num2 is 10. Its type is int
```

2. Booleans
In Dart, boolean holds either true or false value. You can write the bool keyword to define the boolean data type. You can use boolean if the answer is true or false. Consider the answer to the following questions:

Are you married?
Is the door open?
Does a cat fly?
Is the traffic light green?
Are you older than your father?
These all are yes/no questions. Its a good idea to store them in boolean.

```
void main() {
bool isMarried = true;
print("Married Status: $isMarried");
}
```

**Output**

`Married Status: true`

3. Lists

The list holds multiple values in a single variable. It is also called arrays. If you want to store multiple values without creating multiple variables, you can use a list.

```
void main() {
List<String> names = ["Raj", "John", "Max"];
print("Value of names is $names");
print("Value of names[0] is ${names[0]}"); // index 0
print("Value of names[1] is ${names[1]}"); // index 1
print("Value of names[2] is ${names[2]}"); // index 2

  // Finding Length of List 
int length = names.length;  
print("The Length of names is $length");
}
```

**Output**

```
Value of names is [Raj, John, Max]
Value of names[0] is Raj
Value of names[1] is John
Value of names[2] is Max
The Length of names is 3
```

Note: List index always starts with 0. Here names[0] is Raj, names[1] is John and names[2] is Max.

4. Sets
An unordered collection of unique items is called set in dart. You can store unique data in sets.


Note: Set doesn’t print duplicate items.

```
void main() {
Set<String> weekday = {"Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"};
print(weekday);
}
```

**Output**

`{Sun, Mon, Tue, Wed, Thu, Fri, Sat}`

5. Maps
In Dart, a map is an object where you can store data in key-value pairs. Each key occurs only once, but you can use same value multiple times.

```
void main() {
Map<String, String> myDetails = {
   'name': 'John Doe',
   'address': 'USA',
   'fathername': 'Soe Doe'
};
// displaying the output
print(myDetails['name']);
}
```

**Output**

`John Doe`

## Var Keyword In Dart
In Dart, var automatically finds a data type. In simple terms, var says if you don’t want to specify a data type, I will find a data type for you.

```
void main(){

var name = "John Doe"; // String
var age = 20; // int

print(name);
print(age);
}
```

**Output**

```
John Doe
20
```

6. Runes In Dart
With runes, you can find Unicode values of String. The Unicode value of a is 97, so runes give 97 as output.

```
void main() {

String value = "a";
print(value.runes);
}
```

**Output**

`(97)`

## How To Check Runtime Type
You can check runtime type in dart with .runtimeType after the variable name.

```
void main() { 
   var a = 10;
   print(a.runtimeType); 
   print(a is int); // true
}
```

**Output**

```
int
true
```

## Optionally Typed Language
You may have heard of the statically-typed language. It means the data type of variables is known at compile time. Similarly, dynamically-typed language means data types of variables are known at run time. Dart supports dynamic and static types, so it is called optionally-typed language.

## Statically Typed
A language is statically typed if the data type of variables is known at compile time. Its main advantage is that the compiler can quickly check the issues and detect bugs.

```
void main() { 
   var myVariable = 50; // You can also use int instead of var
   myVariable = "Hello"; // this will give error
   print(myVariable);
}
```

**Output**

```
Error:
A value of type 'String' can't be assigned to a variable of type 'int'.
```

## Dynamically Typed Example
A language is dynamically typed if the data type of variables is known at run time.

```
void main() { 
   dynamic myVariable = 50;
   myVariable = "Hello";
   print(myVariable);
}
```

**Output**

`Hello`

Note: Using static type helps you to prevent writing silly mistakes in code. It’s a good habit to use static type in dart.

Operators In Dart
Operators are used to perform mathematical and logical operations on the variables. Each operation in dart uses a symbol called the operator to denote the type of operation it performs. Before learning operators in the dart, you must understand the following things.

Operands : It represents the data.
Operator : It represents how the operands will be processed to produce a value.
 Info
Note: Suppose the given expression is 2 + 3. Here 2 and 3 are operands, and + is the operator.

Types Of Operators

There are different types of operators in dart. They are as follows:

Arithmetic Operators
Increment and Decrement Operators
Assignment Operators
Logical Operators
Type Test Operators
Arithmetic Operators
Arithmetic operators are the most common types of operators. They perform operations like addition, subtraction, multiplication, division, etc.

Operator Symbol	Operator Name	Description
+	Addition	For adding two operands
-	Subtraction	For subtracting two operands
-expr	Unary Minus	For reversing the sign of the expression
*	Multiplication	For multiplying two operands
/	Division	For dividing two operands and give output in double
~/	Integer Division	For dividing two operands and give output in integer
%	Modulus	Remainder After Integer Division
Let’s look at how to perform arithmetic calculations in dart.

void main() {
 // declaring two numbers 
 int num1=10;
 int num2=3;
 
 // performing arithmetic calculation
 int sum=num1+num2;       // addition
 int diff=num1-num2;      // subtraction
 int unaryMinus = -num1;    // unary minus  
 int mul=num1*num2;       // multiplication
 double div=num1/num2;    // division
 int div2 =num1~/num2;     // integer division
 int mod=num1%num2;       // show remainder
 
//Printing info 
 print("The addition is $sum.");
 print("The subtraction is $diff.");
 print("The unary minus is $unaryMinus.");
 print("The multiplication is $mul.");
 print("The division is $div.");
 print("The integer division is $div2.");
 print("The modulus is $mod."); 
}
 Show Output
Increment and Decrement Operators

With increment and decrement operators, you can increase and decrease values. If ++ is used at the beginning, then it is a prefix. If it is used at last, then it is postfix.

Operator Symbol	Operator Name	Description
++var	Pre Increment	Increase Value By 1. var = var + 1 Expression value is var+1
--var	Pre Decrement	Decrease Value By 1. var = var - 1 Expression value is var-1
var++	Post Increment	Increase Value By 1. var = var + 1 Expression value is var
var--	Post Decrement	Decrease Value By 1. var = var - 1 Expression value is var
 Info
Note: ++var increases the value of operands, whereas var++ returns the actual value of operands before the increment.

void main() {
// declaring two numbers 
 int num1=0;
 int num2=0;
 
// performing increment / decrement operator  

// pre increment   
num2 = ++num1;
print("The value of num2 is $num2");

// reset value to 0 
num1 = 0;
num2 = 0;

// post increment  
num2 =  num1++;
print("The value of num2 is $num2");  
  
}
 Show Output
Assignment Operators
It is used to assign some values to variables. Here, we are assigning 24 to the age variable.

int age = 24;
Operator Type	Description
=	Assign a value to a variable
+=	Adds a value to a variable
-=	Reduces a value to a variable
*=	Multiply value to a variable
/=	Divided value by a variable
void main() {
  double age = 24;
  age+= 1;  // Here age+=1 means age = age + 1.
  print("After Addition Age is $age");
  age-= 1;  //Here age-=1 means age = age - 1.
  print("After Subtraction Age is $age");
  age*= 2;  //Here age*=2 means age = age * 2.
  print("After Multiplication Age is $age");
  age/= 2;  //Here age/=2 means age = age / 2.
  print("After Division Age is $age");
}
 Show Output
Relational Operators
Relational operators are also called comparison operators. They are used to make a comparison.

Operator Symbol	Operator Name	Description
>	Greater than	Used to check which operand is bigger and gives result as boolean
<	Less than	Used to check which operand is smaller and gives result as boolean
>=	Greater than or equal to	Used to check which operand is bigger or equal and gives result as boolean
<=	Less than or equal to	Used to check which operand is smaller or equal and gives result as boolean
==	Equal to	Used to check operands are equal to each other and gives result as boolean
!=	Not equal to	Used to check operand are not equal to each other and gives result as boolean
void main() {
  
 int num1=10;
 int num2=5;
 //printing info
 print(num1==num2); 
 print(num1<num2);
 print(num1>num2);
 print(num1<=num2);
 print(num1>=num2);
}
 Show Output
Logical Operators
It is used to compare values.

Operator Type	Description
&&	This is ‘and’, return true if all conditions are true
||	This is ‘or’. Return true if one of the conditions is true
!	This is ’not’. return false if the result is true and vice versa
void main(){
  int userid = 123;
    int userpin = 456;

    // Printing Info
    print((userid == 123) && (userpin== 456)); // print true
    print((userid == 1213) && (userpin== 456)); // print false.
    print((userid == 123) || (userpin== 456)); // print true.
    print((userid == 1213) || (userpin== 456)); // print true
    print((userid == 123) != (userpin== 456));//print false

}
 Show Output
Type Test Operators
In Dart, type test operators are useful for checking types at runtime.

Operator Symbol	Operator Name	Description
is	is	Gives boolean value true if the object has a specific type
is!	is not	Gives boolean value false if the object has a specific type
void main() {
  String value1 = "Dart Tutorial";
  int age = 10;
  
  print(value1 is String);
  print(age is !int);
}
 Show Output


User Input In Dart
Instead of writing hard-coded values, you can give input to the computer. It will make your program more dynamic. You must import the package import 'dart:io'; for user input.

 Info
Note: You won’t be able to take input from users using dartpad. You need to run a program from your computer.

String User Input
They are used for storing textual user input. If you want to keep values like somebody’s name, address, description, etc., you can take string input from the user.

import 'dart:io';

void main() {
  print("Enter name:");
  String? name  = stdin.readLineSync();
  print("The entered name is ${name}");
}
 Show Output
Integer User Input

You can take integer input to get a numeric value from the user without the decimal point. E.g. 10, 100, -800 etc.

import 'dart:io';

void main() {
  print("Enter number:");
  int? number = int.parse(stdin.readLineSync()!);
  print("The entered number is ${number}");
}
 Show Output
Floating Point User Input
You can use float input if you want to get a numeric value from the user with the decimal point. E.g. 10.5, 100.5, -800.9 etc.

import 'dart:io';

void main() {
  print("Enter a floating number:");
  double number = double.parse(stdin.readLineSync()!);
  print("The entered num is $number");
}
 Show Output


STRING IN DART
String In Dart
String helps you to store text based data. In String, you can represent your name, address, or complete book. It holds a series or sequence of characters – letters, numbers, and special characters. You can use single or double, or triple quotes to represent String.

Example: String In Dart
Single line String is written in single or double quotes, whereas multi-line strings are written in triple quotes. Here is an example of it:

void main() {   
   String text1 = 'This is an example of a single-line string.';   
   String text2 = "This is an example of a single line string using double quotes.";   
   String text3 = """This is a multiline line   
string using the triple-quotes.
This is tutorial on dart strings.
""";   
   print(text1);  
   print(text2);   
   print(text3);   
}
 Show Output
String Concatenation

You can combine one String with another string. This is called concatenation. In Dart, you can use the + operator or use interpolation to concatenate the String. Interpolation makes it easy to read and understand the code.

String Concatenation In Dart
void main() {   
String firstName = "John";
String lastName = "Doe";
print("Using +, Full Name is "+firstName + " " + lastName+".");
print("Using interpolation, full name is $firstName $lastName.");  
  
}
 Show Output
Properties Of String
codeUnits: Returns an unmodifiable list of the UTF-16 code units of this string.
isEmpty: Returns true if this string is empty.
isNotEmpty: Returns false if this string is empty.
length: Returns the length of the string including space, tab, and newline characters.
String Properties Example In Dart
void main() {
   String str = "Hi";
   print(str.codeUnits);   //Example of code units
   print(str.isEmpty);     //Example of isEmpty
   print(str.isNotEmpty);  //Example of isNotEmpty
   print("The length of the string is: ${str.length}");   //Example of Length
}
 Show Output
Methods Of String
toLowerCase(): Converts all characters in this string to lowercase.
toUpperCase(): Converts all characters in this string to uppercase.
trim(): Returns the string without any leading and trailing whitespace.
compareTo(): Compares this object to another.
replaceAll(): Replaces all substrings that match the specified pattern with a given value.
split(): Splits the string at matches of the specified delimiter and returns a list of substrings.
toString(): Returns a string representation of this object.
substring(): Returns the text from any position you want.
codeUnitAt(): Returns the 16-bit UTF-16 code unit at the given index.
String Methods Example In Dart

Here you will see various string methods that can help your work a lot better and faster.

Converting String To Uppercase and Lowercase
You can convert your text to lower case using .toLowerCase() and convert to uppercase using .toUpperCase() method.

//Example of toUpperCase() and toLowerCase()
void main() { 
   String address1 = "Florida"; // Here F is capital
   String address2 = "TexAs"; // Here T and A are capital
   print("Address 1 in uppercase: ${address1.toUpperCase()}"); 
   print("Address 1 in lowercase: ${address1.toLowerCase()}"); 
   print("Address 2 in uppercase: ${address2.toUpperCase()}"); 
   print("Address 2 in lowercase: ${address2.toLowerCase()}"); 
}
 Show Output
Trim String In Dart
Trim is helpful when removing leading and trailing spaces from the text. This trim method will remove all the starting and ending spaces from the text. You can also use trimLeft() and trimRight() methods to remove space from left and right, respectively.

 Info
Note: The trim() method in Dart doesn’t remove spaces in the middle.

//Example of trim()
void main() { 
  String address1 = " USA"; // Contain space at leading.
  String address2 = "Japan  "; // Contain space at trailing. 
  String address3 = "New Delhi"; // Contains space at middle.
  
  print("Result of address1 trim is ${address1.trim()}");
  print("Result of address2 trim is ${address2.trim()}");
  print("Result of address3 trim is ${address3.trim()}");
  print("Result of address1 trimLeft is ${address1.trimLeft()}");
  print("Result of address2 trimRight is ${address2.trimRight()}");
}
 Show Output
Compare String In Dart
In Dart, you can compare two strings. It will give the result 0 when two texts are equal, 1 when the first String is greater than the second, and -1 when the first String is smaller than the second.

//Example of compareTo()
void main() { 
   String item1 = "Apple"; 
   String item2 = "Ant"; 
   String item3 = "Basket"; 
   
   print("Comparing item 1 with item 2: ${item1.compareTo(item2)}"); 
   print("Comparing item 1 with item 3: ${item1.compareTo(item3)}"); 
   print("Comparing item 3 with item 2: ${item3.compareTo(item2)}"); 
} 
 Show Output
Replace String In Dart
You can replace one value with another with the replaceAll(“old”, “new”) method in Dart. It will replace all the “old” words with “new”. Here in this example, this will replace milk with water.

//Example of replaceAll()
void main() { 
String text = "I am a good boy I like milk. Doctor says milk is good for health.";
  
String newText = text.replaceAll("milk", "water"); 
 
print("Original Text: $text");
print("Replaced Text: $newText");  
   
} 
 Show Output
Split String In Dart
You can use the dart split method if you want to split String by comma, space, or other text. It will help you to split String to list.

//Example of split()
void main() { 
  String allNames = "Ram, Hari, Shyam, Gopal";

  List<String> listNames = allNames.split(",");
  print("Value of listName is $listNames");

  print("List name at 0 index ${listNames[0]}");
  print("List name at 1 index ${listNames[1]}");
  print("List name at 2 index ${listNames[2]}");
  print("List name at 3 index ${listNames[3]}");
   
} 
 Show Output
ToString In Dart
In dart, toString() represents String representation of the value/object.

//Example of toString()
void main() { 
int number = 20;     
String result = number.toString(); 
  
print("Type of number is ${number.runtimeType}");  
print("Type of result is ${result.runtimeType}");  
    
}   
 Show Output
SubString In Dart
You can use substring in Dart when you want to get a text from any position.

//Example of substring()
void main() { 
   String text = "I love computer"; 
   print("Print only computer: ${text.substring(7)}"); // from index 6 to the last index 
   print("Print only love: ${text.substring(2,6)}");// from index 2 to the 6th index 
} 
 Show Output
Reverse String In Dart
If you want to reverse a String in Dart, you can reverse it using a different solution. One solution is here.

void main() { 
  String input = "Hello"; 
  print("$input Reverse is ${input.split('').reversed.join()}"); 
} 
 Show Output
How To Capitalize First Letter Of String In Dart
If you want to capitalize the first letter of a String in Dart, you can use the following code.

//Example of capitalize first letter of String
void main() { 
  String text = "hello world"; 
  print("Capitalized first letter of String: ${text[0].toUpperCase()}${text.substring(1)}"); 
} 
 Show Output

Basic Dart Practice Questions
Write a program to print your name in Dart.
Write a program to print Hello I am “John Doe” and Hello I’am “John Doe” with single and double quotes.
Declare constant type of int set value 7.
Write a program in Dart that finds simple interest. Formula= (p * t * r) / 100
Write a program to print a square of a number using user input.
Write a program to print full name of a from first name and last name using user input.
Write a program to find quotient and remainder of two integers.
Write a program to swap two numbers.
Write a program in Dart to remove all whitespaces from String.
Write a Dart program to convert String to int.
Suppose, you often go to restaurant with friends and you have to split amount of bill. Write a program to calculate split amount of bill. Formula= (total bill amount) / number of people
Suppose, your distance to office from home is 25 km and you travel 40 km per hour. Write a program to calculate time taken to reach office in minutes. Formula= (distance) / (speed)