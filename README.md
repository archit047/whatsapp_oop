# whatsapp_oop

#include<iostream>
using namespace std;


class chat
{

string cont,chat_name;
int n;

void conts()
{
for(i=0;i<n;i++)
{
cin>>cont[i];
}

cout<<"which chat you want to delete \n";
cout<<"enter the name \n";
cin>>chat_name;

for(i=0;i<n;i++)
{
if(cont[i]==chat_name)
{
cont[i]='';
}
cout<<cont[i];
}
}
};



class user:public chat
{
int contact;
char name;

void person()
{
cout<<"name of the user is \n"<<name;
cout<<"name of the contact is"<<contact;
}

};

class send_message_by_user 
{
int p;
void msg1()
{
cout<<"if you enter 1 you can send an image \n"
cout<<" if you enter 2 you can send a text \n";
cout<<"if you enter 3 you can send a video \n";
cout<<"if you enter 4 you can send an audio\n";

switch(p)
{
case 1: 
cout<<"Its an image";
break;

case 2:
cout<<"Its a text";
break;

case 3:
cout<<"its a video";
break;

case 4:
cout<<"its an audio";
break;

default:
cout<<"you have not enter a valid value";
}

}
};

class text
{
string txt;

void check()
{

if(txt>=97 && txt<=122 || txt>=65 && txt<=90)
{
cout<<" it is a text not an image \n";
}
else
{
cout<<"it is something else \n";
}
}
}


class status: public text
{
 
 void stats()
 {
 cout<<"this class and the function is used  to check status if there is any or not \n";
 }

};


int main()
{
   int ct;
   cin>>ct;
  user us;             
  us.chat_name="Samyank";
  us.conts();
  us.contact= ct;
  us.name="ARCHIT_NEGI";
  
  
  send_message_by_user typ;
  typ.p=2;
  typ.msg1();
  
  
  status std;
  std.txt = "status";
  std.check();
  std.stats();
return 0;
}
