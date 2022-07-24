## 1. Class Constructors in object oriented Programming

![Screenshot from 2022-07-24 08-05-11](https://user-images.githubusercontent.com/109052326/180629924-97cef7c9-2cb3-436f-b615-789e783d30d6.png)
![Screenshot from 2022-07-24 08-06-10](https://user-images.githubusercontent.com/109052326/180629925-62a7f300-0880-4421-b685-9bf7717b4ebe.png)
![Screenshot from 2022-07-24 08-06-18](https://user-images.githubusercontent.com/109052326/180629928-a005717f-ee73-4679-b736-6375c4214182.png)
![Screenshot from 2022-07-24 08-07-45](https://user-images.githubusercontent.com/109052326/180629929-6965ab1a-457e-4bb1-a215-d48609ef618d.png)
![Screenshot from 2022-07-24 08-08-41](https://user-images.githubusercontent.com/109052326/180629930-54ab8e24-e770-450a-92b8-8ef43934ad73.png)
![Screenshot from 2022-07-24 08-08-56](https://user-images.githubusercontent.com/109052326/180629931-c20db1cc-d535-4e52-b950-85b737a379e1.png)
![Screenshot from 2022-07-24 08-10-30](https://user-images.githubusercontent.com/109052326/180629933-5e1862ad-7bad-4b4a-a13e-6e06418d9e5e.png)
![Screenshot from 2022-07-24 08-10-40](https://user-images.githubusercontent.com/109052326/180629934-162988d8-b0fd-44b6-a4d9-2f286bf06727.png)
![Screenshot from 2022-07-24 08-10-45](https://user-images.githubusercontent.com/109052326/180629935-6702a08e-5871-41a3-9a62-8dc57ba1d77a.png)
![Screenshot from 2022-07-24 08-11-34](https://user-images.githubusercontent.com/109052326/180629937-aa2944dc-0379-44b9-af59-0a7874c20e6e.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{   
    // Declare the private member variables
    string name;
    int age;

public:
    
    // Call the default constructor manually
    Human()
    {
        name= "Ajay";
        age=25;
    }
    
    // Display meethod
    void display()
    {
        cout<<name<<" "<<age<<endl;
    }
};

// Main function
int main()
{
   Human anil;
   anil.display();
   return 0;
}


```

## 2. Overloading Class Constructors

![Screenshot from 2022-07-24 08-14-45](https://user-images.githubusercontent.com/109052326/180630240-47913a39-adf9-4959-a77d-ff2f467eb1dd.png)
![Screenshot from 2022-07-24 08-15-26](https://user-images.githubusercontent.com/109052326/180630244-1f3a2750-b72a-48d1-bbe7-2f303d9ff480.png)
![Screenshot from 2022-07-24 08-16-20](https://user-images.githubusercontent.com/109052326/180630245-2c7b30e8-f306-4387-b0d0-ce37ea0ad381.png)
![Screenshot from 2022-07-24 08-19-09](https://user-images.githubusercontent.com/109052326/180630247-5d59bbf5-941d-4dd2-a87c-b86d783ced0f.png)
![Screenshot from 2022-07-24 08-25-16](https://user-images.githubusercontent.com/109052326/180630248-b10e8b07-6277-4dac-87c7-875c23d616d0.png)
![Screenshot from 2022-07-24 08-25-31](https://user-images.githubusercontent.com/109052326/180630250-b1e736aa-80de-481b-8f9d-11a3923bab5c.png)
![Screenshot from 2022-07-24 08-25-53](https://user-images.githubusercontent.com/109052326/180630252-cbc76033-e55d-45c0-863b-a72c4ddcd8a1.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{   
    // Declare the private member variables
    string name;
    int age;

public:
    
    // Call the default constructor manually
    Human()
    {
        name= "Ajay";
        age=25;
    }
    
    Human(string iname)
    {
        cout<<"Constructor with name as params"<<endl;
        age=0;
        name= iname;
    }
    
    Human(int iage)
    {
        cout<<"Constructor with age as params"<<endl;
        age=iage;
        name= "no_name";
    }
    
    Human(string s, int iage)
    {
        cout<<"Constructor with name & age as params"<<endl;
        age=iage;
        name= s;
    }
    
    // Display meethod
    void display()
    {
        cout<<name<<" "<<age<<endl;
    }
};

// Main function
int main()
{
   Human anil("Ajay");
   anil.display();
   return 0;
}


```

## 3. Default Class Constructor Parameters

![Screenshot from 2022-07-24 08-27-47](https://user-images.githubusercontent.com/109052326/180630385-8d4cf160-de08-448c-8bef-8f867188b24e.png)
![Screenshot from 2022-07-24 08-29-26](https://user-images.githubusercontent.com/109052326/180630387-4611377b-b6bb-4fb8-a066-d06fd7503033.png)
![Screenshot from 2022-07-24 08-30-02](https://user-images.githubusercontent.com/109052326/180630388-5c408ae1-757f-4226-afbd-127362100de1.png)
![Screenshot from 2022-07-24 08-31-36](https://user-images.githubusercontent.com/109052326/180630389-997879af-5a0c-4ca6-b409-719c68f40973.png)
![Screenshot from 2022-07-24 08-31-51](https://user-images.githubusercontent.com/109052326/180630391-11a1a21a-560a-492a-8f4f-43675cefcb4f.png)
![Screenshot from 2022-07-24 08-32-07](https://user-images.githubusercontent.com/109052326/180630393-09110a74-b10d-4a92-8478-bbad4512f8c4.png)
![Screenshot from 2022-07-24 08-32-11](https://user-images.githubusercontent.com/109052326/180630394-ab3ec581-5a44-4df1-a80d-66f6784dc998.png)
![Screenshot from 2022-07-24 08-32-22](https://user-images.githubusercontent.com/109052326/180630395-4a3c9601-1653-416d-a6bc-76cf8d2185f9.png)
![Screenshot from 2022-07-24 08-32-33](https://user-images.githubusercontent.com/109052326/180630396-265e0d00-1665-4936-8b89-a1b314813700.png)
![Screenshot from 2022-07-24 08-32-40](https://user-images.githubusercontent.com/109052326/180630399-8b6c61aa-36bc-40e0-b7d2-37681adca354.png)
![Screenshot from 2022-07-24 08-33-37](https://user-images.githubusercontent.com/109052326/180630401-9c7aff12-05e4-47a9-9f8e-881a30cdaf21.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{   
    // Declare the private member variables
    string name;
    int age;

public:
    
    // Call the default constructor manually
    Human()
    {
        name= "Ajay";
        age=25;
    }
    
    // Constructor with default values if not pass while obj creation
    Human(string s, int iage=0)
    {
        cout<<"Constructor with name & age as params"<<endl;
        age=iage;
        name= s;
    }
    
    // Display meethod
    void display()
    {
        cout<<name<<" "<<age<<endl;
    }
};

// Main function
int main()
{
   Human anil("Ajay",5555);
   anil.display();
   return 0;
}

```

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{   
    // Declare the private member variables
    string name;
    int age;

public:
    
    // Constructor with default values if not pass while obj creation
    Human(string s="no_name", int iage=0)
    {
        cout<<"Constructor with name & age as params"<<endl;
        age=iage;
        name= s;
    }
    
    // Display method
    void display()
    {
        cout<<name<<" "<<age<<endl;
    }
};

// Main function
int main()
{
   Human anil;
   anil.display();
   return 0;
}


```

## 4. Destructors in a Class

![Screenshot from 2022-07-24 08-34-50](https://user-images.githubusercontent.com/109052326/180630563-c4c95598-3a40-4fcf-8e97-4bdabed6e4b4.png)
![Screenshot from 2022-07-24 08-36-32](https://user-images.githubusercontent.com/109052326/180630566-70320094-a3c3-4196-a85a-f8a4e9ff2c23.png)
![Screenshot from 2022-07-24 08-36-56](https://user-images.githubusercontent.com/109052326/180630568-1d509f94-ff42-4013-82b1-0a649c3b55c2.png)
![Screenshot from 2022-07-24 08-37-09](https://user-images.githubusercontent.com/109052326/180630570-74c7a051-4412-4d30-9da6-f9e4327bde6c.png)
![Screenshot from 2022-07-24 08-37-11](https://user-images.githubusercontent.com/109052326/180630571-ac19ecb1-c656-491e-bcc8-610081f9d3ad.png)
![Screenshot from 2022-07-24 08-38-45](https://user-images.githubusercontent.com/109052326/180630572-c7a8334c-2d33-4624-b4da-40ecf5da1423.png)
![Screenshot from 2022-07-24 08-39-20](https://user-images.githubusercontent.com/109052326/180630573-e3a15999-e1bc-4a61-8395-d343a8151b45.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{   
    
public:
    
    // Constructor called while object creation
    Human()
    {
        cout<<"Constructor called"<<endl;
    }
    
    // Descructor called while object is deleted from memory
    ~Human()
    {
        cout<<"Descructor called"<<endl;
    }
    
    
};

// Main function
int main()
{
   Human *anil = new Human();
   delete anil;
   return 0;
}


```
