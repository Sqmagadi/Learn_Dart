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