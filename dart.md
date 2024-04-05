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