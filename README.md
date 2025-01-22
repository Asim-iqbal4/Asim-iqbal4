- 👋 Hi, I’m @Asim-iqbal4

Asim-iqbal4/Asim-iqbal4 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
------------------------Electricity bill calculator-----------------------------------------------------------------------#include <iostream>
using namespace std;

int main() {
    double units, bill = 0.0;

    cout << "Welcome to the Electricity Bill Calculator!\n";
    cout << "Enter the number of units consumed: ";
    cin >> units;

    if (units <= 100) {
        bill = units * 1.5; 
    } else if (units <= 200) {
        bill = (100 * 1.5) + ((units - 100) * 2.0); 
    } else if (units <= 300) {
        bill = (100 * 1.5) + (100 * 2.0) + ((units - 200) * 3.0);  
    } else {
        bill = (100 * 1.5) + (100 * 2.0) + (100 * 3.0) + ((units - 300) * 5.0); 
    }

    cout << "Your total electricity bill is: $" << bill << endl;
    cout << "Thank you for using the Electricity Bill Calculator!\n";

    return 0;
}
