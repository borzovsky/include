# include

#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    // Seed the random number generator
    srand(time(0));
    
    // Generate a random number between 1 and 10
    int secretNumber = rand() % 10 + 1;
    
    // Declare variable
    int guess;
    
    // Get input from the user
    std::cout << "Guess the number (between 1 and 10): ";
    std::cin >> guess;
    
    // Check if the guess is correct
    if (guess == secretNumber) {
        std::cout << "Congratulations! You guessed the correct number." << std::endl;
    } else {
        std::cout << "Sorry, the correct number was " << secretNumber << "." << std::endl;
    }
    
    return 0;
}
