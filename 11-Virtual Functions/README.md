## 1. Polymorphism in C++ and Virtual Functions / Methods

![Screenshot from 2022-07-24 20-42-01](https://user-images.githubusercontent.com/109052326/180654059-76d61a26-55a4-4cff-9516-1112134a2e2b.png)
![Screenshot from 2022-07-24 20-43-03](https://user-images.githubusercontent.com/109052326/180654061-418bcb16-20a0-49ac-aff9-151f5279a2d5.png)
![Screenshot from 2022-07-24 20-44-20](https://user-images.githubusercontent.com/109052326/180654062-e4025c83-62a4-42e9-ba4e-c0d8d5137de4.png)
![Screenshot from 2022-07-24 20-44-37](https://user-images.githubusercontent.com/109052326/180654064-3ad2c843-63e3-402c-b971-bd52e663c46d.png)
![Screenshot from 2022-07-24 20-46-13](https://user-images.githubusercontent.com/109052326/180654067-a4600fb8-ce9a-4124-8545-f1a8f5f2af37.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Person
{
    public:
    
    // Using the virtual keyword for polymorphism
    virtual void introduce()
    {
        cout<<"Hey from person"<<endl;
    }
                
};

class Student : public Person
{
    public:
    
    void introduce()
    {
        cout<<"Hey from student"<<endl;
    }
};

class farmer : public Person
{
    public:
    
    void introduce()
    {
        cout<<"Hey from farmer"<<endl;
    }   
        
};

void whos_this(Person &p)
{
    p.introduce();
}

// Main function
int main()
{
    //Student anil;
    farmer farm;
    whos_this(farm);
    return 0;
}


```

## 2. C++ Virtual Function / Inherited Attributes, Hierarchical Nature

![Screenshot from 2022-07-24 20-52-52](https://user-images.githubusercontent.com/109052326/180654454-b40bc20b-2ac0-4a0a-92ca-b21bb13876e0.png)
![Screenshot from 2022-07-24 20-54-31](https://user-images.githubusercontent.com/109052326/180654455-695d030a-5c05-4392-acc6-b46a04aae0fe.png)
![Screenshot from 2022-07-24 20-55-33](https://user-images.githubusercontent.com/109052326/180654458-dcd1cf48-2ff6-4635-b6cc-ca2477455a36.png)
![Screenshot from 2022-07-24 20-56-08](https://user-images.githubusercontent.com/109052326/180654463-b98dc535-a4c5-47dc-ad8f-8cad7d4501a7.png)
![Screenshot from 2022-07-24 20-59-27](https://user-images.githubusercontent.com/109052326/180654465-dd02f586-4530-40d0-9571-190a98bfeeb3.png)
![Screenshot from 2022-07-24 21-00-54](https://user-images.githubusercontent.com/109052326/180654467-abe8180e-066d-4948-838e-98da678adf80.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Person
{
    public:
    
    // Using the virtual keyword for polymorphism
    virtual void introduce()
    {
        cout<<"Hey from person"<<endl;
    }
                
};

class Student : public Person
{
    public:
    
    void introduce()
    {
        cout<<"Hey from student"<<endl;
    }
};

class gstudent : public Student
{
    public:
    
    void introduce()
    {
        cout<<"Hey from gstudent"<<endl;
    }   
};

void whos_this(Person &p)
{
    p.introduce();
}

// Main function
int main()
{
    
    Person anil;
    Student anjali;
    gstudent ajay;
    
    whos_this(anil);
    whos_this(anjali);
    whos_this(ajay);
    
    return 0;
}


```

## 3. C++ Pure Virtual Functions, Abstract Classes

![Screenshot from 2022-07-24 21-02-30](https://user-images.githubusercontent.com/109052326/180655046-d76a672b-3dd1-4f79-be13-137789979fa1.png)
![Screenshot from 2022-07-24 21-06-13](https://user-images.githubusercontent.com/109052326/180655050-4d2418df-d373-48e4-a91a-3d53f80c8f68.png)
![Screenshot from 2022-07-24 21-06-40](https://user-images.githubusercontent.com/109052326/180655056-fff67774-3d59-4b9d-956a-eb7ac28ef9bc.png)
![Screenshot from 2022-07-24 21-06-58](https://user-images.githubusercontent.com/109052326/180655059-f1d4f521-07a5-47dd-b637-74cdfe2090b8.png)
![Screenshot from 2022-07-24 21-07-00](https://user-images.githubusercontent.com/109052326/180655060-b35674a6-f5b5-4937-938a-b74c3739c02c.png)
![Screenshot from 2022-07-24 21-07-31](https://user-images.githubusercontent.com/109052326/180655062-2b6f4f27-b07b-4dc9-b35a-49481498f17f.png)
![Screenshot from 2022-07-24 21-07-33](https://user-images.githubusercontent.com/109052326/180655064-f94ed1a4-5acf-4c1e-b062-51660bf6c6b4.png)
![Screenshot from 2022-07-24 21-07-44](https://user-images.githubusercontent.com/109052326/180655065-bdcc25b9-cde5-4ce6-b89f-6bc50fbcf275.png)
![Screenshot from 2022-07-24 21-07-45](https://user-images.githubusercontent.com/109052326/180655069-2713fba7-67ba-4f21-bc5b-7a08f350dbd3.png)
![Screenshot from 2022-07-24 21-07-56](https://user-images.githubusercontent.com/109052326/180655070-e85177f6-90e2-439f-adfc-60d644fb001f.png)
![Screenshot from 2022-07-24 21-08-22](https://user-images.githubusercontent.com/109052326/180655071-db0635e9-2565-4813-b8fb-275e8c54d996.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Person
{
    public:
    
    virtual void introduce()=0;
                
};

void Person :: introduce()
{
    cout<<"Hey from the person..."<<endl;
}

class Student : public Person
{
    public:
    
    void introduce()
    {
        cout<<"Hey from student"<<endl;
    }
};


// Main function
int main()
{
    Student anjali;
    anjali.introduce();
    return 0;
}


```

## 4. C++ Diamond problem in OOPS, Solution using Virtual Inheritance with Example

![Screenshot from 2022-07-24 21-13-39](https://user-images.githubusercontent.com/109052326/180655595-6c82a7d2-aca4-487c-9202-bc982771c9d9.png)
![Screenshot from 2022-07-24 21-14-24](https://user-images.githubusercontent.com/109052326/180655601-a2c300d4-26c7-4ab3-882a-3c059815fe34.png)
![Screenshot from 2022-07-24 21-14-54](https://user-images.githubusercontent.com/109052326/180655602-27a0fe16-8b43-46d4-b0fc-31eaad43e4a0.png)
![Screenshot from 2022-07-24 21-14-56](https://user-images.githubusercontent.com/109052326/180655604-43c7fa8b-4818-4b74-9ed9-a1741e64be6c.png)
![Screenshot from 2022-07-24 21-15-39](https://user-images.githubusercontent.com/109052326/180655605-f1fe2df5-9542-4197-8ade-f1d4cc166e61.png)
![Screenshot from 2022-07-24 21-15-54](https://user-images.githubusercontent.com/109052326/180655607-6e0e912a-9e06-41be-a30e-3aa41c3fa17a.png)
![Screenshot from 2022-07-24 21-18-34](https://user-images.githubusercontent.com/109052326/180655610-6cd071ae-77f4-421d-a29f-b74183f5c97a.png)
![Screenshot from 2022-07-24 21-20-36](https://user-images.githubusercontent.com/109052326/180655613-5a12bfe9-b197-421d-9924-af3882ff538a.png)
![Screenshot from 2022-07-24 21-20-44](https://user-images.githubusercontent.com/109052326/180655614-ef623133-71c9-4e41-bbc3-5ebb150c3131.png)
![Screenshot from 2022-07-24 21-21-36](https://user-images.githubusercontent.com/109052326/180655616-787c5701-7288-455c-b434-dad72563e977.png)
![Screenshot from 2022-07-24 21-21-52](https://user-images.githubusercontent.com/109052326/180655618-3fee7a9f-de93-4012-9fe4-a31fb6cee67a.png)
![Screenshot from 2022-07-24 21-22-24](https://user-images.githubusercontent.com/109052326/180655620-ed75a6a4-27ae-455f-aa6a-afbc6aad2fef.png)
![Screenshot from 2022-07-24 21-23-24](https://user-images.githubusercontent.com/109052326/180655623-5fef5d27-9751-411d-9e80-b2300094ef62.png)
![Screenshot from 2022-07-24 21-23-31](https://user-images.githubusercontent.com/109052326/180655624-176b157c-f1c4-4361-b67c-7bcfde859466.png)
![Screenshot from 2022-07-24 21-23-34](https://user-images.githubusercontent.com/109052326/180655626-9c3f3262-97fa-4ade-8bc3-d35258d4e83c.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Animal
{
    public:
        int age;
        
        void walk()
        {
            cout<<" Animal Walks..."<<endl;
        }
        
};

class Tiger : virtual public Animal
{
    
};

class Lion : virtual public Animal
{
    
};

class Liger : public Tiger ,public Lion
{
  
};

// Main function
int main()
{
    Liger l;
    l.walk();
   
    return 0;
}


```
