
#include <iostream>
#include<cstdlib>
using namespace std;

int main(){


cout << "Welcome to the number guessing game!" <<endl;

int num;
int count;
int guess;



   num = 1+(rand()%1000);


while (num != guess){
    cout << "Enter your guess between 1 to 1000):" <<endl;
    cin >> guess;
    if (guess>num){
        cout << " your guess is Too high! Try again." <<endl;
    }
    if(guess<num){
        cout << " your guess is Too low! Try again." <<endl;
    }
    count++;
}

cout << "Correct! You found the correct number in " << count <<" tries." <<std::endl;


return 0;
}
