# Ex.No:4  
# Ex.Name: Write a C++ program to override the print() function in the base class with the print() function in the child class using the concept of virtual functions.  

## Date:  

## Aim:  
To write a C++ program that demonstrates **function overriding** using **virtual functions**, where the base class defines a virtual `print()` function that is overridden in the derived class.  

## Algorithm:  
1. Start the program.  
2. Define a base class containing a virtual function `print()`.  
3. Define a derived class that overrides the `print()` function.  
4. Create a base class pointer and point it to an object of the derived class.  
5. Call the `print()` function using the base class pointer.  
6. Due to the virtual keyword, the derived class version of the function will be invoked.  
7. Display the overridden output.  
8. Stop the program.  

## Program:  
```cpp
#include<iostream>
using namespace std;
 
class base {
    public:
    virtual void print(string s)=0;
};
 
class derived : public base
{
    public:
    void print(string s)
    {
        cout<<s<<endl;
    }
};
 
int main()
{
    string s;
    cin>>s;
    base *bptr;
    derived d;
    bptr = &d;
    bptr->print(s);
 
   
    return 0;
}
```

## Output:
<img width="882" height="332" alt="image" src="https://github.com/user-attachments/assets/fe50c87f-9653-48f2-9bb8-79dd7f310fbc" />

## Result:
```
Input:
1

Output:
VirtualOne
```
