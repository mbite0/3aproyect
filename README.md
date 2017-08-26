# 3aproyect

using namespace std;
int main()
{
	int val,num,div,tem,res,cont=0;
	
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
				while(num>0&&num>div&&num%div>0)
					div++;
				if(div==num)
    				cout<<"\nnumero es primo";
    			else
					cout<<"\nnumero no es primo";
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
				
				while (num!=-1)
				{
				cout<<"\nCalificaciones: ";
				cin>>num;
					if(num!=-1)
					{
					res+=num;
					cont++;
					}
					//else
						//cout<<tem=(res++)/(cont--);
				}
				cout<<tem;
			break;
			case 0:
				cout<<"Vuelva pronto";
			break;
		}
	}
	while (val=0);
	return 0;
