# Source-code-for-ATM-in-C-
A personal project
#include <iostream>
#include<string>

using namespace std;

int main()
{
    long int acc_no;
    int pin;
    int option = 0;
    double acc_bal = 89.99;
    int choice;
    int amount;
    int old_pin;
    int new_pin;
    int acc_rec;
    int bank_name;
    int choice3;
    int choice2;
    int what_amt;
    long int bvn;
    int sent_code;
    long int num_ent;
    char myname[20];
    int late;

    ATM:
    cout<<"WELCOME DEAR CUSTOMER\n";
    cout<<"************************************************************************************************************\n\n\n";
    cout<<"\nENTER PIN\n";
    cin>>pin;
    cout<<"1. CHECK BALANCE\n";
    cout<<"2. WITHDRAWAL\n";
    cout<<"3. RECHARGE\n";
    cout<<"4. CHANGE PIN\n";
    cout<<"5. CREATE AN ACCOUNT\n";
    cout<<"6. TRANSFER\n";
    cout<<"7. CANCEL\n";

        cin>>option;


        if(option != 0)
    {

        switch(option)
        {
            case 1:
               cout<<"\nYOUR LEDGER BALANCE IS $"<<acc_bal<<endl;
                break;

            case 2:
                cout<<"1. 500\n";
                cout<<"2. 1000\n";
                cout<<"3. 2000\n";
                cout<<"1. 3000\n";
                cout<<"4. 5000\n";
                cout<<"5. 10,000\n";
                cout<<"6. 20,000\n";
                cout<<"7. 50,000\n";
                cout<<"8. 100,000\n";
                cout<<"9. 150,000\n";
                cout<<"10.OTHER\n";
                cin>>choice;
                 if(choice == 10)
                 {
                     cin>>what_amt;
                 }
                cout<<"\nPLEASE WAIT! \nCOLLECT YOUR CASH\n";
                break;

            case 3:
                cout<<"ENTER AMOUNT\n";
                cin>>amount;
                cout<<"RECHARGE SUCCESSFUL\n";
                break;

            case 4:
                cout<<"ENTER OLD PIN\n";
                cin>>old_pin;
                cout<<"ENTER NEW PIIN\n";
                cin>>new_pin;
                cout<<"PIN CHANGE IS SUCCESSFUL!\n";
                break;
            case 5:
                cout<<"ENTER NAME\n";
                cin>>myname;
                cout<<"ENTER BANK VERIFICATION NUMBER\n";
                cin>>bvn;
                cout<<"ENTER YOUR PHONE NUMBER\n";
                cin>>num_ent;
                cout<<"A NEW CODE WAS JUST SENT TO YOUR LINE. ENTER THE CODE\n";
                cin>>sent_code;
                cout<<"WE WILL GET BACK TO YOU SHORTLY!\n";
                break;

            case 6:
                cout<<"ENTER ACCOUNT NUMBER OF THE RECIPIENT\n";
                cin>>acc_rec;
                cout<<"\nPICK THE RECIPIENT'S BANK NAME\n";
                cout<<"1. FIRST BANK PLC\n";
                cout<<"2. DIAMOND BANK\n";
                cout<<"3. FIDELITY BANK.\n";
                cout<<"4. GTB\n";
                cout<<"5. UBA\n";
                cout<<"6. STANBIC IBTC BANK plc\n";
                cout<<"7. FCMB\n";
                cout<<"8. ZENITH\n";
                cout<<"9. ACCESS\n";
                cout<<"10. UNION BANK\n";
                cout<<"11. POLARIS\n";
                cout<<"12. KEYSTONE\n";
                cout<<"13. ECO BANK \n";
                cout<<"14. OTHER\n";

                cin>>bank_name;
                if(bank_name == 14)
                {
                    cout<<"15. JAIZ BANK\n";
                    cout<<"16. CITY BANK\n";
                    cout<<"17. MAINSTREET BANK LIMITED\n";
                    cout<<"18. UNITY BANK\n";
                    cout<<"19. HERITAGE BANK\n";
                    cout<<"20. STERLING BANK\n";
                    cout<<"22. STANDARD CHARTERED\n";
                    cout<<"23. WEMA BANK\n";
                    cout<<"24. SUNTRUST BANK\n";
                    cin>>late;
                }

                cout<"\n\nSELECT AMOUNT\n";
                cout<<"1. 500\n";
                cout<<"2. 1000\n";
                cout<<"3. 2000\n";
                cout<<"1. 3000\n";
                cout<<"4. 5000\n";
                cout<<"5. 10,000\n";
                cout<<"6. 20,000\n";
                cout<<"7. 50,000\n";
                cout<<"8. 100,000\n";
                cout<<"9. 150,000\n";
                cout<<"10. OTHER\n";
                cin>>amount;
                 if(choice == 10)
                 {
                     cin>>what_amt;
                 }
                cout<<"\n1. PROCEED\n";
                cout<<"2. CANCEL\n";
                cin>>choice2;
                   if(choice2 == 1)
                       {
                           cout<<"TRANSFER SUCCESSFUL\n";
                       }
                   else{
                           cout<<"TRANSFER INTERUPTED OR CANCELLED\n";
                       }
                 break;

            case 7:
                cout<<"OPEATION CANCELLED!\n";
                break;

            default:
                cout<<"INVALID COMMAND!"<<endl;
            }
        }


    cout<<"DO YOU WANT TO PERFORM ANOTHER OPERATION?\n";
    cout<<"1. NO"<<endl;
    cout<<"2. YES"<<endl;
    cin>>choice3;
    if (choice3 == 1)
    {
        cout<<"PLEASE, TAKE YOUR CARD\n";
    }
    else
    {
        goto ATM;
    }


    return 0;
}
