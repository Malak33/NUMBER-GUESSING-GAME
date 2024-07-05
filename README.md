#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
	int num = 0, m=1 , time =5;
	cout << " Guess Number from 1 to 100 " << endl;
	do
	{
		cout << " turns remaning " << time + 1 << endl;
		cin >> num;
		int guess = rand() % 100 + 1;
		if (num == guess)
		{
			cout << "Great guess ! that's the correct number  " << endl;
		}
		else if (num > guess)
		{
			cout << " the guess is too low " << endl;
		}
		else if (num < guess)
		{
			cout << " the guess is too high " << endl;
		}
		else
		{
			cout << " sorry you lost the game " << endl;
		}
	} while (m == 1 && time--);
	
	return 0;

}
