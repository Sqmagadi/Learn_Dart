ASYNCHRONOUS PROGRAMMING
Asynchronous Programming In Dart
Asynchronous Programming is a way of writing code that allows a program to do multiple tasks at the same time. Time consuming operations like fetching data from the internet, writing to a database, reading from a file, and downloading a file can be performed without blocking the main thread of execution.

Synchronous Programming
In Synchronous programming, the program is executed line by line, one at a time. Synchronous operation means a task that needs to be solved before proceeding to the next one.

Example Of Synchronous Programming
void main() {
  print("First Operation"); 
  print("Second Big Operation"); 
  print("Third Operation"); 
  print("Last Operation"); 
}
 Show Output
Here in this example, you can see that it will print line by line. Let’s suppose Second Big Operation takes 3 seconds to load then Third Operation and Last Operation need to wait for 3 seconds. To solve this issue asynchronous programming is here.


Asynchronous Programming
In Asynchronous programming, program execution continues to the next line without waiting to complete other work. It simply means, Don’t wait. It represents the task that doesn’t need to solve before proceeding to the next one.

 Info
Note: Asynchronous Programming improves the responsiveness of the program.

Example Of Asynchronous Programming
void main() {
  print("First Operation");   
  Future.delayed(Duration(seconds:3),()=>print('Second Big Operation'));
  print("Third Operation"); 
  print("Last Operation"); 
}
 Show Output
Here in this example, you can see that it will print Second Big Operation at last. It is taking 3 seconds to load and Third Operation and Last Operation don’t need to wait for 3 seconds. This is the problem solved by Asynchronous Programming. A Future represents a value that is not yet available, you will learn about Future in the next section.


Why We Need Asynchronous
To Fetch Data From Internet,
To Write Something to Database,
To execute a long-time consuming task,
To Read Data From File, and
To Download File etc.
Such asynchronous operations usually take a long time to complete, so it usually provide results in the form of a Future. If the result has multiple parts, then it provides as a Stream. You will learn about Future and Stream in the next section.

 Info
Note: To Perform asynchronous operations in dart you can use the Future class and the async and await keywords. We will learn Future, Async, and Await later in this guide.

Important Terms
Synchronous operation blocks other operations from running until it completes.
Synchronous function only perform a synchronous operation.
Asynchronous operation allows other operations to run before it completes.
Asynchronous function performs at least one asynchronous operation and can also perform synchronous operations.


Future In Dart
In dart, the Future represents a value or error that is not yet available. It is used to represent a potential value, or error, that will be available at some time in the future.

How To Create Future In Dart
You can create a future in dart by using Future class. Here the function will return Future<String> after 5 seconds.

// function that returns a future
Future<String> getUserName() async {
  return Future.delayed(Duration(seconds: 2), () => 'Mark');
}
You can also create a future by using Future.value() method. Here the function will return Future<String> immediately.

// function that returns a future
Future<String> getUserName() {
  return Future.value('Mark');
}
How To Use Future In Dart

You can use future in dart by using then() method. Here the function will return Future<String> after 5 seconds.

// function that returns a future
Future<String> getUserName() async {
  return Future.delayed(Duration(seconds: 2), () => 'Mark');
}

// main function
void main() {
  print("Start");
  getUserName().then((value) => print(value));
  print("End");
}
 Show Output
More About Future
Future represents the result of an asynchronous operation and can have 2 states.

State Of Future
Uncompleted
Completed
Uncompleted

When you call an asynchronous function, it returns to an uncompleted future. It means the future is waiting for the function asynchronous operation to finish or to throw an error.

Completed
It can be completed with value or completed with error. Future<int> produces an int value, and Future<String> produces a String value. If the future doesn’t produce any value, then the type of future is Future<void>.

 Info
Note: If the asynchronous operation performed by the function fails due to any reason, the future completes with an error.

Example 2: Future In Dart
In this example below, we are creating a function middleFunction() that returns a future. The function will return Future<String> after 5 seconds.

