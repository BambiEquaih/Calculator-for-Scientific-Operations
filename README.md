# Calculator-for-Scientific-Operations
GBONO AGNES/UEB3261222
#include <iostream>
#include <cmath>
#include <stdexcept>

class ScientificCalculator {
public:
    // ... (rest of your class methods remain unchanged)
};

int main() {
    ScientificCalculator calculator;

    while (true) {
        try {
            std::cout << "Available operations:\n";
            std::cout << " - add, subtract, multiply, divide, modulo\n";
            std::cout << " - sin, cos, log\n";
            std::cout << "Enter operation (or 'quit' to exit): ";

            std::string operation;
            std::cin >> operation;

            if (operation == "quit") {
                break;
            }

            double result = 0;
            if (operation == "add" || operation == "subtract" || operation == "multiply" ||
                operation == "divide" || operation == "modulo") {
                double a, b;
                std::cout << "Enter two numbers: ";
                std::cin >> a >> b;

                // ... (rest of your code remains unchanged)
            } else if (operation == "sin" || operation == "cos" || operation == "log") {
                double value;
                std::cout << "Enter a number: ";
                std::cin >> value;

                // ... (rest of your code remains unchanged)
            } else {
                std::cout << "Invalid operation.\n";
                continue;
            }

            std::cout << "Result: " << std::fixed << result << "\n";
        } catch (const std::exception& e) {
            std::cout << "Error: " << e.what() << "\n";
        }
    }

    return 0;
}
