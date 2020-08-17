# Understanding different data types:

## Numeric data types:
### 1. Integer

* As the name indicates, an integer data type stores integral values. 
* In addition, there are further subdivisions of integer data types:
~~~
1. short             - stores integers within a small range.
2. unsigned short    - stores positive integers within a small range.
3. int               - stores integers within a range bigger than short.
4. unsigned int      - stores positive integers within a range bigger than short.
5. long              - stores integers within a range bigger than int.
6. unsigned long     - stores positive integers within a range bigger than int.
~~~

### 2. Floating-point 

* Floating point numbers are basically numbers storing decimal values.
* There are 3 data types that store floating point numbers
~~~
1. float         - stores floating point numbers.
2. double        - stores floating-point numbers with a greater precision that float and within a larger range.
3. long double   - stores floating-point numbers with the same precision as a float and within a larger range than double.
~~~


## String or character data types:
### 1. Char
* This data type is used to store a single character, which could be a single letter or symbol.

### 2. String
* It is used to store a group of characters or a string.
* Remember to define a string variable, you must include another header file named **string**.


## Boolean data type
- These variables are set to either `true` or `false`.
- They can also be given binary values where `0` implies false while `1` implies true.
  
## Variable declaration using the above data types
* In C++, it is vital to define the data type of a variable.
* Here is an example that will take into account all the data types we have learnt so far.
```
#include <iostream>
#include <cstring>
using namespace std;
int main()
{
  // defining an integer
  int num_int = 2;
  // defining a float
  float num_float = 3.4;
  // defining a double
  double num_double = 567.67;
  // defining a long double
  long double num_double_long = 180000.6789;
  // defining a char
  char char_name = 'A';
  // defining a string
  string greeting_message = "Hey!";
  // defining a boolean expression
  bool statement;
  statement = TRUE;
}
```

## Determining the size of a data type
 ``sizeof` operator
- It is a special operator which determines the number of bytes used by a specific data type.
```
INPUT
#include <iostream>
using namespace std;
int main()
{
  int number;
  cout << sizeof(number) << endl;
  
}
OUTPUT
4
```

