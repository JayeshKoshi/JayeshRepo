#include <iostream>
#include <stdlib.h>
#include <conio.h>
#include <string.h>
using namespace std;

class casino_game
{
    public: 
    void disp()
    {
        cout << "---------- *CASINO GAME* ----------" <<endl;
        cout << "           -------------           " <<endl;
        cout << endl;
        cout << "             *WELCOME*             " <<endl;
        cout << endl;
        cout << "PRESS ANY KEY TO CONTINUE " << endl;
        getch();
        system("cls");
    }
    void inst()
    {
        cout << "           *//*INSTRUCTIONS*//*          " << endl;
        cout << endl;
        cout << "1. The Player will choose a number between 1-10."<<endl;
        cout << "2. If the number chosen by the player is winning, then the Player will get 10x the money bet."<<endl;
        cout << "3. If the Player fails to guess the winning number, the Player will loose the money bet."<<endl;
        cout << "4. Player can stop playing anytime they want."<<endl;
        cout << endl;
        cout << "PRESS ANY KEY TO CONTINUE "<<endl;
        getch();
        system("cls");
    }
    void main_menu()
    {
        int n;
        cout << "START (Press 1)"<<endl;
        cout << "HELP (Press 2)"<<endl;
        cout << "QUIT (Press 3)"<<endl;
        cin >> n;

        switch(n)
        {
            case 1:
            start();
            break;
            case 2:
            inst();
            break;
            case 3:
            break;
        }
    }
    void start()
    {
        char ch;
        string name;
        int guess, randnum, run=0;
        int bal = 10000, betAmt;
        cout << "PLEASE ENTER YOUR NAME:- ";
        cin >> name;
        while (run==0)
        {
            cout << "           ***DOUBLE OR NOTHING***         "<<endl;
            cout << "           -----------------------         "<<endl;
            cout << endl;
            cout << "                                           BALANCE:- "<< bal<<endl;
            bet:
            cout << "ENTER YOUR GUESS:- ";
            cin >> guess;
            cout << "ENTER YOUR BETTING AMOUNT:- ";
            cin >> betAmt;
            if (betAmt>bal)
            {
                cout << "INSUFFICIENT BALANCE !"<<endl;
                goto bet;
            }
            else
            {
                bal= bal - betAmt;
            }

            randnum = rand()%10;
            cout << "WINNING NUMBER:- " << randnum << endl;
            if (randnum!=guess)
            {
                cout << "YOU LOST !!" << endl;
                cout << "WOULD YOU LIKE TO TRY AGAIN (Y/N)"<<endl;
                cin >> ch;
                if (ch=='n' || ch=='N')
                {
                    run=1;
                    cout << "/*/*/*/*/* THANKS FOR PLAYING */*/*/*/*/"<<endl;
                    cout << "Rs. " << bal << " will be credited in your account." <<endl;
                }
                else if (ch=='y' || ch=='Y')
                {
                    system("cls");
                }
            }
            else
            {
                cout << "** CONGRATULATIONS YOU WON **"<< endl;
                bal = bal + (10 * betAmt);
            }
        }
    }
};

int main()
{
    casino_game p;
    p.disp();
    p.inst();
    p.main_menu();
}

