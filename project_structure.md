# 1. Project sttructure guidelines

## 1.1 Project structure

New projects should follow the Android Gradle project structure that is defined on the [Android Gradle plugin user guide](http://tools.android.com/tech-docs/new-build-system/user-guide#TOC-Project-Structure). The [ribot Boilerplate](https://github.com/ribot/android-boilerplate) project is a good reference to start from.

## 1.2 File naming

### 1.2.1 Class files
Class names are written in [UpperCamelCase](http://en.wikipedia.org/wiki/CamelCase).

For classes that extend an Android component, the name of the class should start with the name of the component; for example: `ActivitySignIn`, `FragmentSignIn`, `ServiceImageUploader`, `DialogChangePassword`.
For other specific kind of classes like enum and interfaces `Enum` and `I` will be used; for example:
`EnumOperations`, `ICustomNetwork`.


### 1.2.2 Resources files

Resources file names are written in __lowercase_underscore__.

## 1.3 Package naming
Packages names shall be only with lowercase
Packages will have meaning names and will be logical groups of classes.

## 1.4 Resources directories.
'Layouts' directory in reources will contain subdirectories that will be determined by the activities and fragments. If one activity have more than one fragment for each fragment a new directory will be created.
Also two more directories will be created :

`general` - layouts that are in use in more than one activity/fragment

`custom` - layouts that belongs to custom views that are used in application.

# 2. Project components

## 2.1 Libraries
There are part of the libraries that will be integrated into the project from the begging even that some of them will not be in use from the first day.

### 2.1.1 Crashlytics
Library to receive reports about crashes in the application automatically without any intervention fron the user.
The reports also contains statistics about the performance of the application like usage of cpu, memory, network and so on.

It's very important to start following the results and the statistics from the first moment of the application.
To read more about it can be done [here](https://crashlytics.com/)

### 2.1.2 Logs
Internal library that is overriding the standard `Log` library. It includes a log with few improved functionality and also a `LogStorage`. The `LogStorage` is capable in saving the logs according to specific parameters. Those logs files can be retrived from the device so it will be possible to check what is happening.

### 2.1.3 EventBus
EventBus will be used to pass data inside the app.
Details about it can be found [here](https://github.com/greenrobot/EventBus)


