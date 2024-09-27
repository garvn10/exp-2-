# CDS-Experiment--02 /* 
Aim:To study and implement C++ Program Structure (Data Types) an storage class.<br>
Software: Visual Studio Code

Theory:<br>
In C++, data types have specific sizes which determine how much memory is allocated for each type. For example, an int typically uses 4 bytes, char uses 1 byte, float uses 4 bytes, and double uses 8 bytes. Sizes can vary based on the system and compiler.<br>

Storage classes define the scope, visibility, and lifetime of variables/functions. <br> The four storage classes are:<br>

auto: Default for local variables.<br>
static: Retains value between function calls, local to the file if used in global context.<br>
extern: Extends visibility across multiple files.<br>
register: Suggests storing variable in a CPU register for faster access, though modern compilers often ignore this.<br>
These classes help manage how and where data is stored and accessed within a program.<br>
Code for the program:<br>
Size of Datatypes:<br>
```
#include <iostream> 
using namespace std; 

int main() 
{
    char a = 's';
    cout << "The size of a character is: "<< sizeof(a) << endl;
    int b = 123456;
    cout << "The size of an integer is: "<< sizeof(b) << endl;
    short int c = 1233;
    cout << "The size of a short integer is: "<< sizeof(c) << endl;
    long int d = 12739482;
    cout << "The size of a long integer is: "<< sizeof(d) << endl;
    long long int e = 122388728;
    cout << "The size of a long long integer is: "<< sizeof(e) << endl;
    float f = 27168.5;
    cout << "The sie of a float is: " << sizeof(f) << endl;
    double g = 84273923.89877;
    cout <<"The size of a double floating point is: "<< sizeof(g) << endl;
    long double h = 8742980.789793;
    cout<< "The size of long double floating point is: "<<sizeof(h) << endl;
    cout<< "The size of a wide character is: "<<sizeof(wchar_t) << endl;
    return 0;
} 
```


Code for storage class: 
```

#include<iostream>
using namespace std;

extern int extern_variable =30;


int main()
{
    auto a = 8;
    register int registered_variable = 100;
    static int s = 7;
    cout << "The local variable: "<< a << std::endl;
    cout <<"The variable in register: "<<registered_variable<<endl;
    std::cout<<"External variable: "<<extern_variable<<endl;
    s = 10;
    cout<<"The static variable: "<<s<<endl;

}
```

Output 1:
![image](https://github.com/user-attachments/assets/ac668922-8829-463b-a205-0058032977ba)

Output 2:
![image](https://github.com/user-attachments/assets/852e2034-b066-437c-ad65-220e2c28d363)

Output 3:
![image](https://github.com/user-attachments/assets/6a6230fb-b327-4135-832c-5e01070477cb)


Conclusion:
In this experiment we have learnt to check the size of the datatypes and made program using storage class example: auto static and etc.
