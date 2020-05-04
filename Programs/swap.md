# Write a function to swap 2 given number using pointer.

- Program
```
#include<iostream>
using namespace std;

void swap(int *x,int *y)
{
        int temp=*x;
        *x=*y;
        *y=temp;
}
int main()
{
        int a,b;
        a=10;
        b=45;
        cout<<"before swapping value of a "<<a<<"b"<<b<<endl;
        swap(&a,&b);
        cout<<"after swapping value od a = "<<a<<"b"<<b<<endl;
        return 0;
}
```
- Output

<img src="programs output/swap op.png">
