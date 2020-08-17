# File input and File output
- Many a time, the programmer wishes to retrieve or read data from a file, perform some operations on the data read and store the output in another file. 
- Here, we will discuss some of the techniques used in carrying out the above operation.

## Header
- We need the `fstream` header to gain read and write permissions for a file.

## Datatypes required
- `ifstream` - It stands for input file stream. This data type is used to read data from an existing file.
- `ofstream` - It stands for output file stream. This data type is used to write data to a file or create a new file where the output is stored.
- `fstream` - It stands for file stream. It performs all the functions of ifstream and ofstream.

## Opening a File
- Let us assume that we define infile as an ifstream object. So. in order to open a file, we must do the following
```
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    ifstream infile;
    infile.open('input.txt');

}
```
- Here, we assume that `newfile.txt` is present in the same directory where we are running our code. Else, we will have to specify the relative path of the file which we wish to read for data retrieval.

## Reading data from a File
- After, we have opened the file, we can easily read the data from it as well.
- All we need to do is use `infile` instead of `cin`
```
infile >> num_1 >> num_2;
```

## Writing data to a file
- Now, we need to store the output of our program in a file.
- For that, we need to use the ofstream object as it grants us writing permission for a file
- Again, let us assume that we define outfile as an ofstream object. So. in order to open a file, we must do the following
```
#include <iostream>
#include <fstream>
using namespace std;
int main()
{
    ofstream outfile;
    outfile.open('output.txt');
    outfile << "This is the first statement written in the output file;
}
```
- Here, again we use `outfile` instead of `cout` to display and store the output in a file instead of displaying it on the output console.

## Closing a file
- Closing a file is very simple and can be done as follows:
`outfile.close();`