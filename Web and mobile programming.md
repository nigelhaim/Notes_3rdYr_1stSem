
#### New room 1802

2023-08-19

Self studied prof on mobile programming 

**More on android programming but also teaches swift back at Roque Ruano. Not a fan of macs so it transitioned to React.** 
- "I will do my best to teach you flutter and Dart"
	- Discussed with sir Decamora 

Objectives 
- Install flutter to windows 

Android studio 
	- Downside is not efficient 


### Orientation

**Rationale** - This course introduces the students in creating a native mobile application known as flutter as the front-end and Dart as the backend
**Focus** - Give emphasis on the development of a native mobile application that will run in any mobile operating system 
**Outcomes** - Exptected to be fluent in Dart and build flutter apps to become a full-pledged flutter developer 

#### Course intended learning outcome 
- **CILO1** - Flutter fundamentals (Online)
- **CILO2** - Dart Fundamentals
- **CILO3** - Objective oriented programming 
- **CILO4** - Control structures 
- **CILO5** - Data Structures
- **CILO6** - Software Design
				- MVC
- **CILO7** - Mobile Concepts on networking
				- JSON Formats
				- API Calls
- **CILO8** - Concepts on Mobile Data Storage 
				- Cloud Based (Firebase)

#### Policies 
- Check announcements
- Attendance anytime
- Kapag sa lab 
	- Yung gamit sa shelf
	- Tubig sa baba ng desk
- Uniform and ID 
- Pag absent 
	- Excuse letter with photo ID of parent/guardian
- UST code of honor

#### Assessment 
- Formatives are not included in the competition
- Recitation
- Short Quizzes
	- Every other meeting sometimes not within 24 hrs deadline 
- Major Exams no final exam but final project 

#### Computation
Semgrade 50% PG + 50% FG
30 - Machine problems
30 quizzes
40 major exam
Pass 60

### Installing flutter
1. Go to docs.flutter.dev
2. Get started then install (top left)
3. Click windows
4. Scroll down and download the zip file  855MB 
5. Install GIt (64 bit)????????
6. Extract the zip file and place the contained flutter in the desired installation location for the flutter SDK 
7. From the Start search bar, enter 'env' and select Edit environemnt varibalbes for your account 
8. Under User Variables check if there is an entry called Path:
	1. If the entry exists, append the full path to flutter\bin using ; as a separator 
	2. If the entry doesn't exist, create a new user variable named Path with the full path to flutter\bin as its avlue 
9. Run the terminal then type flutter and hit enter it will show a prompt that means the path is working 
10. type where.exd flutter dart then it will show another prompt (.bat)
11. type flutter doctor 
12. It will show checks and x where flutter is now running
13. Download Android studio (for the virtual android) and install 
14. Install flutter extension in viusal studio code it will also install dart
**Notes:**
- It was instructed that in step 9 to type where flutter dart but it doenst work until lex discovered what I did in step 9

2023-09-08

## Flutter
Flutter - Is a SDK that is used to build high performance, modern and beautiful apps with ease 
- A free and open-source toolkit developed by Google
- Used to develop applications for Android, iOS, Windows, Mac, Linux, Google Fuchsia and the web 
- Flutter is Google's UI toolkit for building beautiful, natively compiled applications for mobile, web, and desktop from a single codebase 
- Flutter uses Dart language

#### History 
- In 2015 Google unveil Flutter
- 2019 an alpha version of it (0.0.6) was released to the public for the first time 
- In December 2018 Flutter 1.0 was released (promote - make app creation easier) - stable version
- At Google I/O 2019, Flutter support for desktop and web platforms 

#### Why use Flutter? 
- Natively compiled applications for mobile, web, and desktop from a single codebase 
- Noe bridge needed 
- Compiles to Native Code
- Not markup language (only Dart)
- Close related up performance 

**Advantages**
- High performance 
- Immediate Updates
- Custom widgets for quick UI Coding 
- Mild learning curve

**Disadvantages**
- Large File sizes
- Lack of third-party libraries
- Issues with IOS 

**Works for both iOS and Android**

**Other Hybrid/Cross Development Frameworks**
- IONIC
- React Native
- Xamarin 
- PhoneGap
- NativeScript


