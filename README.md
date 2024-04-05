# Practical-5-2-
#include<iostream>
using namespace std;

class convert {
public:
double cm;
double cm_mt(){
     return cm * 0.01; 
}
double cm_km(){
     return cm * 0.00001;
}
double cm_ft(){
     return cm * 0.0328;
}
double cm_in(){
     return cm * 0.3937;
}
};
int main()
{ 
    convert v1;
    double w,x,y,z;
    cout << "Enter Value in centimetre: " << endl;
    cin >> v1.cm;
    w = v1.cm_mt();
    x = v1.cm_km();
    y = v1.cm_ft();
    z = v1.cm_in();
    cout << "CM to Meter is: " << w << endl;
    cout << "CM to Kilometre is: " << x << endl;
    cout << "CM to Feet is: " << y << endl;
    cout << "CM to Inches is: " << z << endl;
    return 0;
}
