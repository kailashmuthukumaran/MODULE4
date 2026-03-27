# Ex.No:5  
# Ex.Name: Write a C++ program to demonstrate the concept of object composition (use string data).  

## Date:  

## Aim:  
To write a C++ program demonstrating **object composition**, where an object of one class is created inside another class and initialized through a constructor initializer list.  

## Algorithm:  
1. Start the program.  
2. Define a class `A` with a constructor that accepts a string value and displays a message when invoked.  
3. Define another class `B` which contains an object of class `A` as a data member.  
4. Use a constructor initializer list in class `B` to initialize the object of class `A`.  
5. In class `B`, define a function to display data from both class `B` and its member object `A`.  
6. In `main()`, read a string value and create an object of class `B` while passing the string to its constructor.  
7. Display the result.  
8. Stop the program.  

## Program:  
```cpp
#include <iostream>
using namespace std;
class A
{
    public:
    string x;
    A(string a)
    {
        cout<<"Constructor A(string a) is invoked"<<endl;
        x=a;
    }
};
class B
{
    public:
    A obj2;
    B(string a):obj2(a)
    {
        cout<<"Data in object of class B = "<<a<<endl;
        cout<<"Data in member object of class A in class B = "<<obj2.x;
    }
    
};

int main()
{
    string x;
    cin>>x;
    B obj1(x);
	return 0;
}
```

## Output:
<img width="874" height="427" alt="image" src="https://github.com/user-attachments/assets/e6f4fcd1-3b3c-4e09-b255-5c975ef883e2" />

## Result:
```
Input:
KUMAR

Output:
Constructor A(string a) is invoked
Data in object of class B = KUMAR
Data in member object of class A in class B = KUMAR
```
