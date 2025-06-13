# Calculator
C++ Code For Calculator

#include <iostream>                                                                                                                                                                                                                                            #include <iostream>
using namespace std;

int main() {
    // Declare variables
    double number1, number2;
    char operation;

    // Introduction message
    cout << "==============================" << endl;
    cout << "  Welcome to C++ Calculator! " << endl;
    cout << "==============================" << endl;

    // Get first number from the user
    cout << "Enter the first number: ";
    cin >> number1;

    // Get second number from the user
    cout << "Enter the second number: ";
    cin >> number2;

    // Ask the user to choose an operation
    cout << "Choose an operation (+, -, *, /): ";
    cin >> operation;

    // Perform the operation based on user input
    cout << "------------------------------" << endl;
    switch (operation) {
        case '+':
            cout << "Result: " << number1 << " + " << number2 << " = " << number1 + number2 << endl;
            break;
        case '-':
            cout << "Result: " << number1 << " - " << number2 << " = " << number1 - number2 << endl;
            break;
        case '*':
            cout << "Result: " << number1 << " * " << number2 << " = " << number1 * number2 << endl;
            break;
        case '/':
            if (number2 != 0)
                cout << "Result: " << number1 << " / " << number2 << " = " << number1 / number2 << endl;
            else
                cout << "Error: Division by zero is not allowed!" << endl;
            break;
        default:
            cout << "Invalid operation! Please use +, -, *, or /." << endl;
    }

    // Goodbye message
    cout << "------------------------------" << endl;
    cout << "Thank you for using the calculator!" << endl;

    return 0;
}
