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

## 2. C++ Protected Access Modifier in Classes

![Screenshot from 2022-07-24 12-23-27](https://user-images.githubusercontent.com/109052326/180636268-164c2cae-0072-4bbb-a3ce-45d5f9ce2414.png)
![Screenshot from 2022-07-24 12-25-32](https://user-images.githubusercontent.com/109052326/180636270-f998ae0d-06b6-4963-a17f-cfb6158a23fd.png)
![Screenshot from 2022-07-24 12-26-04](https://user-images.githubusercontent.com/109052326/180636271-d7334578-1e8c-4dff-b4e2-3ab8b5e2654f.png)
![Screenshot from 2022-07-24 12-26-05](https://user-images.githubusercontent.com/109052326/180636272-61abd3e1-9b7b-4227-95de-88faf52c470e.png)
![Screenshot from 2022-07-24 12-26-55](https://user-images.githubusercontent.com/109052326/180636273-f644b7da-28a3-4ff0-9a05-dfbdcffbff83.png)
![Screenshot from 2022-07-24 12-26-57](https://user-images.githubusercontent.com/109052326/180636274-f58a3a09-377b-4a89-8981-3295144b25b9.png)
![Screenshot from 2022-07-24 12-29-15](https://user-images.githubusercontent.com/109052326/180636275-c97c6ae0-6e49-497f-bd6b-b05285338503.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class Person
{
    
    protected:
        string name;
    public:
        void set_name(string iname)
        {
            name= iname;
        }
};


// Make a subclass/ child class / derived class
class student : public Person
{
    public:
    void introduce()
    {
        cout<<"Hie I am= "<<name<<endl;
    }
};

// Main function
int main()
{
    student anil;
    anil.set_name("Anil");
    anil.introduce();
    
    return 0;
}


```

## 3. C++ Access Control and Inheritance

![Screenshot from 2022-07-24 12-31-49](https://user-images.githubusercontent.com/109052326/180636404-c3a1210b-e1c9-4744-be83-b9814adba8a9.png)


## Code

```cpp
class A
{
public:
    int x;
protected:
    int y;
private:
    int z;
};
 
class B : public A
{
    // x is public
    // y is protected
    // z is not accessible from B
};
 
class C : protected A
{
    // x is protected
    // y is protected
    // z is not accessible from C
};
 
class D : private A    // 'private' is default for classes
{
    // x is private
    // y is private
    // z is not accessible from D
};

```

## 4. Public Inheritance in C++

## Code

```cpp

```
