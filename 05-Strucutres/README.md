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

