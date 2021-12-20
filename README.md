# Calculator



#include <iostream>
#include <string>
#include <math.h>
using namespace std;
int main()
{
	cout << "Enter a number you want the square root and cube root of" << endl;
	int x;
	cin >> x;
	while (cin.fail())
	{
		cout << "Invalid command enter the numbers again: " << endl;
		cin.clear();
		cin.ignore(1000, '\n');
		cin >> x;
	}

	cout << "The square-root of "<<x <<" is " << sqrt(x) << endl;
	cout << "The cube-root of " << x << " is " << cbrt(x) << endl;
	//cout << "The cube-root of "<< x << " is " << pow(x, 0.333333333333333) << endl;
	//cout << "The square-root of "<< x << " is " << pow(x, 0.5) << endl;
	return 0;
}
