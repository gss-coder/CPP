## 1. Inheritance, Poly Morphism - Introduction

![Screenshot from 2022-07-24 10-05-15](https://user-images.githubusercontent.com/109052326/180635936-f3f3460c-73df-456b-bbea-807ad1d79fe6.png)
![Screenshot from 2022-07-24 10-08-11](https://user-images.githubusercontent.com/109052326/180635939-744c1173-1b71-4293-88a1-993f73aabbd8.png)
![Screenshot from 2022-07-24 10-09-50](https://user-images.githubusercontent.com/109052326/180635940-d8c24dbe-184c-40f0-a951-0b6470874ddc.png)
![Screenshot from 2022-07-24 10-10-07](https://user-images.githubusercontent.com/109052326/180635941-6923e0c0-6dce-4976-b8ad-aa22ea6298ca.png)
![Screenshot from 2022-07-24 10-14-48](https://user-images.githubusercontent.com/109052326/180635942-78d4eeaf-3d9e-4e6d-a74d-ab6f5622e242.png)
![Screenshot from 2022-07-24 10-14-58](https://user-images.githubusercontent.com/109052326/180635944-1a64bfa4-00ab-4faf-8ed2-6e1702d561e0.png)
![Screenshot from 2022-07-24 10-15-01](https://user-images.githubusercontent.com/109052326/180635946-3359a26b-1ba6-4b54-a2c4-bf3ee5f7dfbc.png)
![Screenshot from 2022-07-24 10-15-35](https://user-images.githubusercontent.com/109052326/180635947-1a3eca89-1685-4214-b4b2-98e1104a458c.png)
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
