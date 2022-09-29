# Guess-the-Number
#include <stdio.h>
#include <conio.h>
#include <time.h>

int main()
{
	int num,guess,count=1;
	//srand(time(0));
	num=rand()%100 + 1;//random number generates b\w 1-100.
	//printf("The number is %d\n", num);
	//guess the number.
	do
	{  
	printf("Guess the number between 1 and 100\n");
	scanf("%d\n", &guess);
	if(guess>num)
	{
		printf("Lower number please!\n");
	}
	else if(guess<num)
	{
		printf("Higher number please!\n");
	}
	else
	{
		printf("You guess the number in %d attempts\n", count);
	}	
	count++;
	}while(guess!=num);
	return 0;
}
