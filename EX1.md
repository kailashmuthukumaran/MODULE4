# Ex.No:1  
# Ex.Name: Write a C++ program to illustrate Employee Based Multiple inheritance with protected access specifier and find the income after the payment of tax.  
(Declare a base class to get salary amount, another base class to get tax amount, declare a derived class to call the functions from two base classes and perform calculation.)  

## Date:  

## Aim:  
To write a C++ program using multiple inheritance where one base class provides salary, another provides tax, and the derived class computes the net income after tax deduction.  

## Algorithm:  
1. Start the program.  
2. Define a base class `Salary` with a protected data member `salary` and a function to input salary.  
3. Define another base class `Tax` with a protected data member `tax` and a function to input tax amount.  
4. Define a derived class `Employee` which inherits from both `Salary` and `Tax`.  
5. In the derived class, write a function to calculate income as:  income = salary - tax
6. Display the calculated income.  
7. In the `main()` function, read salary and tax from the user.  
8. Call the input functions of the base classes and calculation function from the derived class. 
9. Stop the program.

## Program:
```cpp
#include <iostream>
using namespace std;

class num
{
    public:
    int a,b;
    void input(){
        cin>>a;
        cin>>b;
    }
    void display(){
        cout<<"Income after the payment of Tax : "<<a-b<<endl;
    }
};

int main()
{
    num r;
    r.input();
    r.display();
    
    return 0;
}

```

## Output:
<img width="851" height="446" alt="image" src="https://github.com/user-attachments/assets/dc35da25-7266-497f-8824-4d9bab9ca1bd" />

## Result:
```
Input:
275000
12500

Output:
Income after the payment of Tax : 262500
```
