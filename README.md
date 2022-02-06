# iamrich

first mini project for koding and kahawa.This is a way of showcasing how flutter application are built. Fill up your kahawa mug and lets get started.

# Technologies 

1. Flutter --> This is the UI framework being used 
2. dart --> thsi is the programming language we are using 
3. Visual studio code / Android Studio --> Envronments that can be used to build flutter apps 

# Step 1: How to create an app in flutter 
Flutter apps are created by running the ``` flutter create <app name> ``` on terminal. By default required folders are created together with a default app created by the Flutter team. 

# Step 2: How to run flutter apps 
To run flutter apps, use the command ```flutter run <app name>``` or ```flutter run -d <platform> <app name>```, a platform specification can be ```chrome brwser```, ```linux environment``` or ```android``` and ``IOS`` environment.
# Step 3: Flutter Team default app 
When the flutter run command is used, a default app is generated which usually has a button that when clicked tracks the number of times a user clicked it. 
Explaining Code
````dart import ‘package:flutter/material.dart’;````
The very first line of code is quite self explanatory, it’s being used to import the library Material.dart. This library is used to design the UI which follows Google’s Material Design Guideline. If you want to use controls which are based on iOS controls, you will have to import cupertino.dart package.

````dart
void main() => runApp(new MyApp());
````
This is the main entry point or starting point of the app. When executed, the compiler will create an instance of MyApp class and pass it to the runApp function which will execute the application.

````dart
class MyApp extends StatelessWidget
````
This is the main root of the application. It is extended from StatelessWidget and used to initialize the Material App and to set the Theme, color and home screen of the application. Here, MyApp is just the name given to default root class, if you want, you can change the name of the class as per your requirements.

````dart 
class MyHomePage extends StatefulWidget
````
This class contains the code for Homepage/Screen of the application which is invoked in the MyApp class. This class is extended from StatefulWidget widget class because the elements of the HomePage will change on the actions performed by the user. The Last line of the code
````dart 
( _MyHomePageState createState() => new _MyHomePageState(); )
```` 
of this class is used to create the state of the screen.

````dart 
class _MyHomePageState extends State<myhomepage>
````
This is the class which is responsible for changing the state of the Home screen on the basis of user input. This class is Extended from State class by passing MyHomePage as type.

This was a brief explanation of the default Flutter app code, we will get more used to this as we work further on Flutter development. 

# Step 4: Building our IamRichApp 
Delete the default code generated and add the code below.
````dart
void main() {
  runApp(const MaterialApp(home: Text("I drink coffee ")));
}
````
Like other  programming languages like java,c++ and C,  ```dart``` excecution starts from the main function.A function ```runApp()``` is nested with the main fuction. The ```runApp()``` function takes the given Widget and makes it the root of the widget tree. In this example, the widget tree consists of two widgets, the Center widget and its child, the Text widget. The framework forces the root widget to cover the screen, which means the text “Hello, world” ends up centered on screen. The text direction needs to be specified in this instance; when the MaterialApp widget is used, this is taken care of for you, as demonstrated later.
## introduction to widgets

Flutter comes with a suite of powerful basic widgets, of which the following are commonly used:
All the widgets are usually nested inside the MaterialApp widget so that  our app can use the material design developped by google 
#### What is Material design 
Material is a design system created by Google to help teams build high-quality digital experiences for ```Android```, ```iOS```, ```Flutter```, and the ```web```.Material Design is inspired by the physical world and its textures, including how they reflect light and cast shadows. Material surfaces reimagine the mediums of paper and ink.Material Components are interactive building blocks for creating a user interface, and include a built-in states system to communicate focus, selection, activation, error, hover, press, drag, and disabled states. Component libraries are available for ```Android```, ```iOS```, ```Flutter```, and the ```web```.



```Text```
The Text widget lets you create a run of styled text within your application.If this widgets are nested together they form a widget tree as shown below.
For example we can center the ``text`` widget by nesting it inside the ```Center``` widget 
***picture 






