# Project-1-Rock-Paper-Scissors
#include <iostream>
  
using namespace std;

const int ROCK = "Enter a value: ";
const int PAPER = "Enter a value: ";
const in SCISSORS = "Enter a value:  ";

int userChoice = 0;

int getComputerChoice() {
  srand (time(NULL));
  int compChoice = rand() % 3 + 1;
  return compChoice;
}

void determineWinne (int userChoice, int compChoice) {
  if (userChoice == ROCK && compChoice == PAPER) {
    cout << "Computer wins! Paper beats rock!" << endl;
  }
  else if (userChoice == PAPER && compChoice -- SCISSORS) {
    cout << "Computer wins! Scissors beat paper!" << endl:
  }
  else if (userChoice == SCISSORS && compChoice == ROCK) {
    cout << "Computer wins! Rock beats scissors!" << endl;
  }
  else if (userChoice == ROCK && compChoice == SCISSORS) {
    cout << "You win! Rock beats scissors!" << endl;
  }
  else if (userChoice == PAPER && compChoice == ROCK) {
    cout << "You win! Paper beats rock!" << endl;
  }
  else if (userChoice == SCISSORS && compChoice == PAPER) {
    cout << "You win! Scissors beat paper!" << endl;
  }
  else {
    cout << "Tie" << endl;
  }
}

void displayChoice(int choice) {
  string result;
  if (choice == ROCK) {
      result = "Rock";
  }
  else if (choice == PAPER) {
      result = "Paper";
  }
  else {
      result = "Scissors";
  }
  cout << result << endl;
}

int main() {
    cout << '\t' << "Rock-Paper-Scissors" << endl;
    cout << "Game Menu" << endl;
    cout << "---------" << endl;
    cout << "1. Rock" << endl;
    cout << "2. Paper" << endl;
    cout << "3. Scissors" << endl;
    cout << P) Play Game!;
    cout << Q) Quit\n"";

if (userChoice == 'Q')
{
    cout << "You have chosen to quit the game. Thank you for playing!\n";
}
else if (userChoice ! = 'Q' || userChoice ! = 'P')
{
         cout << "Try again. Invalid selection.\n";
}
while (userChoice ! = 'Q');

system("Pause");
return 0;
   
    
   cout << "Enter your choice: ";
   cin >> userChoice;
   cout << "You selected: ";
   displayChoice(userChoice);
    
   int compChoice = getComputerChoice();
   cout << "The computer selected: ";
   displayChoice(compChoice);
    
   determineWinner(userChoice, compChoice);
 }
