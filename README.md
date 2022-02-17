# C---Solving-2nd-Degree-Equations
This is how you can solve 2nd Degree Equations using C++
------------------------------------------------------------------
#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int A,B,C,D;
    float X1,X2,X;
    cout <<"---------------aX2+bX+c=0-----------"<<endl<<endl;
    cout<<"Enter A: ";
    cin>>A;
    cout<<"Enter B: ";
    cin>>B;
    cout<<"Enter C: ";
    cin>>C;

    D=(B*B)-(4*A*C);
    cout<<endl;

    if (D>0)
    {
        X1=(((-B)+(D))/(2*A));
        X2=(((-B)-(D))/(2*A));
        cout<<"-----------------D>0----------------"<<endl;
        cout<<"X1=  "<<X1<<endl;
        cout<<"X2= "<<X2<<endl;
        cout<<"------------------------------------"<<endl;
    else if (D==0)
    {

        X=(-B)/(2*A);
        cout<<"-----------------D=0----------------"<<endl;
        cout<<"X= "<<X<<endl;
        cout<<"------------------------------------"<<endl;
    }
    else
    {
        system("color 3");
        cout<<"    This Equation has no solution   "<<endl;
        cout<<"               Try Again            "<<endl;
        cout<<"--------------------------------------"<<endl;
    }

    return 0;
}