| |React Native |Ionic|Flutter|
| --- | --- | --- | --- |
|Language|JavaScript & React | HTML, CSS, JavaScript (you can use with React, Vue, or Angular) | Dart Language | 
| Nature of apps | Cross-platform | Hybrid cross-platform | Cross-platform | 
| Founded Year (Initial Release) | March 2015 | 2013 | May 2017 | 
| Developed by | Facebook & Community | Drifty Co. | Google & Community | 
| Community support | Strong | Strong | Lack of community support as it's new | 
| Open source | Yes | Yes, Paid  also | Yes |
| Front-end support | Native components & Declarative UI | HTML, CSS, and a wide range of UI designs | Great support for attractive UIs with built in widgets | 
| Code reusability | Learn once, write everywhere | Once codebase, any platform | Reusable widgets | 
| Used By | Facebook, Instagram, Tesla, Uber, Walmart, Airbnb | MarketWatch, NHS, Sowrkit, Instant Pot, Untapped | Alibaba, AppTree, Google Ads, Reflectly, Tencent |
| Performance | Faster and native like experience | Interactive and faster apps | High-performing and graphically enhance app |
### Flutter Architecture
#### You Can customize everything in green

![[Pasted image 20230908193229.png]]

![[Pasted image 20230908193349.png]]

| Stateful Widget | Stateless Widget | 
| --- | --- | 
| can build in many different BuildContexts | creates a new State object for each BuildContext | 
| when Widget changes its value, that's stateful. e.g. Checkbox, Radio button, Textfield| No change in widget value, that's stateless eg. Text, Icon, Icon buttom, Raised button|
| Override the CreateState and return State. | Override the build() and return Widget |
|Use when user want to change UI dynamically. | Use when UI remains constant during runtime |
|When Widget's state changes, the State object calls setState(), telling framework to redraw widget | |


#### Everything is a Widget 

![[Pasted image 20230908193900.png]]

### IDE SUPPORT
- Android Studio
- Visual Studio Code
- DartPad 
- IntelliJ

### What kinds of apps Flutter can build?
- Flutter is optimized mobile apps that want to run on both Android and IOS.
- You can build full-featured apps with Flutter, including, camera, geolocation, network, storage, 3rd-party SDKs, and more .

### Hot Reload
- Flutter is Engineered for high development velocity apps in which **Stateful Hot Reload** allows user to change their code and see it come to life in less than a **second** without losing the state of that app,
- Injecting **updated source code** files into the running **Dart VM**

###  Flutter is unique 
- Flutter uses neither **WebView** nor the **OEM widgets** that shipped with the device. Instead, Flutter uses its own high-performance rendering engine to draw  widgets.
- In addition, Flutter is different because it only has a thin layer of C/C++ code. Flutter implements most of its system in Dart that developers can easily approach read, change, replace, or remove.


## Dart 
- General-purpose programming language originally developed by **Google** and later approved as a standard by **Ecma** (ECMA-408).
- Used to build **web, server** and **mobile applications** and for **Internet of Things (IoT)** devices.
- Dart was **unveiled** at the **GOTO conference**, **October 10-12, 2011**

2023 - 15 - 09

## Widgets 

- The central purpose is to build the app out of widgets. It describes how your app view should look like with their current configuration and state. 
- When you made any alteration in the code, the widget rebuilds its description by calculating the difference of previous and current widget to determine the minimal changes for rendering in UI of the app 
- These can be nested with each other to build the app. It means taht the root of the app itself a widget, and all the way down is a widget also.
- For example, a widget can display something, can define design, can handle interaction, etc. 
### Widget Tree
![[WidgetTree.png]]
### Widget Creation 

```
	Class ImageWidget extends StatelessWidget{
		//Class stuff
	}
```

### Stateful and Stateless
- A widget is either stateful or stateless. If a widget can change-when a user interacts with it 
- A stateless widget never changes. Icon, IconButton, and Text are examples of stateless widgets. Stateless widgets subclass StatelessWidget
- A stateful widget is dynamic: for examples, it can change its appearance in response to events triggered by user interactions or when it receives data. 
- Checkbox, Radio, Slider, InkWell, form and TextField are examples of stateful widget

### Widget-Types
- We can split the Flutter widget into two categories: 
	- Visible (output and input)
	- Invisible (Layout and Control)