void main() {
  print("Start");
  getData();
  print("End");
}

void getData() async{
  String data = await middleFunction();
  print(data);
}

Future<String> middleFunction(){
  return Future.delayed(Duration(seconds:5), ()=> "Hello");
}
 Show Output
 Info
Note: In the above example, First, it prints Start, secondly it prints End, and after 5 seconds Hello will be printed.



ASYNC AND AWAIT IN DART
Async And Await In Dart
Async/await is a feature in Dart that allows us to write asynchronous code that looks and behaves like synchronous code, making it easier to read.

When a function is marked async, it signifies that it will carry out some work that could take some time and will return a Future object that wraps the result of that work.

The await keyword, on the other hand, allows you to delay the execution of an async function until the awaited Future has finished. This enables us to create code that appears to be synchronous but is actually asynchronous.

The async and await keywords both provide a declarative way to define an asynchronous function and use their results. You can use the async keyword before a function body to make it asynchronous. You can use the await keyword to get the completed result of an asynchronous expression.

Important Concept
To define an Asynchronous function, add async before the function body.
The await keyword work only in the async function.
Example 1: Synchronous Function
void main() {
  print("Start");
  getData();
  print("End");
}

void getData() {
  String data = middleFunction();
  print(data);
}

Future<String> middleFunction(){
  return Future.delayed(Duration(seconds:5), ()=> "Hello");
}
 Show Output
Example 2: Asynchronous function
void main() {
  print("Start");
  getData();
  print("End");
}

void getData() async{
  String data = await middleFunction();
  print(data);
}

Future<String> middleFunction(){
  return Future.delayed(Duration(seconds:5), ()=> "Hello");
}
 Show OutputIn the above example, async handles the states of the program where any part of the program can be executed.async always comes with await because await holds the part of the program until the rest of the program executed.
Handling Errors

You can handle errors in the dart async function by using try-catch. You can write try-catch code the same way you write synchronous code.

Example 3: Handling Errors
main() {
  print("Start");
  getData();
  print("End");
}


void getData() async{
    try{
        String data = await middleFunction();
        print(data);
    }catch(err){
        print("Some error $err");
    }
 
}

Future<String> middleFunction(){
  return Future.delayed(Duration(seconds:5), ()=> "Hello");
}
 Show OutputIn the above example, try-catch handles the exception that could come after the program is executed.
 Info
Note: We cannot perform an asynchronous operation from a synchronous function.

Important Terms
async The async keyword can be used before a function’s body to indicate that a function is asynchronous.
async function Functions marked with the async keyword are known as async functions.
await The completed output of an asynchronous expression can be retrieved with the await keyword. Only async functions can use the await keyword.


STREAMS IN DART
Stream
A stream is a sequence of asynchronous events representing multiple values that will arrive in the future. Stream class deals with sequences of events instead of single events. Stream has one or more listeners, and all listeners will receive the same value.

For example, A stream is like a pipe that emits events, you put a value on the one end, and if there’s a listener on the other end that listener will receive that value. These events can be values of any type, errors or a “done” event to signal the end of the stream.

Single Value	Zero or more values
Sync	int	Iterator
Async	Future<int>	Stream<int>
How To Create Stream In Dart

You can create a stream in dart by using Stream class. Here the function will return Stream<String> after 5 seconds.

// function that returns a stream
Stream<String> getUserName() async* {
  await Future.delayed(Duration(seconds: 1));
  yield 'Mark';
  await Future.delayed(Duration(seconds: 1));
  yield 'John';
  await Future.delayed(Duration(seconds: 1));
  yield 'Smith';
}
 Info
Note: Here yield returns the value from the stream. To use yield you have to use async*.

You can also create a stream by using Stream.fromIterable() method. Here the function will return Stream<String> immediately.

// function that returns a stream
Stream<String> getUserName() {
  return Stream.fromIterable(['Mark', 'John', 'Smith']);
}
How To Use Stream In Dart

You can use stream in dart by using await for loop.

