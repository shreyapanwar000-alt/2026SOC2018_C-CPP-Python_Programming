#include <iostream>
#include <string>

using namespace std;

// Student class definition
class Student {
    // Private data members
    int roll;
    string name;
    float marks[3];
    float total;
    float percentage;

public:
    // Function to take input from the user
    void accept() {
        cout << "Enter roll number: ";
        cin >> roll;
        cin.ignore(); // Clears the newline character left in input stream

        cout << "Enter name: ";
        getline(cin, name);

        cout << "Enter marks for 3 subjects:\n";
        for (int i = 0; i < 3; i++) {
            cout << "Subject " << i + 1 << ": ";
            cin >> marks[i];
        }
    }

    // Function to calculate total marks and percentage
    void calculate() {
        total = 0;
        for (int i = 0; i < 3; i++) {
            total += marks[i]; // Sum up the marks
        }
        percentage = total / 3; // Calculate percentage
    }

    // Function to print student information
    void display() {
        cout << "\nRoll Number: " << roll << endl;
        cout << "Name: " << name << endl;
        cout << "Total Marks: " << total << endl;
        cout << "Percentage: " << percentage << "%" << endl;
    }
};

int main() {
    Student s; // Create an instance of Student

    s.accept();    // Input student details
    s.calculate(); // Process total and percentage
    s.display();   // Show student details

    return 0;
}