### Visible Widget
- The visible widgets are related to the user input and output data. Some of the important  types of this widgets are: 
	- **Text**
		- This holds some text to display on the screen 
		- Using textAlign property, and style property allow the customization of Text that includes font, font weight, font style, letter spacing, color, and many more. 

```
	new Text(
		'Hello, Everyone!',
		texdtAlgin: TextAlign.center,
		style: new TextStyle(fontWeight: FontWeight.bold),
	)
```

```
	//FlatButton Example
	new RaisedButton(
		child:Text("Click here"),
		elevation: 5.0,
		onPressed(){
			//Do something here 
		},
	),
```

### Image
- This widget holds the image which can fetch it from multiple sources like form the asset folder or directly from the URL. It provides many constructors for loading image, which are the following:
	- **Image**: It is a generic image loader, which is used by ImageProvider 
	- **asset**: It load image from your project asset folder
	- **file**: It loads images from the system folder 
	- **memory**: It loads the image from the memory
	- **network**: It loads images from the network 

### Icon 
- This widget acts as a container for storing the Icon in the Flutter 
```
	new Icon(
		Icons.add,
		size:34.0,
	)
```

### Invisible Widget
- The invisible widgets are related to the layout and control of widgets. It provides controlling how the widgets actually behave and how they will look onto the screen. Some of the important types of these widgets are: 
	- **Column**
		- It is a type of widget that arranges all its children's widgets in a vertical alignment.
		- It provides spacing between the widgets by using the mainAxisAlignment and crossAxisAlignmnet properties 
		- In these properties, the main axis is the vertical axis, and the cross axis is the horizontal axis 

- The below code snippets construct two widget elements vertically
```
	new Column(
		mainAxisAlignment: MainAxisAlignment.center, 
		children:<Widget>[
			new Text("VegElement",
			),
			new Text("Non-vegElement"),
		],
	),
```

- The row widget is similar to the column widget, but it constructs a widget horizontally rather than vertically 
- Here, the main axis is the horizontal axis, and the cross axis is the vertical axis 
```
	new Row(
		mainAxisAlignmen: MainAxisAlignment.spaceEvenly,
		children:<Widget>[
			new Text("VegElement",
			),
			
			new Text("Non-vegElement"),
		],
	),
```
- This widget wraps other widgets to give them padding in specified directions. You can also provide padding in all directions

```
	Padding(
		padding:const EdgeInsets.all(6.0),
		child:new Text(
			"Element 1",
		)
	)
```

- Scaffold
	- this widget provides a framework that allows you to add common material design elements like AppBar, Floating Action Buttons, Drawers, etc 
- Stack
	- It is an essential widget, which is mainly used for overlapping a widget, such as a button on a background gradient. 

- A StatefulWidget has state information
- Two Classes: State object and widget 
- It is dynamic because it can change the inner data during the widget lifetime. 
- This widget does not have a build() method 
- It has createState() method, which returns a class that extends the Flutters State class
- Examples: Checkbox, Radio, Slider, InkWell, Form and TextField
### Flutter Engine
- It is portable runtime for high-quality mobile apps and primarily based on the c++ language
- It implements Flutter core libraries taht include animation, and grpahics, fiole and network I/O, plugin architecture, accessibility support, and a dart runtime for developing, compiling and running Flutter applications
- IT takes Googel's open-source graphics library, Skia to render low-level graphics


### How to run a flutter app on windows and android

1. Enable Developer mode (phone)
2. Enable USB Debugging (phone)
3. Connect Your Phone with USB
4. Trust Your Computer if Prompted (Phone)
5. Run App From Android Studio 
**Android Studio**
1. You should see your phone on the top right (HTC One Physical Device)
2. Click play on the main.dart 
3. Done 


# Starter codes 

https://drive.google.com/drive/u/2/folders/163pvMpKtnrGZz5K1w2zAdmzcccjybW_b




2023-10-4

## Prelim Exam
- 75 items good for 90 mins
- Not allowed to take the exam on their own devices

**Flexibility options allows the app to resize based on the screen device**

IntentionAtactions Gestures Functions Variable declaration Datatypes

## Dicee app

Clone a repository 

https://github.com/londonappbrewery/dicee-flutter.git

#### The user interface 
![[Pasted image 20231004081354.png]]


>[!note]- The scaffold is already made 
>![[Pasted image 20231004081529.png]]

