# Formatting output
- It is common for the programmer to desire a specific output display, with appropriate amount of spacing, specific precision of a number etc.
- Here, we will discuss some of the common ways in which we can format the output.

## Header file 
- Firstly, we need an important header file to format the output. It is called `iomanip`.

## setw
- This stream manipulator(aka function) stands for set width.
- This can be used to provide a few spaces between two output statements or numbers.
- It can also serve as a padding for a specific output.
- Here is an example using setw.
```
INPUT
# include <iostream>
# include <iomanip>
using namespace std;
int main()
{
    int num = 5;
    cout << num << endl;
    cout << setw(3) << num;

} 
OUTPUT
5
  5
```
- Here, the first line displays the number 5 without any spacing.
- However, the second line displays the number 5 with 2 spaces in front of it and the third space being the number 5 itself.

## setprecision
- This stream manipulator is used to display a specific number of digits in numerical data .
- Its allows the programmer to control the level of precision of a number that should be visible to the user or displayed on the output console.
- Also, setprecision() tends to round off numbers in case their precision is higher than what is displayed on the output console.
- Here is an example using setprecision
```
INPUT 
# include <iostream>
# include <iomanip>
using namespace std;
int main()
{
    double num = 5.78264;
    cout << num << endl;
    cout << setprecision(4) << num;

}
OUTPUT
5.78264
5.783
```
- Here, the first line displays the number as is or as defined by the programmer.
- THe second line displays the number with a precision of 4 i.e it displays the first four digits of the number with the last one being rounded up from 2 to 3 due to the 6 following it.


## fixed
- Often, when the precision demanded by the programmer is less than the actual value of the variable, the output tends to be displayed in scientific notation. To avoid this situation, we use the fixed manipulator.
- When we used fixed and setprecision together, the precision specified by setprecision() refers to the number of digits after the decimal point that must be displayed on the output console.
- Here is an example which shows the use of this manipulator
```
INPUT
# include <iostream>
# include <iomanip>
using namespace std;
int main()
{
    double num = 50456.8345;
    cout << num << endl;
    cout << setprecision(3) << num << endl;
    cout << fixed << setprecision(3) << num;


}
OUTPUT
50456.8345
5.05e+04
50456.834
```
- Here, in the first line, the number is displayed as is. 
- In the second line, the number is displayed in scientific notation as I mentioned above.
- In the last line, the number is displayed with 3 digits after the decimal point as we used the `fixed` and `setprecision` manipulators together.

## showpoint
- This manipulator facilitates the display of trailing zeroes for a number, on the output console.
```
INPUT 
# include <iostream>
# include <iomanip>
using namespace std;
int main()
{
    double num = 5.7;
    cout << num << endl;
    cout << setprecision(4) << num << endl;
    cout << showpoint << setprecision(4) << num << endl;

}
OUTPUT
5.7
5.7
5.700
```
- As shown above, when we used setprecision() without showpoint(), the trailing zeroes arent displayed while when these two manipulators are used together, the trailing zeroes are shown.
- 
