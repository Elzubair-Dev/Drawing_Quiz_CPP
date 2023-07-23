# Drawing_Quiz_CPP
A well-known C++ quiz that asks you to draw a diamond shape based on the number of rows entered by the user

## Explanation
Enter any number of rows you want and press ENTER

## Code:

using namespace std;
#include <iostream>
int main()
{
	int row = 1, half;
	bool isEven = false;
	cout << "Enter the Number of rows \n\n";
	cout << "Rows = ";
	cin >> row;
	cout << "\n------------------------------\n\n";
	if (row % 2 == 0) {
		half = row  / 2;
		isEven = true;
	}
	else {
		half = (row + 1) / 2;
		isEven = false;
	}
	for (int i = 1; i <= row; i++)
	{
		if (i <= half) 
		{
			for (int j = 1; j <= half - i; j++)cout << " ";
			for (int j = 1; j <= i * 2; j++)
			{
				if (j <= i)cout << i - (j - 1);
				else if (j > i)  cout << j  - i;
			}
		}
		else
		{
			if (isEven) {
				for (int j = 1; j <= i - (half + 1); j++)cout << " ";
				for (int j = 1; j <= ((row + 2) - 2 * (i - half)); j++)
				{
					if (j <= ((row + 2) - 2 * (i - half)) / 2) cout << ((row + 1) - i - (j - 1));
					else if (j > ((row + 1) - 2 * (i - half)) / 2) cout << ((j + i) - (row + 1));
				}
			}
			else {
				for (int j = 1; j <= i - half; j++)cout << " ";
				for (int j = 1; j <= ((row + 1) - 2 * (i - half)); j++)
				{
					if (j <= ((row + 1) - 2 * (i - half)) / 2)cout << ((row + 1) - i - (j - 1));
					else if (j > ((row + 1) - 2 * (i - half)) / 2) cout << ((j + i) - (row + 1));
				}
			}
		}
		cout << "\n";
	}
}

## Screens:
![Screenshot of the quiz.]
(https://drive.google.com/file/d/19Nc8dk9HPN6Ypek_Kfg3fv9tQkaUrWc9/view?usp=drive_link)
(https://drive.google.com/file/d/1YXFGA8fx_d7nA4yNZbSt5CKk03NIFG25/view?usp=drive_link)

## Buy me a Coffee:
if you want to support me
(https://www.buymeacoffee.com/zu698air)

## Done
