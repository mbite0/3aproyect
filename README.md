# 3aproyect
#include<iostream>
using namespace std;
int main()
{
	int val,num,primo,tem,res;
	
	do
	{
		cout<<"\t\t\t\tMENU:\n\n\n";
		cout<<"\t\t\tOpciones: \n\n";
		cout<<"\t\t1==> El valor es primo?\n";
		cout<<"\t\t2==> Factorial\n";
		cout<<"\t\t3==> Promedio\n";
		cout<<"\t\t0==> salir\n\n";
		cout<<"\t\tElije una opcion: ";
		cin>>val;
		switch (val)
		{
			case 1:
				cout<<"\n\nIngrese el valor: ";
				cin>>num;
				if(num==2)
					cout<<"\n\nEl valor es primo";
				else
				if(num%2==0)
					cout<<"\n\nEl valor no es primo";
					else
					cout<<"El valor es primo";
			break;
			case 2:
				cout<<"\n\nIngrese el valor: ";
				cin>>num;
					tem=num-1;
					res=num;
				while(tem>=1)
				{
					res=res*tem;
					tem--;
				}
				cout<<"\t\tel factorial de: "<<num<<" es: "<<res<<"";
			break;
			case 3:
				cout<<"\t\tIngurese sus calificaciones separadas por un enter\n\t\tpara dejar de introducir datos coloque -1\n";
				cin>>tem;
				while(tem!=-1)
				{
					cout<<"ingrese la calificacion: ";
					cin>>tem;
					if(tem!=-1)
					{
						res+=tem;
						num++;
					}
					else
					{
						val=res/num;
					}
				}
				cout<<"el promedio es:\n"<<val;
			break;
		}
	}
	while (val!=0);
	return 0;
}