// function that returns a stream
Stream<String> getUserName() async* {
  await Future.delayed(Duration(seconds: 1));
  yield 'Mark';
  await Future.delayed(Duration(seconds: 1));
  yield 'John';
  await Future.delayed(Duration(seconds: 1));
  yield 'Smith';
}

// main function
void main() async {
  // you can use await for loop to get the value from stream
  await for (String name in getUserName()) {
    print(name);
  }
}
 Show Output
Future vs Stream
Future	Stream
Future represents the value or error that is supposed to be available in the Future.	Stream is a way by which we receive a sequence of events.
A Future can provide only a single result over time.	Stream can provide zero or more values.
You can use FutureBuilder to view and interact with data.	You can use StreamBuilder to view and interact with data.
It can’t listen to a variable change.	But Stream can listen to a variable change.
Syntax: Future <data_type> class_name	Syntax: Stream <data_type> class_name
Types Of Stream
There are two types of streams:

Single Subscription streams
Broadcast streams
Single Subscription Stream
By default, Streams are set up for a single subscription. They hold onto the values until someone subscribes and can only be listened to once. You will get an exception if you try to listen more than once. Any event’s value should not be missed and must be in the correct order. Inside the stream controller, there is only one stream, and only one subscriber can use that stream.

Broadcast Stream
This is the stream that is set up for multiple subscriptions. They hold onto the values until subscribers can only listen many times. You can use the broadcast stream if you want more objects to listen to the stream. It can be used for mouse events in a browser. Inside the stream controller, many streams can be used by many subscribers. E.g., You can start watching videos on such a stream at any time, and more than one subscriber can watch the video simultaneously. Similarly, you can watch again after canceling a previous subscription.

Syntax
StreamController<data_type> controller = StreamController<data_type>.broadcast();
How Streams Are Created
You can create a stream in many ways. Let’s create a StreamController first.

StreamController<data_type> controller = StreamController<data_type>();
Now we can access this controller through the stream property.

Stream stream = controller.stream;
How To Subscribe A Stream
After getting access from the stream you subscribe to the stream by calling a listen() method.

 stream.listen((value) {
  print("Value from controller: $value");
});
How To Add Value To The Stream
We can add the stream by calling the add() method. Let’s add some value to the stream.

controller.add(3);
When we call the above function, we’ll get the output as:

Value from controller: 3

How To Manage The Stream
To manage the stream, listen() method is used.

StreamSubscription<int> streamSubscription = stream.listen((value){
  print("Value from controller: $value");
});
How To Cancel A Stream
You can cancel a stream by using the cancel() method.

streamSubscription.cancel();
Types Of Classes In Stream
Four major classes in Dart’s async libraries are used to manage streams.

Stream: It represents an asynchronous stream of data. For E.g:

 final controller = StreamController<String>();

final subscription = controller.stream.listen((String data) {
  print(data);
});
controller.sink.add("Data!");
EventSink: It is like a stream that flows in the opposite direction.

StreamController: It simplifies stream management, automatically creating a stream and sink and also providing methods for controlling a stream’s behavior.

StreamSubscription: It saves the references of the subscription and allows them to pause, resume or cancel the flow of data they receive.

Method Used In Stream
There are four methods used in the stream: *listen(): It returns a StreamSubscription object representing the active stream-producing events. The stream subscription allows you to pause, resume the subscription after a pause, and cancel the subscription completely.

Syntax: listen
final subscription = myStream.listen()
onError: Stream can provide errors just like a future can; by adding an onError method, you can catch and process an mistakes.
Syntax: onError
onError: (err){

}
cancelOnError: This property or method is true by default but can be set to false to keep the subscription going even after an error.
Syntax: cancelOnError
cancelOnError : false
onDone: This method can execute some code when the stream is finished sending data, such as when a file has been completely read.
Syntax: onDone
onDone: (){
  
}
Keywords Used In Stream
async*: It is mainly used in the stream that works like the async in the future.

yield: It is used to emit values from a generator, either async or sync. yield returns values from an Iterable or a Stream.

