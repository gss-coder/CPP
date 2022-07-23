## 1. Introduction to Structures in C++

![Screenshot from 2022-07-23 10-40-32](https://user-images.githubusercontent.com/109052326/180591542-527edf5f-335e-4bf1-a79d-ae83055fea0f.png)
![Screenshot from 2022-07-23 10-42-23](https://user-images.githubusercontent.com/109052326/180591543-51f1778f-f941-40eb-9811-6af55b551907.png)
![Screenshot from 2022-07-23 10-43-37](https://user-images.githubusercontent.com/109052326/180591544-fe0f1d35-89fa-444d-97c7-c13642253b53.png)
![Screenshot from 2022-07-23 10-44-19](https://user-images.githubusercontent.com/109052326/180591547-3e7de80b-48a5-4cd6-aa80-508b96b9f9f7.png)
![Screenshot from 2022-07-23 10-44-47](https://user-images.githubusercontent.com/109052326/180591548-8bdcaf5c-0b17-4b44-939e-7bc0e9430330.png)
![Screenshot from 2022-07-23 10-44-52](https://user-images.githubusercontent.com/109052326/180591549-b5d1faf1-4276-4977-a0bd-3551e19c3318.png)
![Screenshot from 2022-07-23 10-45-01](https://user-images.githubusercontent.com/109052326/180591550-0d0c08cd-d00b-4978-ac28-6e5a852e5d4c.png)

## Code

```cpp
#include <iostream>
using namespace std;

struct student
{
    int rollno;
    char sex;
    
}vj;

int main()
{
    // Create the struccture variable 
    student vijay;
    
    // Values assignment
    vijay.rollno =333;
    vijay.sex= 'M';
    
    
    // Assign Values to struct variable
    vj.rollno=222;
    vj.sex='M';
    
    // Printing the values of the struct variable
    cout<<vijay.rollno<<vijay.sex<<endl;
    cout<<vj.rollno<<vj.sex<<endl;

    return 0;
}

```

## 2. Arrow Operator with Pointers to Access Structure Members

![Screenshot from 2022-07-23 10-52-35](https://user-images.githubusercontent.com/109052326/180592032-d03e4674-7961-4587-a532-6c9476c3f4cb.png)
![Screenshot from 2022-07-23 10-58-40](https://user-images.githubusercontent.com/109052326/180592038-448674c7-63b8-44d8-a519-c09c3c9fe7ba.png)
![Screenshot from 2022-07-23 11-00-52](https://user-images.githubusercontent.com/109052326/180592039-aaf044d1-f6e7-4a82-bc74-8882c0a1fd10.png)

## Code

```cpp
#include <iostream>
using namespace std;

// Create the structure of type student
struct student
{
    int rollno;
    char sex;
    
};

// Main function
int main()
{
    // Create a struct variable
    student anil;
    
    // Create a pointer to the struct variable
    student *anil_ptr;
    
    // Assign the address to the ptr
    anil_ptr = &anil;
    
    // Assign values
    anil_ptr->rollno = 1234;
    anil_ptr->sex= 'M';
    
    // Print the values
    cout<<anil_ptr->rollno<<" "<<anil_ptr->sex<<endl;
    
    return 0;
}

```

## 3. Passing Structure to Functions by Value, Pointer (Address)

![Screenshot from 2022-07-23 11-07-30](https://user-images.githubusercontent.com/109052326/180608557-abc2a1d7-183d-42a6-a03a-86ee3232b242.png)
![Screenshot from 2022-07-23 19-25-17](https://user-images.githubusercontent.com/109052326/180608560-a01b6de1-ac27-4430-a9d6-9abc35591fd2.png)
![Screenshot from 2022-07-23 19-28-21](https://user-images.githubusercontent.com/109052326/180608561-7f9c6991-d5c2-4d7d-98b7-34ddf5763960.png)
![Screenshot from 2022-07-23 19-29-23](https://user-images.githubusercontent.com/109052326/180608564-2deba668-c2ac-4a09-a4c5-95a5167ade77.png)
![Screenshot from 2022-07-23 19-30-16](https://user-images.githubusercontent.com/109052326/180608566-8d8c550d-37f1-44e5-bb87-edb5b4099fcb.png)
![Screenshot from 2022-07-23 19-31-17](https://user-images.githubusercontent.com/109052326/180608569-240cab4b-c90d-407b-b5ef-2841f495206c.png)
![Screenshot from 2022-07-23 19-31-28](https://user-images.githubusercontent.com/109052326/180608571-ca821d05-3d07-4644-a6f6-7ac73478003c.png)
![Screenshot from 2022-07-23 19-31-42](https://user-images.githubusercontent.com/109052326/180608572-969b906d-9310-4512-9a90-692ac2b96a27.png)
![Screenshot from 2022-07-23 19-31-43](https://user-images.githubusercontent.com/109052326/180608574-6f338f28-537d-4749-b9f7-19907f964ffc.png)
![Screenshot from 2022-07-23 19-31-47](https://user-images.githubusercontent.com/109052326/180608575-ec8c5ca7-daab-4a9a-aa7f-1fad29d723c4.png)
![Screenshot from 2022-07-23 19-31-54](https://user-images.githubusercontent.com/109052326/180608576-b65969a4-a812-4c06-9066-e24be8478730.png)
![Screenshot from 2022-07-23 19-34-47](https://user-images.githubusercontent.com/109052326/180608577-3c74b21b-d8ee-465b-879f-066c88a8d2cf.png)
![Screenshot from 2022-07-23 19-34-53](https://user-images.githubusercontent.com/109052326/180608580-634f0771-f6f8-4765-ae0b-9205e5949194.png)
![Screenshot from 2022-07-23 19-35-01](https://user-images.githubusercontent.com/109052326/180608581-cdc1e412-b321-4246-8837-795290c54f30.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

struct student
{
    int rollno;
    char sex;
    int age;
};

void display(student s)
{
    cout<< s.rollno <<endl;
    cout<<s.sex<<endl;
    cout<<s.age<<endl;
    
    // This change will not be refelcted since its a pass by val
    // s.rollno = 0000;

}

void show(student *s)
{
    cout<<s->rollno <<endl;
    cout<<s->sex<<endl;
    
    // This change will be refelcted since its a pass by reference
    s->rollno = 1111;
    cout<<s->rollno<<endl;


        
}
int main()
{
    student anil ={1234,'m',23};
    display(anil);
    show(&anil);
    return 0;
}


```
## 4. Nested Structures and C++ Dot Operator

![Screenshot from 2022-07-23 19-39-16](https://user-images.githubusercontent.com/109052326/180608960-3ff31465-cb17-4114-be77-5f3842a9e761.png)
![Screenshot from 2022-07-23 19-39-27](https://user-images.githubusercontent.com/109052326/180608964-bc87ed2a-79e8-46c3-8c78-977101ac0d2d.png)
![Screenshot from 2022-07-23 19-40-53](https://user-images.githubusercontent.com/109052326/180608965-e9ea5a44-cc77-4b11-bde1-3759a3b6f089.png)
![Screenshot from 2022-07-23 19-46-42](https://user-images.githubusercontent.com/109052326/180608966-1c623ee7-113e-4618-a53e-92de8365327a.png)
![Screenshot from 2022-07-23 19-46-47](https://user-images.githubusercontent.com/109052326/180608968-b46cff84-4b0b-46ab-aa82-d0f123dc4edb.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a struct adddress
struct address
{
    int house_no;
    string street_name;
    
};

// Make a struct student
struct student
{
    string name;
    int roll;
    address add;
    
};

// Main function
int main()
{
   // Create a struct variable
   student anil;
   
   // Assign the struct variable
   anil.name="anil";
   anil.roll=1234;
   
   // Nested struct assignment
   anil.add.house_no=300;
   anil.add.street_name="MG ROAD";
   
   // Print all the information
   cout<<anil.name<<endl;
   cout<<anil.roll<<endl;
   cout<<anil.add.house_no<<endl;
   cout<<anil.add.street_name<<endl;
   
   
   return 0;
}


```

## 5. Accessing C++ Nested Structure Members using Arrow Operator

![Screenshot from 2022-07-23 19-48-17](https://user-images.githubusercontent.com/109052326/180609289-e38acf5c-3a6c-4e2a-ac66-1386b6f76f09.png)
![Screenshot from 2022-07-23 19-49-46](https://user-images.githubusercontent.com/109052326/180609291-600f9487-4ad3-4582-9d21-0467cac38fdf.png)
![Screenshot from 2022-07-23 19-49-57](https://user-images.githubusercontent.com/109052326/180609292-8d007d03-c9b7-44e3-affc-2acabcf018cb.png)
![Screenshot from 2022-07-23 19-52-24](https://user-images.githubusercontent.com/109052326/180609294-20bbf36e-ebe1-499e-b1ba-85dafb225424.png)
![Screenshot from 2022-07-23 19-52-32](https://user-images.githubusercontent.com/109052326/180609296-08c592ea-66fd-48a9-9ced-18236d5016e6.png)
![Screenshot from 2022-07-23 19-53-23](https://user-images.githubusercontent.com/109052326/180609298-423262db-3be4-4422-bab8-c59eb22114ff.png)
![Screenshot from 2022-07-23 19-53-34](https://user-images.githubusercontent.com/109052326/180609301-3a735233-ab40-4033-9b0c-85b25b31a558.png)
![Screenshot from 2022-07-23 19-53-44](https://user-images.githubusercontent.com/109052326/180609303-9476984b-0673-4617-9260-8511ac2a6139.png)
![Screenshot from 2022-07-23 19-53-46](https://user-images.githubusercontent.com/109052326/180609304-4195ef7c-9fa6-4ef5-ba28-b699b971676a.png)
![Screenshot from 2022-07-23 19-54-12](https://user-images.githubusercontent.com/109052326/180609305-db280f6f-fb48-496c-96f7-180e1d86e921.png)
![Screenshot from 2022-07-23 19-54-24](https://user-images.githubusercontent.com/109052326/180609306-d57b30ee-6c7f-4a11-8ab8-8872aca8da19.png)


## Code

```cpp
#include <bits/stdc++.h>
using namespace std;

// Make a struct adddress
struct address
{
    int house_no;
    string street_name;
    
};

// Make a struct student
struct student
{
    string name;
    int roll;
    address add;
    
};

// Main function
int main()
{
   // Create a struct variable
   student anil;
   
   // create the pointer of type structure
   student *anilptr;
   
   // Take the address of anil into the anilptr
   anilptr = &anil;
   
   // Assign the struct variable
   anilptr->name="anil";
   anilptr->roll=1234;
   
   // Nested struct assignment
   anilptr->add.house_no=300;
   anilptr->add.street_name="MG ROAD";
   
   // Print all the information
   cout<<anilptr->name<<endl;
   cout<<anilptr->roll<<endl;
   cout<<anilptr->add.house_no<<endl;
   cout<<anilptr->add.street_name<<endl;
   
   
   return 0;
}

```

