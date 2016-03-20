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