- The dice image does not fit the screen that causes the overflow 


## Expanded child 
- A child of a row or column 
- Expands to fill the available space in the main axis 
> [!Note]- Insert the image
> ![[Pasted image 20231004081901.png]]

>[!Note]- Changing it to column
>![[Pasted image 20231004081919.png]]


>[!Note]- Duplicating the images 
>![[Pasted image 20231004082003.png]]

---
### Side note 
>[!Note]- If you want an image takes up the space twice than on the right
>![[Pasted image 20231004082054.png]]

--- 

# As programmers we may not have a lot of friends but documentation is our friend 


>[!Note]- Importing images in a shorter way 
>Less nesting 
>Less potential error 
>![[Pasted image 20231004082418.png]]

>[!Note]- Move row to the center of the screen 
>![[Pasted image 20231004082826.png]]

Move row to the center of the screen a much easier way 
>[!Note]- The new user interface tree
>![[Pasted image 20231004082908.png]]

>[!Note]- Click the line or the row and click the button 
>![[Pasted image 20231004082947.png]]

>[!Note]- Automatically adds the center widget 
>![[Pasted image 20231004083014.png]]

---

>[!Note]- Further exploration 
![[Pasted image 20231004083114.png]]

>[!Note]- You can also click the lightbulb at the left of the code for further actions(Alt+Enter)
>![[Pasted image 20231004083311.png]]

---

>[!Notes]- Change the row to Center 
>![[Pasted image 20231004083341.png]]
>![[Pasted image 20231004083421.png]]



>[!Notes]- Putting a space between the dices 
>![[Pasted image 20231004083543.png]]


### Documentation 

User Interface -> Widget Catalog 


>[!Notes]- Changing the user interface to 
>![[Pasted image 20231004083654.png]]

>[!Notes]- Adding the button and the image as its child 
>![[Pasted image 20231004083744.png]]


Noticing the button is smaller 

>[!Note]- Remove the padding of the button 
>![[Pasted image 20231004083917.png]]


>[!Note]- Notice the changes based on the wireframe 
![[Pasted image 20231004084010.png]]

>[!Note]- Apply changes on the right side 
![[Pasted image 20231004084120.png]]



Make the button do something 

When you see yellow lines it means there is a warning 
When you see red lines it is an error/fail 

>[!Note]- using onPressed 
![[Pasted image 20231004084312.png]]

> [!note]- Test onPressed using print 
>![[Pasted image 20231004084548.png]]


> [!note]- applying it to the right dice 
>![[Pasted image 20231004084730.png]]

--- 
Functions 
- Gives the program some functionality 
- Package bits of code together as a block 
- So you wont need to make the code type it again and again 

### Creating the function 
```
	void getMilk() { //doSomething }
```

### Calling the function 
```
	getMilk()
```
### Anonymous function 
```
	(){ //doSomething }
```


> [!note]- onPressed requires an anonymous function 
> ```
> onPressed: () { //doSomething }
> ```
```
```


---

Applying the concept of functions to update the image which button was pressed 


> [!note]- Create a variable that refers the number of the die and change the variable on the string of the Image.asset
> ![[Pasted image 20231004085821.png]]

**String interpolation** - Adding variables on a string 

--- 
### Variables
- A data container 
---
Updating the variable creates a warning of a StateLessWidget 

>[!note]- Initiating the variable outside the build method
>![[Pasted image 20231004092142.png]]

We need to use the StateFullWidget 

shortcut on android studio 
```
stful [Enter]
```

> [!note]- Creating the StatefulWidget
> ![[Pasted image 20231004092552.png]]

>[!note]- copy everytthing
>![[Pasted image 20231004092641.png]]

> [!note]- Updating the state on press with setState()
> **Watch the change**
> ![[Pasted image 20231004092907.png]]
> ![[Pasted image 20231004092918.png]]

### setState()
- marks the state as dirty 
- calls the build then updates the dirty state 
- In contrast it **redraws everything**
- ![[Pasted image 20231004093213.png]]
- ![[Pasted image 20231004093242.png]]

### Continuation

> [!note]- using math random 
> **import 'dart.math';**
> ![[Pasted image 20231004093751.png]]
> ![[Pasted image 20231004094229.png]]

>[!note]- applying it to the right die 
>![[Pasted image 20231004094523.png]]

