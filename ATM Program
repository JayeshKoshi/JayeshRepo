#include <iostream>
#include <conio.h>
#include <string>
using namespace std;
string name, password;
char s;
int n, amount,ded, count,l, dep, ac1, ac2;
int arr[4]= {2000,500,200,100};
class first
{
	public: 
	void v1()
	{
		system("Color 1E");
		cout << "			*-*-* WELCOME *-*-*"<< endl;
		cout << "\n";
		cout << "	*** ENTER YOUR DEBIT/CREDIT/ATM CARD IN THE MACHINE SLOT ***" << endl;
		cout << "		*** (PRESS '*' TO CONTINUE) ***" << "\n";
		cin >> s;
		cout << endl;
		cout << "ENTER PIN: ";
		cin >> password;
		cout << endl;
	}
};
class second: public first
{
	public: 
	void v2()
	{
		if (password=="2405")
		{
			cout << "		*** LOGIN SUCCESSFULL ***" << "\n";
			cout << "\n";
		}
		else if (password!="2405")
		{
			cout << "		-- PIN IS INCORRECT. ENTER PIN AGAIN --" << "\n";
			for (int i=0;i<2;i++)
			cout << "*********************" << "\n";
			cout << "ENTER PIN: ";
			cin >> password;
				if (password=="2405")
				cout << "		*** LOGIN SUCCESSFULL ***" << "\n";
				cout << endl;
		}
		else 
		cout << "*** THANK YOU FOR BANKING WITH US ***" << endl;
	}
};
class third: public second
{
	public: 
	void v3()
	{
		cout << endl;
		cout << "		*-*-* SELECT YOUR OPTION*-*-*" << "\n";
		cout << endl;
		cout << "BALANCE ENQUIRY 	(PRESS -> 1)"<< endl;
		cout << "WITHDRAWL 		(PRESS -> 2)" << "\n";
		cout << "DEPOSIT 		(PRESS -> 3)" << endl;
		cout << "MONEY TRANSFER  	(PRESS -> 4)" << endl;
		cout << "QUIT 			(PRESS -> 0)" << "\n";
		cout << endl;
		cout << "-> ";
		cin >> n;
			if (n==1){
			cout << "TOTAL BALANCE: Rs.50000" << "\n";
			cout << endl;
			cout << "*** THANK YOU FOR BANKING WITH US ***" << endl;}
			else if (n==4)
			{
				cout << "ENTER ACCOUNT NUMBER: ";
				cin >> ac1;
				cout << "RE-ENTER ACCOUNT NUMBER: ";
				cin >> ac2;
				cout << "\n";
				if (ac1==ac2){
					cout << "ENTER AMOUNT TO BE TRANSFERRED(IN THE MULTIPLES OF 100): ";
					cin >> ded;
					cout << endl;
					if (ded%100==0 && ded<50000){
					cout << "AMOUNT TRANSFERRED: Rs." << ded << "\n";
					cout << "AVAILABLE BALANCE: Rs." << 50000-ded << endl;
					cout << endl;
					cout << "		*** THANK YOU FOR BANKING WITH US ***" << endl;}
					else{
					cout << "AMOUNT NOT IN THE MULTIPLES OF 100" << "\n";
					cout << "		*** THANK YOU FOR BANKING WITH US ***" << endl;}
				}
				else 
				{
					cout << "ACCOUNT NUMBER DOES NOT MATCH!" << "\n";
					for (int i=0;i<=10;i++)
					{
						cout << "ENTER ACCOUNT NUMBER: ";
						cin >> ac1;
						cout << "RE-ENTER ACCOUNT NUMBER: ";
						cin >> ac2;
						if (ac1==ac2){
							cout << "ENTER AMOUNT TO BE TRANSFERRED(IN THE MULTIPLES OF 100): ";
							cin >> ded;
							cout << endl;
							cout << "AMOUNT TRANSFERRED: Rs." << ded << "\n";
							cout << "AVAILABLE BALANCE: Rs." << 50000-ded << endl;
							cout << "\n";
							cout << "		*** THANK YOU FOR BANKING WITH US ***" << endl;}
							break;
					}
				}
			}
			else if (n==2)
			{
				cout << "ENTER THE AMOUNT IN THE MULTIPLES OF 100: ";
				cin >> amount;
				cout << endl;
				if (amount>50000)
				cout << "NOT AVAILABLE (LOW BALANCE)" << "\n";
				else{
				cout << endl;
				cout << "*** PLEASE COLLECT YOUR AMOUNT ***" << endl;
				cout << endl;
				cout << "CHECK BALANCE (PRESS 4)" << "\n";
				cin >> l;
				cout << "\n";
				cout << "AMOUNT DEBITED: Rs." << amount << endl;
				cout << "AVAILABLE BALANCE: Rs." << 50000-amount << endl;
				cout << "\n";
				cout << "		*** THANK YOU FOR BANKING WITH US ***" << endl;}
			}
			else if (n==0)
			cout << "*** THANK YOU FOR BANKING WITH US ***" << endl;
			else if (n==3)
			{
				cout << "ENTER AMOUNT TO BE DEPOSITED: ";
				cin >> dep;
				cout << endl;
				cout << "AMOUNT TO BE DEPOSITED: Rs." << dep << "\n";
				cout << "TOTAL BALANCE: Rs." << dep+50000;
				cout << endl;
				cout << "\n";
				cout << "		*** THANK YOU FOR BANKING WITH US  ***" << endl;
			}
			else{
			cout << "INVALID! TRY AGAIN" << "\n";
			cout << "		*** THANK YOU FOR BANKING WITH US  ***" << endl;}
	}
};

int main()
{
	third p;
	p.v1();
	p.v2();
	p.v3();
}
