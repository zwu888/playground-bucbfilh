# 
```C++ runnable
#include <iostream>

using namespace std;

class Base {
    public:
        Base() { cout << "Base() called" << endl;
        }
};

class S1:public Base {
    public:
        S1() { cout << "S1() called" << endl;}
};

class S1:public virtual Base {
    public:
        S1() { cout << "S2() called" << endl;}
};

class M : public S1, public S2 {
    public:
         M() { cout << "M() called" << endl;}
};

int main() 
{
    M mm;
    return 0;
}
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C++ template](https://tech.io/select-repo/598)
