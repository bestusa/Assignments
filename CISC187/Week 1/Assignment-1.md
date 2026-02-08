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
        cout << elements[i] << " ";
    }


    cout << sizeof(elements);

    for (int i=0; i < 100; i++) {
        std::cout <<"The memory address of element[" << i << "] is: " << &elements[i] << endl;
    }

    return 0;
}
