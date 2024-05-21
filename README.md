# Guess-the-number-game

#include<iostream>
#include<conio.h>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{
	int input,r;
	srand(time(0));
	do{

		cout<<"Enter your Guess: "<<endl;
		cin>>input;
		r=rand()%100;
	
	
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
		cout<< "CONGRATULATIONS!! Your guess is correct";
		break;
	}
}while(input!=r);
	return(0);
}
