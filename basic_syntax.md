# Basic Syntax

    //My first C++ code
    #include <iostream>  
     using namespace std; 
    int main() 
    { 
      cout << "Welcome to the world of CS!";
    }



Let's try to understand each line one by one.

## Comments

    //My first C++ code </br>

* This is just a comment. The compiler would not read it. It is for your own understanding or for others who might want to understand your code better. 
* So, to write a code in C++, just put two forward slashes **("//")** and type in your comment.
* However, the forward slashes work well when you wish to add only a single-line comment. If you want to add multi-line comments, use a slash followed by a star __("/* your_comment */")__. Here is an example of the same:
```
/* This is my first C++ code.
I am truly excited to learn a new CS language. */

```

```
#include <iostream> 
```

* Here, the pound sign merely indicates that the line would be read by the preprocessor and not by the compiler.
* iostream is a header file which helps us to input values from the keyboard and display the output on the screen. 

## Header files
```
using namespace std;
```
* This statement specifies that we will be using several functions and objects which are a part of the namespace named "std".

## Defining functions
```
int main() 
    { 
    }
```
* This defines a function named "main".
* In general, the main function in C++ is the first or the starting function. If someone is reading your code, they should begin reading it from the main function.
* The prefix "int" mainly suggests that the function will return an integer value to the operating system, once its executed.
* The braces are meant for you to write your code in.

## The cout object
```
cout << "Welcome to the world of CS!";
```
* The *cout* object is used to display the desired output on the screen.
* Remember, in order to use the *cout* operator, we must include the header file named *iostream*.
* Here, we simply display a string to the output console.

## The importance of semicolon in C++
* In C++, if we wish to end a statement, we must use a semicolon at the end of the statement.
* Like, in the above cout statement, we ended it with a semicolon.
* A semicolon is a way of telling the compiler that a specific statement has ended. 
* However, we didn't include a semicolon in the header file inclusion statement as it is meant for the preprocessor to read and not for the compiler to read and process.

## The cin object
```
int num;
cout << "Please enter any integer value";
cin >> num;
\\ user enters an integer
```
- The *cin* object is used to take an input by the user, though the data type of the input is predefined.
- In the example above, we define a integral variable and then the user inputs a value of the variable.
- Most of the cin statements are preceeded by a cout statement which displays a prompt (i.e a message for the user to input something )