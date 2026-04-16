# CodSoft-Task-1
This is a task from CodSoft internship .I have code for the given task,which was the calculator a basic program in c++ language.
#include <iostream>
using namespace std;

int main() {
    double num1, num2;
    int choice;

    // Input two numbers
    cout << "Enter first number: ";
    cin >> num1;

    cout << "Enter second number: ";
    cin >> num2;

    // Display menu
    cout << "Choose operation:\n";
    cout << "1. Addition\n";
    cout << "2. Subtraction\n";
    cout << "3. Multiplication\n";
    cout << "4. Division\n";

    cout << "Enter choice (1-4): ";
    cin >> choice;

    // Perform calculation
    switch(choice) {
        case 1:
            cout << "Result: " << num1 + num2;
            break;

        case 2:
            cout << "Result: " << num1 - num2;
            break;

        case 3:
            cout << "Result: " << num1 * num2;
            break;

        case 4:
            if(num2 != 0)
                cout << "Result: " << num1 / num2;
            else
                cout << "Error! Division by zero.";
            break;

        default:
            cout << "Invalid choice.";
    }

    return 0;
}
