Function In Dart
In this tutorial, you will learn about functions in dart. Functions are the block of code that performs a specific task. They are created when some statements are repeatedly occurring in the program. The function helps reusability of the code in the program.

 Info
Note: The main objective of the function is DRY(Don’t Repeat Yourself).

Function Advantages
Avoid Code Repetition
Easy to divide the complex program into smaller parts
Helps to write a clean code
Syntax
returntype functionName(parameter1,parameter2, ...){
  // function body
}
Return type: It tells you the function output type. It can be void, String, int, double, etc. If the function doesn’t return anything, you can use void as the return type.


Function Name: You can name functions by almost any name. Always follow a lowerCamelCase naming convention like void printName().

Parameters: Parameters are the input to the function, which you can write inside the bracket (). Always follow a lowerCamelCase naming convention for your function parameter.

Example 1: Function That Prints Name
This is a simple program that prints name using function. The name of function is printName().

// writing function outside main function.
void printName(){
  print("My name is Raj Sharma. I am from function.");
}
// this is our main function.
void main(){
  printName();
}
 Show Output
Example 2: Function To Find Sum of Two Numbers

This function finds the sum of two numbers. Here, the function accepts two parameters. i.e., num1 and num2, and the return type is void.

void add(int num1, int num2){
  int sum = num1 + num2;
   print("The sum is $sum");
}

void main(){
  add(10, 20);
}
 Show Output
Example 3: Function That Find Simple Interest
This function finds simple interest from principal, time and rate and display result.

// function that calculate interest
void calculateInterest(double principal, double rate, double time) {
  double interest = principal * rate * time / 100;
  print("Simple interest is $interest");
}

void main() {
  double principal = 5000;
  double time = 3;
  double rate = 3;
  calculateInterest(principal, rate, time);
}
 Show Output
Challenge
Create a function that finds a cube of numbers.

Key Points
In dart function are also objects.
You should follow the lowerCamelCase naming convention while naming function.
You should follow the lowerCamelCase naming convention while naming function parameters.
About lowerCamelCase
Name should start with lower-case, and every second word’s first letter will be upper-case like num1, fullName, isMarried, etc. Technically, this naming convention is called lowerCamelCase.

Function Parameters Vs Arguments
Many programmers are often confused about parameters and arguments. Let’s have a look at this example.

// Here num1 and num2 are parameters
void add(int num1, int num2){
  int sum;
  sum = num1 + num2;
   
  print("The sum is $sum");
}

void main(){
// Here 10 and 20 are arguments
  add(10, 20);
}
 Show Output
Here in add(int num1, int num2), num1 and num2 are parameters and in add(10, 20), 10 and 20 are arguments.
Parameter is the name and data type you define as an input for your function.
Argument is the actual value that you passed in.
 Info
Note: In dart, if you don’t write the return type of function. It will automatically understand.


TYPES OF FUNCTIONS IN DART
Types Of Function
Functions are the block of code that performs a specific task. Here are different types of functions:

No Parameter And No Return Type
Parameter And No Return Type
No Parameter And Return Type
Parameter And Return Type
Function With No Parameter And No Return Type
In this function, you do not pass any parameter and expect no return type. Here is an example of it:

Example 1: No Parameter & No Return Type

Here printName() is a function which prints name on screen.

void main() {
  printName();
}

void printName() {
  print("My name is John Doe.");
}
 Show Output
In this program, printName() is the function which has keyword void. It means it has no return type, and the empty pair of parentheses implies that there is no parameter that is passed to the function.

Example 2: No Parameter & No Return Type
Here printPrimeMinisterName() is a function which prints prime minister name on screen.

void main() {
  print("Function With No Parameter and No Return Type");
  printPrimeMinisterName();
}

void printPrimeMinisterName() {
  print("John Doe.");
}
 Show Output
Function With Parameter And No Return Type

In this function, you do pass the parameter and expect no return type. Here is an example of it:

Example 1: Parameter & No Return Type
Here printName(String name) is a function which welcome person.

void main() {
  printName("John");
}

