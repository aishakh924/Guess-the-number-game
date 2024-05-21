# Guess-the-number-game

#include<iostream>
#include<conio.h>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{
	int input,r,tries=0;
	srand(time(0));
	r=rand()%100;
	cout<<"WELCOME to guess the number game!"<<endl;
	do{

		cout<<"Enter your Guess: "<<endl;
		cin>>input;
		
	
	
	if(input>r)
	{
		cout<<"The number you've guessed is TOO HIGH. Try again! ";
	}
	else if(input<r)
	{
		cout<<"The number you've guessed is TOO LOW. Try again! ";
	}
	else if(input==r)
	{
		cout<< "CONGRATULATIONS!! Your guess is correct"<<endl;
		break;
	}
	tries++;
}while(input!=r);
cout<<"Total tries are :"<<tries;
	return(0);
}
