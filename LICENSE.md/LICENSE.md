
#include <iostream>
using namespace std;
class calc {
private:
    int *n1 , *n2;
public:
    calc () {
        n1= new int;
        n2= new int;
        cout<<"enter the first number:"<<endl;
        cin>>*n1;
        cout<<"enter the second number:"<<endl;
        cin>>*n2;
    }
    ~calc (){
        delete n1;
        delete n2;
        cout<<"there data member are deleted:"<<endl;
        
    }
    int sum (){
        return *n1 + *n2;
    }
    int sub(){
        return *n1 - *n2;
    }
    int mult (){
        return *n1 * *n2;
    }
    int div (){
        return *n1 / *n2;
        
    }
    int mod (){
        return *n1 % *n2;
    }
    
};

int main (){
    calc c;
    cout<<"there summation is : "<<c.sum()<<endl;
    cout<<"there subtraction is : "<<c.sub()<<endl;cout<<"there multblcation is : "<<c.mult()<<endl;cout<<"there summation is : "<<c.div()<<endl;cout<<"there remainder is : "<<c.mod()<<endl;
    return 0;
}