>[!note]- both dice will change if one die is clicked 
>![[Pasted image 20231004094723.png]]

> [!note]- applying the concept of functions
> ![[Pasted image 20231004095026.png]]


# Machine languages and requirements 

- 50% prelim grade + 50% Final Period grade 

**Final period grade**
- 30% MP/Act 
- 30% Quizzes
- 40% Final project

## Machine Problem 
- Xylophone app but different instrument 
- 1 Full octave 

## Quizzes 
- Dicee app 



## Flutter packages 

### Xylophone app 

Clone a git repository 

Open the project (Main.dart)

>[!Image]- Upon Opening
>![[Pasted image 20231018081440.png]]

>[!Note]- Pubspec.yaml
>![[Pasted image 20231018081504.png]]

When you add image and sound files it is done the same way
- assets/msc.mov

>[!Note]- What are flutter packages 
>open source libraries of code that other people created which anyone can incorporate in their projects 

**Search for generattes words** 

>[!Note]- Generates words 
>Look for the score on the right (Blue circle with a number)
>![[Pasted image 20231018081737.png]]

>[!Note]- english_words
>![[Pasted image 20231018081938.png]]

### Link
https://pub.dev/packages/english_words

>[!Note]- add english_words on the pubspec.yaml 
>![[Pasted image 20231018082106.png]]
- This tells flutter to grab the package with any of its version 

>[!Note]- To specify the  version of the package 
>![[Pasted image 20231018082212.png]]

**Install the package**

>[!Note]- click packages get
> You can also run it on the terminal
>![[Pasted image 20231018082404.png]]
>![[Pasted image 20231018082419.png]]

**Import the package**

>[!Note]- Get an English adjective and show it on screen
>![[Pasted image 20231018082609.png]]
>Using last the word on the list 
>![[Pasted image 20231018082638.png]]

- We can only use adjectives, nouns, and all 
>[!Note]- Find the list of words on the package 
>![[Pasted image 20231018082728.png]]


**Think of packages as Lego**
- Everything was already premade just be creative how to implement it 

**Search for play audio file**

>[!Note]- audioplayers 0.10.0
>![[Pasted image 20231018083116.png]]

**Add pubspec.yaml and run Packages get**

>[!Note]- adding the package 
>![[Pasted image 20231018083229.png]]

>[!Note]- Import the package
>![[Pasted image 20231018083409.png]]

**Add a flat button to play a specific audio**
>[!Note]- Flatbutton
>![[Pasted image 20231018083532.png]]
>Adding the specific audio what to play 
>![[Pasted image 20231018083602.png]]

- You don't need to use assets/filename since the package already assumes all your files are in the assets folder

**When working with audio players always do cold restart**
- When running the app for first time just accept the permissions 

**Organize the buttons**
>[!Note]- Add the buttons 
>Copy paste the code the how many buttons needed 
>Change the colors
>Change the audio files 
>![[Pasted image 20231018084107.png]]

#### Input arguments 
**Add a function**
>[!Note]- PlaySound() function 
>![[Pasted image 20231018084655.png]]
>![[Pasted image 20231018084718.png]]


### Dart Functions - Part 1

>[!Note]- Creating and calling a function 
>![[Pasted image 20231018085317.png]]
>![[Pasted image 20231018085604.png]]
>

>[!Note]- Multiple input parameters
>![[Pasted image 20231018085859.png]]


**Fixing the button sizes**

>[!Note]- Change the background 
>![[Pasted image 20231018090139.png]]

>[!Note]- Expand widget
>![[Pasted image 20231018090344.png]]
>CrossAxisAlignmnet
>![[Pasted image 20231018090431.png]]

buildKey() - type of void that cannot be used 


**Use buildKey()**
>[!Note]- BuildKey()
>![[Pasted image 20231018092902.png]]
>![[Pasted image 20231018093021.png]]
>![[Pasted image 20231018093026.png]]


### "=>" function

>[!Note]- Arrow
>![[Pasted image 20231018093353.png]]
> is equal to 
> ![[Pasted image 20231018093435.png]]

- Runs a specific function 
Another example 

```
	int add(){
		return 5+2;
	}

	int add() => 5 + 2;
```

```
	int add(int n1, int n2){
		return n1 + n2;
	}

	int add(int n1, int n2) => n1 + n2;
```



