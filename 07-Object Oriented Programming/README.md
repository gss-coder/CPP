## 1. C++ Object Oriented Programming Introduction

![Screenshot from 2022-07-23 20-13-10](https://user-images.githubusercontent.com/109052326/180610551-893f1b25-983d-4ee2-bf4f-62a5124c0d2f.png)
![Screenshot from 2022-07-23 20-13-54](https://user-images.githubusercontent.com/109052326/180610555-28e3cd87-97bc-44c0-b00d-2cf3d9bb304d.png)
![Screenshot from 2022-07-23 20-24-21](https://user-images.githubusercontent.com/109052326/180610557-6d9f6831-8087-4c53-8161-078e6d680724.png)
![Screenshot from 2022-07-23 20-25-11](https://user-images.githubusercontent.com/109052326/180610559-a682cee3-252d-424c-8c85-501c3c28747f.png)
![Screenshot from 2022-07-23 20-25-13](https://user-images.githubusercontent.com/109052326/180610560-1c795313-44ff-4ac9-9474-1b42c778c213.png)
![Screenshot from 2022-07-23 20-26-55](https://user-images.githubusercontent.com/109052326/180610562-0424b8af-0a76-45b8-a020-1d0dcd702a41.png)
![Screenshot from 2022-07-23 20-28-43](https://user-images.githubusercontent.com/109052326/180610563-f47be2b7-0c59-4a17-92a4-ede0053b57f7.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

class Human
{
    public:
        void display()
        {
            cout<<"I am from class Human"<<endl;
        }
};

// Main function
int main()
{
   Human h;
   h.display();
   return 0;
}


```

## 2. Class Properties, Methods, Members

![Screenshot from 2022-07-23 20-30-34](https://user-images.githubusercontent.com/109052326/180610861-8020b23c-0c2a-4253-99c2-634fb4d05a96.png)
![Screenshot from 2022-07-23 20-32-18](https://user-images.githubusercontent.com/109052326/180610864-a61fc1a6-0fef-47db-bd2d-12eedd69ac56.png)
![Screenshot from 2022-07-23 20-32-30](https://user-images.githubusercontent.com/109052326/180610866-31e31354-b516-4394-b345-06953a1a681e.png)

## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{
    public:
        // Make a new variable
        string name;
        
        // Make the introduce method
        void introduce()
        {
            cout<<"Hie I am -> "<<name<<endl;
        }
};

// Main function
int main()
{
   // Create the new object of the clas
   Human ajay;
   
   // Assign the values to the class
   ajay.name= "Ajay";
   
   // Call the class method
   ajay.introduce();
   return 0;
}


```

## 3. Creating Objects from a Class in Different Ways in object oriented

![Screenshot from 2022-07-23 20-43-38](https://user-images.githubusercontent.com/109052326/180611353-ec570626-f210-4618-b53a-e48edcae9366.png)
![Screenshot from 2022-07-23 20-46-37](https://user-images.githubusercontent.com/109052326/180611355-1bfc846b-3202-4ba6-abe7-5c27f6395ca8.png)
![Screenshot from 2022-07-23 20-47-33](https://user-images.githubusercontent.com/109052326/180611356-e04c75c0-342a-48a0-a029-3e1af37586d7.png)
![Screenshot from 2022-07-23 20-47-35](https://user-images.githubusercontent.com/109052326/180611358-063b0bf4-a66b-46ef-a079-0bd8830511a6.png)
![Screenshot from 2022-07-23 20-48-52](https://user-images.githubusercontent.com/109052326/180611360-65194818-441d-4af3-90c4-5e943985cedd.png)
![Screenshot from 2022-07-23 20-48-54](https://user-images.githubusercontent.com/109052326/180611364-1a2b1c40-0cf3-4467-b227-1b91f8967cb7.png)



## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{
    public:
        // Make a new variable
        string name;
        
        // Make the introduce method
        void introduce()
        {
            cout<<"Hie I am -> "<<name<<endl;
        }
};

// Main function
int main()
{
   // Create the new object of the class this will be stored into stack
   Human ajay;
   
   // This will create the object into the heap and it will be created dynamically
   Human *bunty = new Human();
   
   // Assign the values to the class
   ajay.name= "Ajay";
   
   // Assign the values to the class memebers using ptr method
   bunty->name= "Bunty";
   
   // Call the class method
   ajay.introduce();
   
   // Call the class method
   bunty->introduce();
   return 0;
}


```

## 4. Scope Resolution Operator

![Screenshot from 2022-07-23 20-54-53](https://user-images.githubusercontent.com/109052326/180612022-baf234a4-16a5-4a9c-b4cf-c013bdf05aee.png)
![Screenshot from 2022-07-23 21-05-16](https://user-images.githubusercontent.com/109052326/180612024-81653ca7-309e-4147-a600-4d07363f5f7f.png)
![Screenshot from 2022-07-23 21-05-34](https://user-images.githubusercontent.com/109052326/180612026-fcd4ab38-41e7-40b6-8115-9f5afba985ac.png)
![Screenshot from 2022-07-23 21-05-37](https://user-images.githubusercontent.com/109052326/180612030-7f1b3444-8def-47cb-b61f-e60a143ff4da.png)
![Screenshot from 2022-07-23 21-07-14](https://user-images.githubusercontent.com/109052326/180612033-011f0e3a-4c79-4521-a513-d96bb7c2f85c.png)
![Screenshot from 2022-07-23 21-08-43](https://user-images.githubusercontent.com/109052326/180612111-82442822-9c06-40a8-8d63-0e834eb88213.png)
![Screenshot from 2022-07-23 21-08-50](https://user-images.githubusercontent.com/109052326/180612119-23537f5f-37e6-4fb6-bf84-caf0f5191e1d.png)
![Screenshot from 2022-07-23 21-09-14](https://user-images.githubusercontent.com/109052326/180612122-ac161a6e-95d8-40cd-9036-c8c835a227ae.png)
![Screenshot from 2022-07-23 21-09-17](https://user-images.githubusercontent.com/109052326/180612126-debc7527-256e-47bb-a548-101231c3fbb8.png)

## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{
    public:
        // Make a new variable
        string name;
        
        // Make the introduce method
        void introduce();
};

// Using the scope resolution operator
void Human:: introduce()
{
    cout<<Human :: name<<endl;
}

// Main function
int main()
{
   Human anil;
   anil.name= "Anil";
   anil.introduce();
   return 0;
}


```

## 5. Private Access Specifier

![Screenshot from 2022-07-23 21-10-52](https://user-images.githubusercontent.com/109052326/180612478-d42838f6-e061-4149-88f5-5bf18a20a757.png)
![Screenshot from 2022-07-23 21-11-17](https://user-images.githubusercontent.com/109052326/180612479-a3d50d30-1ad6-4006-a5f1-2874addbe11a.png)
![Screenshot from 2022-07-23 21-11-32](https://user-images.githubusercontent.com/109052326/180612482-1f710071-4b81-49bf-aa7d-8e515f5ed8e4.png)
![Screenshot from 2022-07-23 21-11-35](https://user-images.githubusercontent.com/109052326/180612484-025d3cb0-3109-4359-86b0-a32378de06f2.png)
![Screenshot from 2022-07-23 21-12-23](https://user-images.githubusercontent.com/109052326/180612486-b5ba9b66-a95c-4164-ad6c-7df0c5dae4b2.png)
![Screenshot from 2022-07-23 21-12-35](https://user-images.githubusercontent.com/109052326/180612489-c057bf64-2c43-41ae-8e55-cefa2287d9f5.png)
![Screenshot from 2022-07-23 21-12-38](https://user-images.githubusercontent.com/109052326/180612491-66583b11-f40f-46ca-83fb-ff1f23d7e7da.png)
![Screenshot from 2022-07-23 21-16-27](https://user-images.githubusercontent.com/109052326/180612494-75396d9b-dbe8-4f07-be9b-f026c55acd22.png)
![Screenshot from 2022-07-23 21-16-31](https://user-images.githubusercontent.com/109052326/180612496-88f8d92a-295f-4d93-92c9-ab71fdb7b8d7.png)
![Screenshot from 2022-07-23 21-17-25](https://user-images.githubusercontent.com/109052326/180612498-07376313-118b-425a-87c2-009282d5bc2b.png)
![Screenshot from 2022-07-23 21-17-39](https://user-images.githubusercontent.com/109052326/180612500-7e188297-167c-45e2-a8eb-1908016fc41f.png)
![Screenshot from 2022-07-23 21-17-46](https://user-images.githubusercontent.com/109052326/180612502-5661e28c-2009-4d38-b6f7-186cf93dd3f4.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Human class
class Human
{
    // Private memeber variables
    private:
        int age;
    public:
        // void display_age
        void display_age()
        {
            cout<<age<<endl;
        }
        
        // void set_age
        void set_age(int value)
        {
            age= value;
        }
};

// Main function
int main()
{
   Human anil;
   anil.set_age(24);
   anil.display_age();
   return 0;
}


```
