# Ex.No:2  
# Ex.Name: Write a C++ program to demonstrate the this pointer.  

## Date:  

## Aim:  
To write a C++ program that demonstrates the use of the `this` pointer to access or modify data members of a class.  

## Algorithm:  
1. Start the program.  
2. Define a class with a private integer data member.  
3. Define a member function to set the value of the data member using the `this` pointer.  
   - Syntax: `this->variable = value;`  
4. Define another function to display the value of the data member.  
5. In the `main()` function, input a number.  
6. Create an object of the class, set the value using the `this` pointer, and display it.  
7. Stop the program.  

## Program:  
```cpp
#include <iostream>
using namespace std;
class First 
{
    public:
    string a;
    void disp()
    {
        cin>>a;
        cout<<"x = "<<a<<endl;
    }
};
class Second 
{
    public:
    void disp()
    {
        First ob1;
        ob1.disp();
    }
};

int main()
{
    Second ob2;
    ob2.disp();
	return 0;
}
```

## Output:
<img width="855" height="311" alt="image" src="https://github.com/user-attachments/assets/41a9fdfc-1ebf-4a7e-95fb-f4dc8666df13" />

## Result:
```
Input:
20

Output:
x = 20
```
