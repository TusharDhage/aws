**create a class "MyClass1" with members and member function "disp1().
create another class "MyClass2" with members and member function "disp2().
now try to invoke disp1() from disp2()in the main() function,
 create instances of both the classes and invoke their member functions.**


- Program
```
#include <iostream>
using namespace std;

class Myclass1
{
        public:
                void display1()
                {
                        cout<<"you are in display1"<<endl;
                }
};
class Myclass2
{
        public:
                void display2(Myclass1 &ref)
                {
                        cout<<"you are in display2"<<endl;
                        ref.display1();
                }
};
 int main()
{
        Myclass1 c1;
        Myclass2 c2;
        c2.display2(c1);
        return 0;
}
```

- Output

<img src="programs output/funol op.png">