# Requirement 

## Machine problem
- Create a musical instrument 
- Runs in the mobile device 

| Xylophone app | MP |
|-|-|
|7 notes | 1 full octave |


## Quizler 

### Why Do We Need Classes?
**Understand how computer actually work**
- 01100101- Machine code 
**4 Pillars of OOP**

>[!Note]- Make a new file 
>![[Pasted image 20231108071929.png]]
>![[Pasted image 20231108071948.png]]


>[!Note]- Make new object



>[!Note]- Import quiz brain 
>![[Pasted image 20231108072203.png]]


### Video context 
- **Statistics**



## Phase 1 November 18, 2023:
- Come up with a really good design 
- Color Hunt 
- Flat UI Colors 
- User Flow Diagram 

## Phase 2 November 25, 2023: 
- Wireframes 
- Mockups 
- POP and UXPIN
- 
## Phase 3 December 2, 2023: 

## Phase 4 December 9, 2023: 



You're task:  
Create an FAP idea for your group. Identify the market void / niche you're addressing. 

  
Phase 1:   
Design your User-Flow Diagram, save it on your google drive and a video presentation your UFD next week to allow me to have an idea of the app that you'll be creating for your FAP. Due on Nov 18.

Phase 2:   
After the UDF, create a Wire-Frame and Mock ups, link them together using POP and UXPIN. You can either create a recorded video or present this in class on Nov 25.

Phase 3: Your actual app. Due date Dec 2 (will be revisited and may be adjusted).

Your app must have: 
- Multiple screns
- Your code and presenation should demonstrate all the 4 pillars of OOP 
- Must be useful 
- Your UI should be faithful with the designs you've submitted in phase 1 and phase 2 designs 

Phase 4: Get 30 users to try out your app, prepare a google form with at least 15 questions (the more, the better) that will evaluate the UI, functionality and use of your app. Collect the data and share the ss of the responses. Due date: Dec 9  (will be revisited and may be adjusted).

Addendum:

Answer the following questions: 

1. On a scale from 1 (lowest) to 5(highest), how will you rate your app in terms of its functionality? 
2. On a scale from 1 (lowest) to 5(highest), how will you rate your app in terms of it's similarity to your phase 1 and phase 2 UI submissions? 

2023-11-15


## BMI app

>[!Note]- Pulled from Github
>![[Pasted image 20231115080946.png]]

### Flutter themes
- Custom color palette

>[!Note]- No styling 
>![[Pasted image 20231115081331.png]]

>[!Note]- Adding a theme
>Adding the dark theme
>![[Pasted image 20231115081445.png]]
>![[Pasted image 20231115081524.png]]

#### Creating your own theme data widget 

>[!Note]- Changing the primary color
>Mostly it is the background color
>The theme defaults to the light theme
>![[Pasted image 20231115081701.png]]
>![[Pasted image 20231115081809.png]]

>[!Note]- ColorZilla
>Online color picker
>Requires installation
>![[Pasted image 20231115081913.png]]

>[!Note]- Cusom Color (Hex codes)
>![[Pasted image 20231115082318.png]]


>[!Note]- Changing the background color 
>![[Pasted image 20231115082502.png]]

>[!Note]- Text Theme 
>![[Pasted image 20231115082643.png]]

>[!Note]- Interchangable theme
>![[Pasted image 20231115082811.png]]

>[!Note]- Changing other widgets 
>![[Pasted image 20231115083001.png]]

>[!Note]- Redoing everything 
>![[Pasted image 20231115083257.png]]

>[!Note]- Page 2
>![[Pasted image 20231115083324.png]]

>[!Note]- Building the second page 
>![[Pasted image 20231115083604.png]]
>

>[!Note]- Border Radius
>![[Pasted image 20231115083826.png]]

>[!Note]- Expanded widgets 
>![[Pasted image 20231115084029.png]]
>![[Pasted image 20231115084058.png]]
>![[Pasted image 20231115084128.png]]
>Add the code earlier onthe expanded widgets
>![[Pasted image 20231115084148.png]]

>[!Note]- Reusable card 
>![[Pasted image 20231115084335.png]]
>![[Pasted image 20231115084330.png]]
>You can sue the reusable card on any part 

