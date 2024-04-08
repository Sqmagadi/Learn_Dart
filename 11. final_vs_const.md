Final Vs Const In Dart
If you do not want to change the value of a variable, then you can use either final or const in dart.

Example
void main() {
  final finalName = "Final John Doe";
  const constName = "Const John Doe";

  finalName = "Raj"; // Not Possible
  constName = "Anu"; // Not Possible

  print("Final name is " + finalName);
  print("Const name is " + constName);
}
 Show Output
Const In Dart

If you need to calculate value at compile-time, it is a good idea to choose const over final. A const variable is a compile-time constant. They must be created from data that can be calculated at compile time. 100+1 is valid const expression but const date = DateTime.now(); is not.

What Is Compile Time
When you run code in the dart, it will be compiled into the format that the machine can understand. This time is called compile time. Const value should be known at compile time.

What Is Run Time
Runtime is the time when your compiled code is started running. It generally occurs after the compile time.

 Info
Note: If you use const inside the class, declare it as static const.

const total = 50+50; // Possible
const date = DateTime.now(); // Not Possible
Advantage Of Constant
Improve Performance
Final In Dart

If the value is calculated at runtime, you can choose final for it. For. e.g if you want to calculate date on run time, you can use final date = DateTime.now(); but not const date = DateTime.now();.

 Info
Note: Anything that is unknown at compile time should be final over const.

final date = DateTime.now(); // Possible
const date = DateTime.now(); // Not Possible
When To Use Const
If you know the value at compile-time, choose const for e.g. const a = 100;.
When To Use Final
If you don’t know the value at compile-time, choose final.
If you want a network request that can’t be changed, choose final.
If you want to get some values from the database, choose final.
If you want to read a local file, choose final.
 Info
Note: Final variables will have a value known at runtime. Const variables have a value known at compile time. Instance variable can be final but not const.

