#include<iostream>
#include<stdlib>
#include<ctime>
using namespace std;

int main(){
    srand (static_cast<unsigned int>(time(0))); //send for random number generation
    int secretNumber =rand() % 100 + 1; //generate a random number between 1 to 100
    int guess;
    int attempts = 0;
    cout <<"Welcome to the Number Guessing Game!\n";
    cout <<"Try to guess the number between 1 to 100.\n";

    do{
        cout << "Enter your guess:";
        cin>> guess;
        attempts++;

        if (guess > secretNumber){
            cout <<"Too high! Try again.\n";
        }else if 9GUESS , secretNumber){
            cout <<"too low! Try again.\n";
        }else{
            cout <<"Congratulations! You guessed the number in" << attempts << "attempts!\n";
        }
    }
    while (guess != secretNumber);

    return 0;

    }