>[!Note]- Changable color on the reusable card 
>![[Pasted image 20231115084921.png]]
>![[Pasted image 20231115084906.png]]
>![[Pasted image 20231115085225.png]]

>[!Note]- Bottom bar 
>![[Pasted image 20231115090727.png]]

>[!Note]- Custom fonts and icons
>![[Pasted image 20231115091532.png]]
>![[Pasted image 20231115091556.png]]
>![[Pasted image 20231115091657.png]]
>![[Pasted image 20231115091758.png]]
>![[Pasted image 20231115091910.png]]


>[!Note]- Icon Data 
>![[Pasted image 20231115092502.png]]
>![[Pasted image 20231115092601.png]]

>[!Note]- icon_content.dart
>![[Pasted image 20231115092753.png]]

>[!Note]- Inactive card color 
>![[Pasted image 20231115093549.png]]
>On Tap
>![[Pasted image 20231115093632.png]]
>![[Pasted image 20231115093916.png]]



### Enum 
- For different types 

>[!Note]- Enum
>![[Pasted image 20231122081227.png]]

>[!Note]- Enum Examples 
>![[Pasted image 20231122081626.png]]

>[!Note]- Improved code with Enum
>![[Pasted image 20231122082009.png]]
>![[Pasted image 20231122081957.png]]


### Ternary Operator 
>[!Note]- Dart Ternary Operator 
>![[Pasted image 20231122082148.png]]

>[!Note]- Example 
>![[Pasted image 20231122082440.png]]


>[!Note]- Functions
>![[Pasted image 20231122083807.png]]


### Routes & Navigation 

>[!Note]- Main.dart and screen1  
>![[Pasted image 20231129081614.png]]
>![[Pasted image 20231129081621.png]]
>![[Pasted image 20231129081640.png]]

>[!Note]- Routes
>![[Pasted image 20231129082733.png]]

>[!Note]- Initial Route 
>![[Pasted image 20231129082957.png]]

>[!Note]- Named Route 
>![[Pasted image 20231129082950.png]]

---
# Script

So good evening sir ako po si Nigel ang backend developer ng pomotasker.

I'll be explaining how the app functions in the background. 


So we start at the main.dart main function. so async po siya kasi maghihintay po siya ng respond galing sa isang flutter package which is hive, which is a key value database. Basically nagfufunction po siya as like a database ng boxes na kung saan pwede ka mag store ng objects for the app. 

So ioopen ni main yung box which is pomobox. Then naka set yung app as portraitUP orientation lang. 

So pag pasok po sa build. which is everytime maoopen po yung app meron po tayong splash screen. Tapos if ioopen yung app for the first time meron po tayo screen na get_started na ieexplain ni Mark Nicasio. If not diretso po siya sa main screen which is pomodoroscreen. 

Sir since sa sobrang dami ng lines of code I'll be just providing snapshots para mas madali po ma explain yung code. So pag pasok po ng main screen which is pomodoroscreen. 

First iexplain ko muna po yung backbone ng both features ng app which can be found in the database. dart. So we have two objects ToDoDatabase and Timer Data. ang ToDoDatabase ay para sa todo list na mula sa isang Hivebox which is yung pomobox. Meron tayong list na in every list merong title, boolean, date and time for the deadline and yung descriptions yung date and time po strings lang po sila since hive is a simple database. if need po istore ang ibang objects kailangan pa po ng adapters na magcoconvert from objects to its binaryform.

inside the ToDoDatabase ay yung create InitialData which is used na if null yungdatabase or for the first time siya gagamitin then magcrecreate ng dalawang tasks para mashowcase sa user for the first time kung paano siya magfucntion. 

loadData ay para ma kuha ng mainscreen yung value na list of lists na kuha from the pomobox na may key TODOLIST and updateDatabase ay nagrurun everytime maychanges sa todo list ng user
![[Pasted image 20231201202347.png]]
 TimerData which is galing rin sa pomobox na in keys like WORKTIMER, SHORTTIMER, LONGTIMER ay may kanya kanyang value na Map which is meron map of key na min and sec which holds the data int for the details ng every type of timer. Meron rin siya na initial setters, updateSetters and loaders which acts as the getters for the main screen. 

