# Ex.No:3  
# Ex.Name: Write a C++ program for Class conversion that can be achieved by conversion function which is done by the use of operator overloading (use Integer data).  

## Date:  

## Aim:  
To write a C++ program to demonstrate class-to-class type conversion using a conversion function achieved through operator overloading.  

## Algorithm:  
1. Start the program.  
2. Define a source class with an integer data member and method to read value.  
3. Define a destination class with an integer data member and a constructor that accepts an object of the source class.  
4. In the source class, overload the type conversion operator to return the integer value.  
5. In the destination class constructor, assign the source object’s value to its own member.  
6. In `main()`, input integer value into source object.  
7. Convert the source object to destination object implicitly/explicitly.  
8. Display the values of objects after conversion.  
9. Stop the program.  

## Program:  
```cpp
#include <bits/stdc++.h>
#include <string.h>
using namespace std;
class Class_type_one 
{
   float a=0;
   public:
   float get()
   {
     cin>>a;
     return a;
   }
   void display()
   {
       cout<<a<<endl;
   }
};
class Class_type_two 
{
   float b=0;
   public:
   void operator=(Class_type_one a)
   {
       b=a.get();
       a.display();
   }
   void display()
   {
      cout<<b;
   }
};
int main()
{
    Class_type_one a;
    Class_type_two b;
    b = a;
    b.display();
    return 0;
}
```
## Output:
<img width="872" height="357" alt="image" src="https://github.com/user-attachments/assets/3fc85ebe-7a0c-4f8b-b7d6-1e607ca4737c" />

## Result:
```
Input:
10

Output:
10
10
```
