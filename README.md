# student-database-management-system
This is a code using c++.


#include <iostream>
using namespace std;

class Student
{
    char name[30];
    int dob;
    int marks,m1,m2,m3;
    int total;
    float average;
    
    
    public: 
            void getdata(void);
            void display(void);
            
            
};

void Student::getdata()
{
    cout<<"\nEnter name:";
    cin>>name;
    cout<<"Enter Date of Birth:";
    cin>>dob;
    cout<<"Enter first Mark:";
    cin>>m1;
    cout<<"Enter second Mark: ";
    cin>>m2;
    cout<<"Enter third Mark:";
    cin>>m3;
}

void Student :: display(void)
{
    cout<<"\nName:"<<name;
    cout<<"\nDate of Birth:"<<dob;
    cout<<"\nTotal:"<<(m1+m2+m3);
    cout<<"\nAverage:"<<(m1+m2+m3)/3;
    
}

int main()
{
    Student s1,s2,s3;
    s1.getdata();
    s1.display();
    s2.getdata();
    s2.display();
    s3.getdata();
    s3.display();
    return 0;
    
}