![[Pasted image 20231201202405.png]]
Not on the main screen Meron tayo Class na PomoTasker which inherits StateFulWidget funcitonalities for the timer and to-do list. Ang functions ng getWorkTime, getShortTime, and getLongTime is kukunin yung time details from the HiveDatabase which runs the getters from the TimerData sa database. 
![[Pasted image 20231201203802.png]]
These methods ay icoconvert nila into Duration na mastore sa 3 variables 
![[Pasted image 20231201203939.png]]

So meron tayong _MyTimerstate na ininherit yung state ng statefulwidget ng pomo tasker. which is meron tayong SingleTickerProvider na natitick and iimport ang CustomTimer package

![[Pasted image 20231201204657.png]]

The imter is initiated that starts on the working timer. 

![[Pasted image 20231201204727.png]]


and meron rin tayong function na didispose yung tiemr after the session 
![[Pasted image 20231201204748.png]]

Sa timer dito na rin papasok yung todo list which access the pomobox and gets the data which isd yung TodoDatabase. 

if wala sa box yung todolist this also means the app was opened for the first time. Then it runs the initial timer data function sa database
![[Pasted image 20231201205048.png]]

dito rin sa main scren meron tayong TextEditingControllers that gets the values form the textfields if the user deicides to add a task. 
![[Pasted image 20231201205619.png]]

If a user decides to add a task  saveNewTask function ay iseset niya yung bagong state adding the task at the same time irurun yung database object to run the updateDataBase method. 
![[Pasted image 20231201205647.png]]

Sa app meron tayong button which kung saan yung user ay gagawa ng panibagong task. Since ang controllers natin ay global ang gianwa ko is pag run ng function icleclear niya all values na meron sa controllers. 
and irurun ang showDialog which I will be explaianing later but basically iniimport niya yung controllers and yung method na saveNewtask bago ipakita yung Form na isang alert dialogue para makapag add yung user ng bagong task.
![[Pasted image 20231201210104.png]]

Similary yung updateTask Function ay ginagawa ang pag show dialogue but ang difference is before ipakita yung  Alert Dialogue iniimport ko muna yung task dtails sa controllers para pag pop up ng dialogue makikita ng user ang editable task details 


saveUpdateTask sets the state and saves the new details based on the list_index ng task na inedit. Similar siya sa save newtask function kanina 
![[Pasted image 20231201210445.png]]

The build method is the one of the longest block sa pomodoro screen since including na rin dito yung front end codes na maeexplain later. but I would like to focus on sa body where dito makikita yung BuildCustom timer which is isang object
![[Pasted image 20231201210632.png]]
Dito rin makikita yung isang block of code which acts as the method of showing all the tasks coming from the database everytask is enclosed in an Elevated button na when pressed dito mapopop up and DialogueBox or alert box that runs the update tasks 

![[Pasted image 20231201210720.png]]



and ofcourse this also houses the add task button na magpapakita ng Same dialogue box but with different method and functions of updating sa database. 

![[Pasted image 20231201210821.png]]

the timerbuttons class enhouses yun dialogue box na may form na pwede iedit yung user yung minutes and seconds ng bawat timer Working, Short Breaks and long breaks. It has its own controller na kukunin ang bawat value and istostore sa database
![[Pasted image 20231201211908.png]]![[Pasted image 20231201211930.png]]

pagpinindot ni user ang ok button irurun ng database ToDoList object ang update setters then update sa database 

![[Pasted image 20231201213450.png]]

BUild custom timer controlles the timer whether the user is working on short break or long break meron siyang listener na dinedetect if tapos na yung timer then irurun yung getters para ma check if may updates sa database about sa data ng timer tapos may booleans para ma check kung anong type ang timer ang ipapakita. May method na jumpTo sa package para lilipat yung timer sa specific time na timer type ng user. 
![[Pasted image 20231201215121.png]]

Dito na rin makikita yung functionalities ng timer which in every tick magbabago yung Text showing yung minutes and seconds remaining and yung buttons which yung mga buttons is enclosed sa isa pang function na it acts as a class pero expanded function lang siya na rineread ang string and irurun yung function para ipause, start, reset or stop ang time 
![[Pasted image 20231201215516.png]]
![[Pasted image 20231201215526.png]]


Sa todo tile ay may object siya na may task name, onChanged, taskCompleted isang boolean and taskCOmpletion na nagdedetect if compeleted na yung task 

![[Pasted image 20231201222113.png]]