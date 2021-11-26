# Table-till-10
#While loop
#include<iostream>
using namespace std;
int main()
{
	int table, z = 1;
	cout << "Table of : ";
	cin >> table;
    while (cin.fail()!=0)
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Invalid command! Enter the number : " << endl;
		cin >> table;
	}
	while (z <= 10)
	{
		cout << "\n" << table << " X " << z << " = " << table * z << endl;
		z++;
	}
	return 0;
}