yield*: yield* is used to call its Iterable or Stream function recursively.

Example Of async
Future<int> doSomeLongTask() async {
  await Future.delayed(const Duration(seconds: 2));
  return 21;
}main() async {
  int result = await doSomeLongTask();
  print(result); // prints '42' after waiting 2 second
}
 Show Output
Example Of async In Dart*
Stream<int> countForOneMinute() async* {
  for (int i = 1; i <= 5; i++) {
    await Future.delayed(const Duration(seconds: 1));
    yield i;
  }
} main() async {
  await for (int i in countForOneMinute()) {
    print(i); // prints 1 to 5, one integer per second
  }
}
 Show Output
Example Of yield In Dart*
Stream<int> str(int n) async* {
 if (n > 0) {  
   await Future.delayed(Duration(seconds: 2));
   yield n;
   yield* str(n - 2);
 }
}

void main() {
 str(10).forEach(print);
}
 Show OutputIn the above example, you have printed only an even number from 10 to 2 using stream. It will print the number after 2 sec.
Some More Example OF Stream
Example 1
import 'dart:async';

void main() {
  var controller = StreamController();
  controller.stream.listen((event) {
    print(event);
  });
  controller.add('Hello');
  controller.add(42);
  controller.addError('Error!');
  controller.close();
}
 Show Output
In this example, a String, integer and an error are added to the StreamController and then printed using the listen property.

Example 2
Stream<int> numberOfStream(int number) async* {
  for (int i = 0; i <= number; i++) {
    yield i;
  }
}

void main(List<String> arguments) {
  // Calling the Stream 
  var stream = numberOfStream(6);
  // Listening to Stream yielding each number
  stream.listen((s) => print(s));
}
 Show OutputIn the above example, you must print the number from 0 to 6 using stream.
Example 3
Stream<int> str(int n) async* {
 for (var i = 1; i <= n; i++) {
   await Future.delayed(Duration(seconds: 1));
   yield i;
 }
}

void main() {
 str(10).forEach(print);
}
 Show Output
In the above example, you must print the number from 1 to 5 using stream. It will print the number after 1 sec.

async vs async In Dart*
async	async*
It gives a Future.	It gives a Stream.
async keyword does some work that might take a long time.	async* returns a bunch of future values on at a time.
It gives the result wrapped in future.	It gives the result wrapped in the stream.
yield vs yield In Dart*
yield	yield*
It is a keyword that returns single value to the sequence, but doesn’t stop the generator function.	It is used for returning recursive generator.
To sum up, Streams are used in Dart to handle asynchronous data flows. They allow us to process data as it becomes available, rather than waiting for it to be fully loaded before processing.

Streams are commonly used in scenarios where data is being continuously updated or where we want to handle events as they occur. For example, we can use streams to monitor user interactions in real-time, or to receive data from a server as it becomes available.

In Dart, we can use the Stream and StreamController classes to create and manage streams. The StreamController class is used to create a stream and add data to it, while the Stream class is used to listen to the stream and process incoming data.

Ultimately, streams are a strong feature in Dart that let us handle asynchronous data flows in a flexible and effective way.


QUESTION FOR PRACTICE 8
Dart Asynchronous Programming Practice Questions
Explain what is asynchronous programming in dart?

What is Future in dart?

Write a program to print current time after 2 seconds using Future.delayed().

Write a program in dart that reads csv file and print it’s content.

Write a program in dart that uses Future class to perform multiple asynchronous operations, wait for all of them to complete, and then print the results.

Write a Dart program to calculate the sum of two numbers using async/await.

Write a Dart program that takes in two integers as input, waits for 3 seconds, and then prints the sum of the two numbers.

Write a Dart program that takes a list of strings as input, sorts the list asynchronously, and then prints the sorted list.

Write a Dart program that takes a list of integers as input, multiplies each integer by 2 asynchronously, and then prints the modified list.

Write a Dart program that takes a string as input, reverses the string asynchronously, and then prints the reversed string.