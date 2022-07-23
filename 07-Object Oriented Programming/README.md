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


