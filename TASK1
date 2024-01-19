#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    // Seed the random number generator with the current time
    std::srand(std::time(0));

    // Generate a random number between 1 and 100
    int secretNumber = std::rand() % 100 + 1;

    int userGuess;
    int attempts = 0;

    std::cout << "Welcome to the Guess the Number game!\n";

    do {
        // Ask the user for a guess
        std::cout << "Enter your guess (between 1 and 100): ";
        std::cin >> userGuess;

        // Provide feedback on the guess
        if (userGuess < secretNumber) {
            std::cout << "Too low! Try again.\n";
        } else if (userGuess > secretNumber) {
            std::cout << "Too high! Try again.\n";
        } else {
            std::cout << "Congratulations! You guessed the correct number in " << attempts << " attempts.\n";
        }

        // Increment the number of attempts
        attempts++;

    } while (userGuess != secretNumber);

    return 0;
}
