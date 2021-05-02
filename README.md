//header files
#include <iostream>
#include <stdlib.h>
#include <stdio.h>

using namespace std;



int main()
{
	signed long int x, y, z; //define var x,y,z,sum as long int -2,147,483,648 => 2,147,483,648
	char op;
	/*input*/
	cout << "Dumb calculator" << endl;
	cout << "Type the first value: " << endl;
	cin >> x;
	cout << "type in your second value: " << endl;
	cin >> y;
	cout << "type in your thrid value: " << endl;
	cin >> z;
	cout << "Choose a operator:[+][-][*][/]" << endl;
	cin >> op;
	cout << x;
	cout << op;
	cout << y;
	cout << op;
	cout << z;
	cout << "=";
	

	/*output*/
	switch (op)
	{
	case '+':
		cout << x + y + z;
		break;

	case'-':
		cout << x - y - z;
		break;

	case 'x':
		cout <<x*y*z;
		break;

	case'/':
		x / y / z;
		break;

	default:
		cout << "Oops, you've met an error.";
		cout << "Reasons may be:"<< endl;
		cout << "(1)sum over 2e32" << endl;
		cout << "(2)Wrong Operator."<< endl;
		cout << "(3)Unknown error" << endl;
	}

	return 0;
	system("pause");
}

//by Timothy51 at github