void printName(String name) {
  print("Welcome, ${name}.");
}
 Show Output
In this program, printName(String name) is the function which has keyword void. It means it has no return type, and the pair of parentheses is not empty but this time that suggests it to accept an parameter.

Example 2: Parameter & No Return Type
Here add(int a, int b) is a function that finds and prints the sum of two numbers.

// This function add two numbers
void add(int a, int b) {
  int sum = a + b;
  print("The sum is $sum");
}

void main() {
  int num1 = 10;
  int num2 = 20;

  add(num1, num2);
}
 Show Output
Function With No Parameter And Return Type
In this function, you do not pass any parameter but expect return type. Here is an example of it:

Example 1: No Parameter & Return Type
Here primeMinisterName() is a function which returns prime minister name. In the entire program, anyone can use this function to find the name of the prime minister.

void main() {
// Function With No Parameter & Return Type
  String name = primeMinisterName();
  print("The Name from function is $name.");
}
String primeMinisterName() {
  return "John Doe";
}
 Show Output
In this program, primeMinisterName() is the function which has String keyword before function name, means it return String value, and the empty pair of parentheses suggests that there is no parameter that is passed to the function.

Example 2: No Parameter & Return Type
Here voterAge() is a function which returns minimum voter age.

// Function With No Parameter & Return Type
void main() {
  int personAge = 17;

  if (personAge >= voterAge()) {
    print("You can vote.");
  } else {
    print("Sorry, you can't vote.");
  }
}

int voterAge() {
  return 18;
}
 Show Output
Function With Parameter And Return Type
In this function, you do pass the parameter and also expect return type. Here is an example of it:

Example 1: Parameter & Return Type
Here add(int a, int b) is a function that returns its sum in integer. We can display results in our main function.

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
 Show Output
In this program, int add(int a, int b) is the function with int as the return type, and the pair of parenthesis has two parameters, i.e., a and b.

Example 2: Parameter & Return Type
Here calculateInterest(double principal, double rate, double time) is a function that returns its simple interest in double. We can display results in our main function.

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
 Show Output
 Info
Note: void is used for no return type as it is a non value-returning function.

**Complete Example **
Here is the program, which includes all types of functions we studied earlier.

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
 Show Output


FUNCTION PARAMETER IN DART
Parameter In Dart
The parameter is the process of passing values to the function. The values passed to the function must match the number of parameters defined. A function can have any number of parameters.

// here a and b are parameters
void add(int a, int b) { 
} 
Positional Parameter In Dart
In positional parameters, you must supply the arguments in the same order as you defined on parameters when you wrote the function. If you call the function with the parameter in the wrong order, you will get the wrong result.


Example 1: Use Of Positional Parameter
In the example below, the function printInfo takes two parameters. You must pass the person’s name and gender in the same order. If you pass values in the wrong order, you will get the wrong result.

void printInfo(String name, String gender) {
  print("Hello $name your gender is $gender.");
}

void main() {
  // passing values in wrong order
  printInfo("Male", "John");

  // passing values in correct order
  printInfo("John", "Male");

}
 Show Output
Example 2: Providing Default Value On Positional Parameter

In the example below, function printInfo takes two positional parameters and one optional parameter. The title parameter is optional here. If the user doesn’t pass the title, it will automatically set the title value to sir/ma’am.

void printInfo(String name, String gender, [String title = "sir/ma'am"]) {
  print("Hello $title $name your gender is $gender.");
}

void main() {
  printInfo("John", "Male");
  printInfo("John", "Male", "Mr.");
  printInfo("Kavya", "Female", "Ms.");
}
 Show Output
Example 3: Providing Default Value On Positional Parameter
In the example below, function add takes two positional parameters and one optional parameter. The num3 parameter is optional here with default value 0.

void add(int num1, int num2, [int num3=0]){
   int sum;
  sum = num1 + num2 + num3;
   
   print("The sum is $sum");
}

void main(){
  add(10, 20);
  add(10, 20, 30);
}
 Show Output
Named Parameter In Dart
Dart allows you to use named parameters to clarify the parameter’s meaning in function calls. Curly braces {} are used to specify named parameters.

