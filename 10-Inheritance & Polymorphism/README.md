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

![Screenshot from 2022-07-24 15-07-29](https://user-images.githubusercontent.com/109052326/180642276-4671ebcb-f0ee-467e-9a32-dd63b54f2d5c.png)
![Screenshot from 2022-07-24 15-09-33](https://user-images.githubusercontent.com/109052326/180642279-1c5c5dc2-b7f0-4b37-9b73-55c339e36b66.png)
![Screenshot from 2022-07-24 15-39-24](https://user-images.githubusercontent.com/109052326/180642282-144d2e6e-3196-4d7a-b0be-e339e94fe20d.png)


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

## 5. Protected Inheritance in C++

![Screenshot from 2022-07-24 15-42-01](https://user-images.githubusercontent.com/109052326/180642542-d89fd104-1668-4da1-942f-5bc48154f11e.png)
![Screenshot from 2022-07-24 15-42-07](https://user-images.githubusercontent.com/109052326/180642546-de2348b3-2804-426e-8448-748e10785178.png)
![Screenshot from 2022-07-24 15-42-12](https://user-images.githubusercontent.com/109052326/180642548-2b08fd9d-6a88-4aff-a6a8-16600a159695.png)
![Screenshot from 2022-07-24 15-42-40](https://user-images.githubusercontent.com/109052326/180642550-40db5534-b8d8-4091-8ea5-5f103019574f.png)


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
class student : protected Person
{
    public:
    
    void introduce()
    {
        cout<<"Hie I am= "<<name<<endl;
    }
    
    void set_student_name(string iname)
    {
        set_name(iname);
    }
};

// Main function
int main()
{
    student anil;
    anil.set_student_name("Anil");
    anil.introduce();
    
    return 0;
}

```

## 6. Private Inheritance in C++

![Screenshot from 2022-07-24 15-46-43](https://user-images.githubusercontent.com/109052326/180642919-41c36049-6a99-4e45-9e49-ebbe90f736ca.png)
![Screenshot from 2022-07-24 15-47-27](https://user-images.githubusercontent.com/109052326/180642922-8f6945f6-0ea9-4dad-9441-a987f0d88581.png)
![Screenshot from 2022-07-24 15-48-26](https://user-images.githubusercontent.com/109052326/180642923-ebc38ecc-0ca8-4aaa-9c98-80924f8e2ff5.png)
![Screenshot from 2022-07-24 15-48-29](https://user-images.githubusercontent.com/109052326/180642924-a2a13b19-4f7b-4972-a4b7-12437fbc53cb.png)


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
class student : private Person
{
    public:
     
    void introduce()
    {
        cout<<"Hie I am= "<<name<<endl;
    }
    
    void set_student_name(string iname)
    {
        set_name(iname);
    }
};

class g_student : public student
{
    public:
        void set_g_student_name(string iname)
        {
            set_student_name(iname);
            
        }
};

// Main function
int main()
{
    g_student anil;
    anil.set_student_name("Anil");
    anil.introduce();
    
    return 0;
}


```

## 7. Changing Access Level of Base Class Members

![Screenshot from 2022-07-24 15-57-18](https://user-images.githubusercontent.com/109052326/180643141-bfcf550a-f576-4278-8917-c81dfedbfb81.png)
![Screenshot from 2022-07-24 15-58-48](https://user-images.githubusercontent.com/109052326/180643143-227f850c-0c51-4fb5-9d68-4767c1798619.png)
![Screenshot from 2022-07-24 15-58-53](https://user-images.githubusercontent.com/109052326/180643144-eb93f891-d89a-4134-af05-aa22e02b3358.png)


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
class student : private Person
{
    public:
    
    // Changing the access level 
    using Person :: name;
    using Person :: set_name;
    
    
    void introduce()
    {
        cout<<"Hie I am= "<<name<<endl;
    }
    
    void set_student_name(string iname)
    {
        set_name(iname);
    }
};

class g_student : public student
{
    public:
        void set_g_student_name(string iname)
        {
            set_student_name(iname);
            
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

## 8. Order of Execution of Constructors and Destructors in Inheritance

![Screenshot from 2022-07-24 16-03-38](https://user-images.githubusercontent.com/109052326/180643380-b76fd3f5-36f5-4b72-aa3c-cb690ad836e4.png)
![Screenshot from 2022-07-24 16-07-08](https://user-images.githubusercontent.com/109052326/180643381-0faf99df-16eb-4dee-8074-17c2bf5f6fcb.png)
![Screenshot from 2022-07-24 16-07-14](https://user-images.githubusercontent.com/109052326/180643382-c43d6d7f-db15-4977-af01-744cb122e34e.png)
![Screenshot from 2022-07-24 16-07-37](https://user-images.githubusercontent.com/109052326/180643383-b0896e4f-c140-479d-bbc1-921867e721ca.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class Person
{
    public:
    
        Person()
        {
            cout<<"Const of person class called"<<endl;
        }
        
        ~Person()
        {
            cout<<"Desctructor of person class called"<<endl;
        }
};


// Make a subclass/ child class / derived class
class student : public Person
{
     public:
    
        student()
        {
            cout<<"Const of student class called"<<endl;
        }
        
        ~student()
        {
            cout<<"Desctructor of student class called"<<endl;
        }
};

// Main function
int main()
{
    student anil;
 
    return 0;
}


```

## 9. C++ Multiple Inheritance Explained

![Screenshot from 2022-07-24 16-11-50](https://user-images.githubusercontent.com/109052326/180643812-68e61615-e5a9-4843-8745-b563d2ec9f01.png)
![Screenshot from 2022-07-24 16-12-34](https://user-images.githubusercontent.com/109052326/180643814-17e4c7d6-344b-4fac-bd26-114a96e6f9f4.png)
![Screenshot from 2022-07-24 16-19-46](https://user-images.githubusercontent.com/109052326/180643818-98d1923a-1491-4599-a6cd-5b8b5d4e62bd.png)
![Screenshot from 2022-07-24 16-20-12](https://user-images.githubusercontent.com/109052326/180643823-fdfd6628-b15e-4a66-9479-1654f1642405.png)
![Screenshot from 2022-07-24 16-20-14](https://user-images.githubusercontent.com/109052326/180643827-bd277e7c-8c06-4548-9160-7081a6447612.png)
![Screenshot from 2022-07-24 16-22-27](https://user-images.githubusercontent.com/109052326/180643828-e1634cc4-6c71-41ce-bea6-cf72736ef581.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class father
{
    public:
        int height;
        
        void askfather()
        {
            cout<<"I am ur father ask me"<<endl;
        }
};

// Make a base class
class Mother
{
    public:
        string skincolor;
        
        void askmother()
        {
            cout<<"I am ur mother ask me"<<endl;
        }
};

// Make a subclass/ child class / derived class
class child : public father , public  Mother
{
    public:
    
    void askparents()
    {
        cout<<"I am asking my parent's"<<endl;
    }
    
    void set_color_and_height(string icolor, int iheight)
    {
        skincolor = icolor;
        height = iheight;
    }
    
    void display()
    {
        cout<<"Height -> "<<height<<"Color -> "<<skincolor<<endl;
    }
};


// Main function
int main()
{
    child anil;
    anil.set_color_and_height("White", 6);
    anil.display();
    anil.askfather();
    anil.askmother();
    
 
    return 0;
}


```

## 10. C++ Calling and Passing Values to Base Class Constructor in Derived Class

![Screenshot from 2022-07-24 16-24-12](https://user-images.githubusercontent.com/109052326/180646284-b9e1c1aa-f0a9-4c74-9fca-19be85ad97aa.png)
![Screenshot from 2022-07-24 16-24-14](https://user-images.githubusercontent.com/109052326/180646287-d80a3560-9367-4354-9904-e8b1900f4fbe.png)
![Screenshot from 2022-07-24 16-25-53](https://user-images.githubusercontent.com/109052326/180646288-a88c0fe5-395d-424e-af18-5fa0ebbc24e6.png)
![Screenshot from 2022-07-24 16-25-58](https://user-images.githubusercontent.com/109052326/180646289-5f0f2369-3ed3-49d8-8959-e56597b84aa6.png)
![Screenshot from 2022-07-24 16-31-51](https://user-images.githubusercontent.com/109052326/180646291-b46dd1e2-dea2-4c17-9b7b-5232c7efabfb.png)
![Screenshot from 2022-07-24 16-32-11](https://user-images.githubusercontent.com/109052326/180646292-849a13dc-2c0b-4d57-8f65-f4d362542884.png)
![Screenshot from 2022-07-24 16-32-17](https://user-images.githubusercontent.com/109052326/180646295-35068982-3cf1-487e-a83f-56c52c324bce.png)
![Screenshot from 2022-07-24 16-32-22](https://user-images.githubusercontent.com/109052326/180646296-fe73dcbd-4333-41e4-9e70-3900c5bfdd61.png)
![Screenshot from 2022-07-24 16-32-34](https://user-images.githubusercontent.com/109052326/180646297-b364b426-76b1-4330-9f41-2f1d0ee0849e.png)
![Screenshot from 2022-07-24 16-33-59](https://user-images.githubusercontent.com/109052326/180646298-d3510af6-ce5d-46df-9219-8696a52368c2.png)
![Screenshot from 2022-07-24 17-38-32](https://user-images.githubusercontent.com/109052326/180646299-cb39f9e3-d1dd-4a03-a013-5d8ddc904c1f.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class father
{
    public:
        int height;
        
        father(int h)
        {
            cout<<"Constructor of the father is called.."<<endl;
            height = h;
        }
};


// Make a subclass/ child class / derived class
class child : public father 
{
    public:
    child(int x) : father(x)
    {
        cout<<"Child class construcutor.. "<<endl;
    }
    
    void display()
    {
        cout<<"Height is= "<<height<<endl;
    }
    
};


// Main function
int main()
{
    child anil(244);
    anil.display();
    return 0;
}
```

```cpp

#include <bits/stdc++.h>
using namespace std;

// Make a Base class
class father
{
    public:
        int height;
        
        father()
        {
            cout<<"Const of the father is called.."<<endl;
        }
};

class mother
{
    protected:
        string skincolor;
        
    public:
    
        mother()
        {
            cout<<"Const of the mother class"<<endl;
        }
};

// Make a subclass/ child class / derived class
class child : public father , public mother
{
    public:
    child(int x,string sk) : father() , mother()
    {
        height = x;
        skincolor = sk;
        cout<<"Child class construcutor.. "<<endl;
    }
    
    void display()
    {
        cout<<"Height is= "<<height<<endl;
        cout<<"Skin color is= "<<skincolor<<endl;
    }
    
};


// Main function
int main()
{
    child anil(244,"White");
    anil.display();
    return 0;
}

```
