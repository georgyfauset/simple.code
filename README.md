#include <iostream>

int factorial(int number) {
    if (number <= 1) {
        return 1;
    }

    int fact = 1;
    for (int i = 2; i <= number; ++i) {
        fact *= i;
    }

    return fact;
}

int main() {
    int number;

    // Prompt the user to enter a number
    std::cout << "Enter a positive integer: ";
    std::cin >> number;

    // Calculate the factorial of the number
    int result = factorial(number);

    // Display the result
    std::cout << "The factorial of " << number << " is " << result << std::endl;

    return 0;
}
