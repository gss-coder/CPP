## 1. Inheritance, Poly Morphism - Introduction

![Screenshot from 2022-07-24 11-53-19](https://user-images.githubusercontent.com/109052326/180635948-f3d37726-4181-4e42-bc24-435f642160d9.png)
![Screenshot from 2022-07-24 11-54-16](https://user-images.githubusercontent.com/109052326/180635950-8cf3d368-4bbe-4148-b66a-7ffce00d2745.png)
![Screenshot from 2022-07-24 12-14-44](https://user-images.githubusercontent.com/109052326/180635952-9ba21f44-9473-4651-baaa-137111310a66.png)
![Screenshot from 2022-07-24 12-16-23](https://user-images.githubusercontent.com/109052326/180635953-e669bc0c-c32f-4fd8-8d38-4c726e09e42a.png)
![Screenshot from 2022-07-24 12-18-04](https://user-images.githubusercontent.com/109052326/180635956-61193ba8-62bc-4ece-8bcf-faca965bb17b.png)
![Screenshot from 2022-07-24 12-18-36](https://user-images.githubusercontent.com/109052326/180635958-bc628f46-9db0-4481-940f-364f1ab01c18.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class Person
{
    
public:

    string name;
    int age;
    
    void set_name(string iname)
    {
        name= iname;
    }
    
    void set_age(int iage)
    {
        age= iage;
    }
    
};


// Make a subclass/ child class / derived class
class student : public Person
{
    public:
        
        int id;
        
        void set_id(int iid)
        {
            id= iid;
        }
        
        void introduce()
        {
            cout<<"Hie I am= "<<name<<endl<<"And My age is= "<<age<<endl<<"Student id= "<<id<<endl;
        }
};

// Main function
int main()
{
    student anil;
    
    anil.set_age(25);
    anil.set_name("Ajay");
    anil.set_id(12345);
    anil.introduce();
    
    return 0;
}


```