Example 1: Use Of Named Parameter
In the example below, function printInfo takes two named parameters. You can pass value in any order. You will learn about ? in null safety section.

void printInfo({String? name, String? gender}) {
  print("Hello $name your gender is $gender.");
}

void main() {
  // you can pass values in any order in named parameters.
  printInfo(gender: "Male", name: "John");
  printInfo(name: "Sita", gender: "Female");
  printInfo(name: "Reecha", gender: "Female");
  printInfo(name: "Reecha", gender: "Female");
  printInfo(name: "Harry", gender: "Male");
  printInfo(gender: "Male", name: "Santa");
}
 Show Output
Example 2: Use Of Required In Named Parameter
In the example below, function printInfo takes two named parameters. You can see a required keyword, which means you must pass the person’s name and gender. If you don’t pass it, it won’t work.

void printInfo({required String name, required String gender}) {
  print("Hello $name your gender is $gender.");
}

void main() {
  // you can pass values in any order in named parameters.
  printInfo(gender: "Male", name: "John");
  printInfo(gender: "Female", name: "Suju");
}
 Show Output
 Info
Note: You can pass the value in any order in the named parameter. ? is used to remove null safety, which we will discuss in the coming chapter.

Optional Parameter In Dart
Dart allows you to use optional parameters to make the parameter optional in function calls. Square braces [] are used to specify optional parameters.

Example: Use Of Optional Parameter
In the example below, function printInfo takes two positional parameters and one optional parameter. First, you must pass the person’s name and gender. The title parameter is optional here. Writing [String? title] makes title optional.

void printInfo(String name, String gender, [String? title]) {
  print("Hello $title $name your gender is $gender.");
}

void main() {
  printInfo("John", "Male");
  printInfo("John", "Male", "Mr.");
  printInfo("Kavya", "Female", "Ms.");
}
 Show Output


Anonymous Function In Dart
This tutorial will teach you the anonymous function and how to use it. You already saw function like main(), add(), etc. These are the named functions, which means they have a certain name.

But not every function needs a name. If you remove the return type and the function name, the function is called anonymous function.

Syntax
Here is the syntax of the anonymous function.

(parameterList){
// statements
}
Example 1: Anonymous Function In Dart

In this example, you will learn to use an anonymous function to print all list items. This function invokes each fruit without having a function name.

void main() {
  const fruits = ["Apple", "Mango", "Banana", "Orange"];

  fruits.forEach((fruit) {
    print(fruit);
  });
}
 Show Output
Example 2: Anonymous Function In Dart
In this example, you will learn to find the cube of a number using an anonymous function.

void main() {
// Anonymous function
  var cube = (int number) {
    return number * number * number;
  };

  print("The cube of 2 is ${cube(2)}");
  print("The cube of 3 is ${cube(3)}");
}
 Show Output

Arrow Function In Dart
Dart has a special syntax for the function body, which is only one line. The arrow function is represented by => symbol. It is a shorthand syntax for any function that has only one expression.

Syntax
The syntax for the dart arrow function.

returnType functionName(parameters...) => expression;
 Info
Note: The arrow function is used to make your code short.=> expr syntax is a shorthand for { return expr; }.

Example 1: Simple Interest Without Arrow Function

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
 Show Output
Example 2: Simple Interest With Arrow Function

This program finds simple interest using the arrow function.

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
 Show Output
Example 3: Simple Calculation Using Arrow Function
This program finds the sum, difference, multiplication, and division of two numbers using the arrow function.

int add(int n1, int n2) => n1 + n2;
int sub(int n1, int n2) => n1 - n2;
int mul(int n1, int n2) => n1 * n2;
double div(int n1, int n2) => n1 / n2;

void main() {
  int num1 = 100;
  int num2 = 30;

  print("The sum is ${add(num1, num2)}");
  print("The diff is ${sub(num1, num2)}");
  print("The mul is ${mul(num1, num2)}");
  print("The div is ${div(num1, num2)}");
}
 Show Output

