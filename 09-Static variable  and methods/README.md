## 1. C++ Static Variables and Members in Class

![Screenshot from 2022-07-24 09-39-07](https://user-images.githubusercontent.com/109052326/180632093-8e813434-691d-449b-8110-87f9eef8e1ea.png)
![Screenshot from 2022-07-24 09-40-02](https://user-images.githubusercontent.com/109052326/180632096-ed2e867b-12ad-4196-9da6-c5faafa58c1b.png)
![Screenshot from 2022-07-24 09-40-03](https://user-images.githubusercontent.com/109052326/180632098-b7c7a849-bae4-4ca3-b875-ac79dec753ea.png)
![Screenshot from 2022-07-24 09-40-08](https://user-images.githubusercontent.com/109052326/180632101-dc5682b2-14ae-4cc4-a04f-c93612f6ef1a.png)
![Screenshot from 2022-07-24 09-40-12](https://user-images.githubusercontent.com/109052326/180632104-17ae1c51-37ca-4c26-a10a-18d1f31a7309.png)
![Screenshot from 2022-07-24 09-42-17](https://user-images.githubusercontent.com/109052326/180632107-260404c5-567f-4a3d-a4cf-fd7f78e91235.png)
![Screenshot from 2022-07-24 09-43-14](https://user-images.githubusercontent.com/109052326/180632110-8cc9e4f4-2557-419f-b889-e5c0cf782736.png)
![Screenshot from 2022-07-24 09-44-06](https://user-images.githubusercontent.com/109052326/180632111-d2555e44-4228-4263-8398-de3ddf8f806e.png)
![Screenshot from 2022-07-24 09-44-36](https://user-images.githubusercontent.com/109052326/180632115-a7270dd1-71f8-4f8a-bff3-889069b2acb4.png)
![Screenshot from 2022-07-24 09-44-49](https://user-images.githubusercontent.com/109052326/180632117-e6fa786f-75b4-48ff-b0ce-05d22430d1a4.png)
![Screenshot from 2022-07-24 09-44-51](https://user-images.githubusercontent.com/109052326/180632120-7615a23e-5c04-4149-885e-43910040748a.png)
![Screenshot from 2022-07-24 09-46-34](https://user-images.githubusercontent.com/109052326/180632122-2245c04b-3cdd-45d7-9d66-89d1cbe3783d.png)
![Screenshot from 2022-07-24 09-47-32](https://user-images.githubusercontent.com/109052326/180632125-2cc402a8-337d-4ee5-8ca3-5e6058dd4f9b.png)
![Screenshot from 2022-07-24 09-50-30](https://user-images.githubusercontent.com/109052326/180632127-806394c7-0e7b-4396-8b64-311010232cfa.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

void display()
{
    // Static counter value will be retained
    static int counter=0;
    cout<<"Display function called -> "<<++counter<<endl;
}

// Main function
int main()
{
   // Display function called these many no of times
   display();
   display();
   display();
   display();
   return 0;
}


```

```cpp
#include <bits/stdc++.h>
using namespace std;

class Human
{
    public:
        static int human_count;
        
    Human()
    {
        human_count++;
    }
    
    void total_count()
    {
        cout<<"There are -> "<<human_count<<" No of people in program"<<endl;
    }
};

int Human :: human_count =0;

// Main function
int main()
{
   cout<<Human:: human_count<<endl;;
   
   Human ajay;
   Human viajy;
   Human giri;
   
   ajay.total_count();
   cout<<Human:: human_count;
   
   return 0;
}


```

## 2. C++ Static Methods in Classes CPP Object Oriented Programming

![Screenshot from 2022-07-24 09-54-04](https://user-images.githubusercontent.com/109052326/180632315-93b91669-a866-4c35-bc6c-a158ac8916ca.png)
![Screenshot from 2022-07-24 09-54-06](https://user-images.githubusercontent.com/109052326/180632320-8b6fd2e6-7ed1-463c-91e1-78b8a9cedf94.png)
![Screenshot from 2022-07-24 09-59-43](https://user-images.githubusercontent.com/109052326/180632323-c9b59a86-7bd7-484a-9848-cda9d3f8f8fe.png)
![Screenshot from 2022-07-24 10-00-11](https://user-images.githubusercontent.com/109052326/180632327-73a43dd3-d41c-4ee5-bc8c-1f209616f28f.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Human
{
    public:
        static int human_count;
        
    Human()
    {
        human_count++;
    }
    
    // Static method creation
    static void total_count()
    {
        cout<<"There are -> "<<human_count<<" No of people in program"<<endl;
    }
};

int Human :: human_count =0;

// Main function
int main()
{
   // Creating the 3 objects for demo
   Human ajay;
   Human viajy;
   Human giri;
   
   // Calling the static method
   Human:: total_count();
   
   return 0;
}


```

## 3. Friend Function

![Screenshot from 2022-07-24 10-05-15](https://user-images.githubusercontent.com/109052326/180632584-9e6cd4f3-4068-4513-964d-a3865ee00e5c.png)
![Screenshot from 2022-07-24 10-08-11](https://user-images.githubusercontent.com/109052326/180632591-d7c543ac-4c2f-4c5d-932c-e3036cea2bfe.png)
![Screenshot from 2022-07-24 10-09-50](https://user-images.githubusercontent.com/109052326/180632593-f82097ea-a8b7-4bb0-a7aa-216a9ab2d63e.png)
![Screenshot from 2022-07-24 10-10-07](https://user-images.githubusercontent.com/109052326/180632597-6c25d08d-63ee-464d-a559-7a3c6d3ff939.png)
![Screenshot from 2022-07-24 10-14-48](https://user-images.githubusercontent.com/109052326/180632602-41136ba0-5253-42df-a876-8804426fbf72.png)
![Screenshot from 2022-07-24 10-14-58](https://user-images.githubusercontent.com/109052326/180632603-6ab67ea2-a362-48dc-bc23-8a434a448ce6.png)
![Screenshot from 2022-07-24 10-15-01](https://user-images.githubusercontent.com/109052326/180632604-769cf16b-0203-4646-a43e-1a451e6e794a.png)
![Screenshot from 2022-07-24 10-15-35](https://user-images.githubusercontent.com/109052326/180632606-fba98d37-a4d4-44e1-bf9c-b01ba107576d.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a class
class Human
{
   // Private member variables
   int age;
   string name;
   
   // Public 
public:

    // Make a constructor and assign the values
    Human(string iname, int iage)
    {
        name= iname;
        age= iage;
    }
    
    // Make a method tellme
    void tellme()
    {
        cout<<name<<endl;
        cout<<age<<endl;
    }
   
// Make a friend function 
friend void display(Human h);

};

// Make a display method and pass object 
void display(Human man)
{
    cout<<man.name<<endl;
    cout<<man.age<<endl;
    
}

// Main function
int main()
{
  Human ajay("Ajay",24);
  display(ajay);
   return 0;
}


```
