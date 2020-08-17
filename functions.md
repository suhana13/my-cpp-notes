# Functions
-  A function is a group of statements which solve a specific purpose.
## Function definition
-  Each function definition consists of the following components:
1. Function Name
2. Return type
3. Function parameters
4. Body
- The `int main()` statement that we have used so far is in fact a function whose name is *main* and return type is *int*. Also all the statements enclosed within the braces following the `int main()` statement constitute the body of the function. We,usually, don't specify any parameters for the main function but the paramters for a function are specified in the paranthesis written after the name of the function. 
- Here is an example of a function
```
INPUT
include <iostream>
using namespace std;
double sum(double num_1, double num_2)
{
    double sum;
    sum = num_1 + num_2;
    return sum;
}
int main()
{
    double sum;
    sum = sum(10.5,9.9);
    cout << "The sum of 10.5 and 9.9 is "<< sum;

}
OUTPUT
The sum of 10.5 and 9.9 is 20.4
```
- In the example above, we have two functions, namely `sum` and `main`. Let's use the sum function as an example to understand the various components of a function.
```
double sum(double num_1, double num_2)
{
    double sum;
    sum = num_1 + num_2;
    return sum;
}
```
- Here, `double` at the beginning of the function definition is the return type of the function. We return the sum of two numbers with double as their datatype and consequently, the sum must be of double type too.
- `sum` refers to the name of the function.
- `double num_1, double num_2` refer to the parameters of the function. While specifying the function parameters, we must mention their datatypes and their respective names.
- All the statements listed in the braces constitute the body of the function.
## Function prototype
- It is considered good practice to define functions after the main function. In such cases, we use a function prototype before the main function. It basically tells the compiler that function definition follows the main function and instructs it not to throw an error when the function is called in the main function.
- A function prototype is pretty much a truncated version of a function definition. It consists of the following components:
1. Function name
2. return type
3. datatype of the variables in a function parameter
- Now, I'll write the above program that I used as an example, by using a prototype for the sum function.
```
INPUT
include <iostream>
using namespace std;
double sum(double ,double );
int main()
{
    double sum;
    sum = sum(10.5,9.9);
    cout << "The sum of 10.5 and 9.9 is "<< sum;

}
double sum(double num_1, double num_2)
{
    double sum;
    sum = num_1 + num_2;
    return sum;
}
OUTPUT
The sum of 10.5 and 9.9 is 20.4
```
## Local and global variables
- The variables defined in a function have a limited scope i.e they can be used and they retain their values witihin the function only. Such variables are called `local variables`.
- However, certain variables can be used througout the program. They must be defined before the main function and are called `global variables`.
## Reference variables
- Reference variables are used as function parameters which tend to modify the value of the original variable defined in another function.
- Below are two examples, one the usage of a reference variable and one with it.
```
EX -1 (with reference variable)
INPUT
include <iostream>
using namespace std;
// function prototype
void triple(int &);
// main function
int main()
{
    int num = 7;
    cout << "The value of num is " << num << endl;
    // calling the triple function
    triple(num);
    cout << "The modified value of num is " << num << endl;
}
// triple function
void triple(int &var)
{
    var = var*3;
}
OUTPUT
The value of num is 7
The modified value of num is 21

EX -2 (without reference variable)
INPUT
include <iostream>
using namespace std;
// function prototype
void triple(int );
// main function
int main()
{
    int num = 7;
    cout << "The value of num is " << num << endl;
    // calling the triple function
    triple(num);
    cout << "The modified value of num is " << num << endl;
}
// triple function
void triple(int var)
{
    var = var*3;
}
OUTPUT
The value of num is 7
The modified value of num is 7
```
