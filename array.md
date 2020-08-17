# Array 
An array is a collection of values of the same data type. In other words, it is similar to a container holding multiple values.

## Array Initialization
- Array Initialization is step where we define an array size and its elements.
- It is important to note that the array size should `always` be a constant value.
- Also, the elements stored in an array, follow zero-based indexing instead of 1-based indexing.
- Here is an example of an array initialization -
```
INPUT
# include <iostream>
using namespace std;
int main()
{
    // defining constant for array size
    const int array_size = 5;
    // assigning size 5 to array and storing 5 integers in it. Also, int at the beginning signifies that all elements in the array are of type int.
    int first_array[5] = {1,2,3,4,5};
}
```

## Changing and Accessing elements in an array
- Changing and accessing elements in an array can be tricky, especially due to the zero-based indexing used by the array.
- Here is an example which builds up on the previous one -
```
INPUT
# include <iostream>
using namespace std;
int main()
{
    // defining constant for array size
    const int array_size = 5;
    // assigning size 5 to array and storing 5 integers in it. Also, int at the beginning signifies that all elements in the array are of type int.
    int first_array[5] = {1,2,3,4,5};
    // Changing 5 to 7.
    // According to zero-based indexing, the position of the number 5 is 4.
    first_array[4] = 7
    // Printing all elements of the array now
    for(int i = 0; i < 5; i++)
    {
        cout << first_array[i] << endl;
    }
}
OUTPUT
1
2
3
4
7
```