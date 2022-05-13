# stack-basiccode
#include <iostream>

using namespace std;


class stack{
    

     // attributes
     public:
     int *arr;
     int top;
     int size;
     //manam attributes or properties ivalli so that the whole class function lo dani values vadachu
    
    stack(int size){
        //oka stack create chesamu anamata
        // ee stack oka well lantidhi we can use when ever we want
        this -> size=size;
        arr=new int [size];
        top=-1;
        
    }
    
    
    // insertion in stack linked list dwara
    void push(int data){
          if (size-top>1){
              top++;
              arr[top]=data;
              
          }
              else {
                  cout<<"stack over flow"<<endl;
              }
              
          }
     void pop(){
          if (top<0){
              cout<<"stack under flow"<<endl;
          }
              else{
                  top--;
                  
              }
          }
};
    
int main()
{
    stack s(5);
    s.push(2);
    s.push(1);
    s.push(8);
    s.push(222);
    s.push(2300);

    


    return 0;
}
