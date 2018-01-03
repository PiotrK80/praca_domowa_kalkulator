#include <iostream>
#include <conio.h>
using namespace std;

int dzialanie(int a, int b, int dzialanie);
int main()

{
	int a,b;
	int dzial;
	cout <<endl<<" Podaj A i B:"<<endl;
	cin>>a;
	cin>>b;
	cout<<"wybierz dzialanie:"<<endl;
	cout<< "1 dodawanie" <<endl;
	cout<< "2 odejmowanie" <<endl;
	cout<< "3 mnozenie" <<endl;
	cout<< "4 dzielenie" <<endl;
	cin>>dzial;
	cout<<"Wynik jest rowny "<<endl;
	cout<<dzialanie(a,b,dzialanie)<<endl;
	system("PAUSE");
	return 0;
}

int dzialanie(int a, int b, int dzialanie)
{
	int wynik;

	switch(dzialanie)
{
	case 1 :
	wynik=a+b;
	break;

	case 2 :
	wynik=a-b;
	break;

	case 3 :
	wynik=a*b;
	break;

	case 4 :
	wynik=a/b;
	break;
}

	return wynik;

}