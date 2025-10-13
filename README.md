#include <iostream>
using namespace std;

// Class template definition
template <class T1, class T2>
class Pair {
    T1 first;
    T2 second;

public:
    // Constructor
    Pair(T1 a, T2 b) {
        first = a;
        second = b;
    }

    // Function to display the values
    void display() {
        cout << "First: " << first << ", Second: " << second << endl;
    }
};

// Main function
int main() {
    // Create objects with different data types
    Pair<int, double> p1(10, 3.14);
    Pair<string, int> p2("Karthik", 25);

    // Display results
    p1.display();
    p2.display();

    return 0;
}
