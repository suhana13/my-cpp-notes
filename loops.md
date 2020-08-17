# Loops
- The three most used loops in C++ are:
## While loop
- It is a pretest loop i.e it tests for the condition entered by the programmer and only then gets executed.
- The two main features of the while loop are:
1. It checks for a condition
2. It continues to get executed till the condition is met
- Here is an example of a `while loop`
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int num = 1;
    while(num <=4)
    {
        cout << num << endl;
        num = num + 1;

    }
}
OUTPUT
1
2
3
4
```
- Here, we assigned our integer variable num, a value of 1.
- Then, we checked if num was less than or equal to 4. If it was true, we let num enter the while loop.
- After that, we displayed the value of num on the output console and increases its value by 1.
- Now, after a total of 4 repetitions of the while loop, the value of num became 5 and hence, it no longer entered the while loop.

## Do while loop
- It is a posttest loop i.e it tests for the condition entered by the programmer only after getting executed at least once.
- So, it is essentially a while loop which gets executed atleast once irrespective of the condition.
- Here is an example of a `do-while loop`
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int num = 5;
    do 
    {
        cout << num << endl;
        num = num + 1;

    }
    while(num <=4);
}
OUTPUT
5
```
- Here, even though the value of num is 5 and it doesn't enter the while loop, it does get executed once, thus displaying the value of num on the output console.
- Also, note that for a do-while loop, we put a semicolon at the end of the while statement but we don't put one in a while loop. This is because semicolon basically marks the end of a statement as as a do-while loop essentially ends after the while condition, we put a semicolon af†er it.

## For loop
- It is a pretest loop, like the while loop.
- It requires three major conditions to be specified: initialization, test, update.
- I will explain these terms and the `for loop` better with the help of an example
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    for(int i = 0; i < 5; i++)
    {
        cout << i << endl;
    }
}
OUTPUT
0
1
2
3
4
```
- Here, initialization refers to the `int i = 0` statement. So, unlike a while loop, we initialize the variable within the for loop itself.
- Test refers to the `i < 5` statement which decides whether the loop should continue to be executed or not.
- Lastly, update refers to the `i++` statement according to which the value of i is increment at the end of each iteration of the for loop.
