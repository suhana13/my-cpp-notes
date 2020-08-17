# Conditional statements
- This document will cover conditional statements including relational operators, if-else if-else statements and logical operators.

## Relational operators:
- They are used to evaluate relations between numerical data.
- They are binary in nature i.e they require two operands.
- Here is a list of relational operators:
```
1. <     - less than
2. >     - more than
3. <=    - less than or equal to
4. >=    - more than or equal to
5. ==    - equal to
6. !=    - not equal to
```
## If-Else if-Else 

### If statements
- Used to check a specific condition and thereafter execute a specific command in case the condition is fulfilled.
- In most cases, the relational operators we discussed above, are used to validate the condition.
- Here is an example using an `if` statement
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int x, y;
    x = 5;
    y = 9;
    if(x<y)
    {
        cout << "X is less than Y";
        
    }
}
OUTPUT
X is less than Y
```
- Note here that we `didn't use a semicolon after the statement if(x<y)`. This is because the statement hasn't ended after the if condition and it continues to the output that should be printed on the output console in case the statement is true.


### If-else statements
- These statements are just a continuation of the if statements with the additional detail of what should be done in case the if statement isn't satisfied.
- Here's an example using an `if-else` statement
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int x, y;
    x = 9;
    y = 5;
    if(x<y)
    {
        cout << "X is less than Y";
        
    }
    else
    {
        cout << "X is equal to or greater than Y";
    }
}
OUTPUT
X is equal to or greater than Y
```
- Another way of writing if-else statements is this : `stat_1 ? stat_2 : stat_3`
- Here stat_1 is `(x<y)`, stat_2 is `cout << "X is less than Y"` and stat_3 is `cout << "X is equal to or greater than Y"`
### If-else if-else statements
- These statements are an extension to the if-else statements.
- These statements starts with an if condition, then in case it fails, we move to the next else if condition and the process continues till the else statement occurs.
- Here is an example which shows the usage of If-else if-else statements
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int x = 74
   
    if(x > 90)
    {
        cout << "A";
    }
    else if(x > 80)
    {
        cout << "B";
    }
    else if(x > 70)
    {
        cout << "C";
    }
    else
    {
        cout << "D";
    }
}
OUTPUT
C
```

## Logical Operators
- These operators are used to connect two relational expressions.
```
!   - not
&&  - and
||  - or
```
- Here is an example using logical operators.
```
INPUT
#include <iostream>
using namespace std;
int main()
{
    int x = 5, y = 10, z = 15;
    if( (x > 0) && (y > 5))
    {
        cout << " The sum of x and y is greater than 5 "
    }

}
OUTPUT

The sum of x and y is greater than 5
```