
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

