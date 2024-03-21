#include <iostream>

using namespace std;

int main() {
    double a, b, k, m;

    cout << "Enter the values of a, b, k, m for the lines y=ax+b and y=kx+m: ";
    cin >> a >> b >> k >> m;

    if (a == k) {
        cout << "The lines are parallel and do not intersect." << endl;
    } else {
        double x = (m - b) / (a - k);
        double y = a * x + b;
        cout << "The lines intersect at the point (" << x << ", " << y << ")." << endl;
    }

    return 0;
}
