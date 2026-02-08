# Christopher Aragon
# CISC 187 / Professor Khan

## Activity 1 Arrays

```C++
cout << "This is Activity 1 Arrays";
```
#include <iostream>
using namespace std;

int main() {
    int  elements[100];

    for (int i=0; i < 100; i++) {
        elements[i] = i;
        std::cout<< elements[i] << " ";
    }


    cout << sizeof(elements);

    for (int i=0; i < 100; i++) {
        std::cout <<"The memory address of element[" << i << "] is: " << &elements[i] << endl;
    }

    return 0;
}

//notes:
//Read-  Is considered a single step operation to retrieve an element
    //#steps - 1 step per element
//insertion- refers to adding an element to an existing array
    //if the insertion takes place at the end of the array, then the compiler/interpreter would increase the size of an array and allocate a memory address.
//deletion- refers too removing an existing value form an arra. (array rearranges the size/index numbers
    //if the deletion happens at index 0, then one step for deletion and N-1 steps to shift the elements in an array.
    //For example, if an array size is 100, one step for deletion and 99 steps to shift elements in an array, which gives a total of N steps.
//search- refers to looking for a particular element in an array (can take one or more steps)
    //if the element is at index 0, then it would take only a single step. If the element is at the last index, then it would take N steps.



//1  explain mycode
//2  4 bytes
//3  100 (101 for steps referring to insertion operations)
//4  searching for a specific element in an array depends where is that element located (my code element 49 should take 49 steps to recover)\
//5 research how to find memory address in an array. --use address-of operator "& "
