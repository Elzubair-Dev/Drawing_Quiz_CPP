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

![1--Drawing-Quiz](https://github.com/Elzubair-Dev/Drawing_Quiz_CPP/assets/104657152/00228654-b39c-4a4c-9d67-3142b7b37575)


![1--Drawing-Quiz-1](https://github.com/Elzubair-Dev/Drawing_Quiz_CPP/assets/104657152/2975d86a-19c0-40c5-9449-ea7b83e6e60f)


## Buy me a Coffee:
if you want to support me
(https://www.buymeacoffee.com/zu698air)

## Done
