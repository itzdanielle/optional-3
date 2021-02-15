# optional-3
#include <iostream>
#include <cmath>
using namespace std;

int main() {
 double a, b, c;

cout << "Enter the value of a: " << endl;
cin >> a;
cout << "Enter the value of b: " << endl;
cin >> b;
cout << "Enter the value of c: " << endl;
cin >> c;

double discriminant = (pow( b , 2 ) - 4 * a * c);
double positiveRoot = ((( -b ) + sqrt( discriminant )) / ( 2 * a ));
double negativeRoot = ((( -b ) - sqrt(discriminant)) / ( 2 * a ));

if (discriminant == 0) {
  cout << "The discriminant is " << discriminant << endl;
  cout << "The equation has one root" << endl;
}

else if (discriminant < 0) {
  cout << "The discriminant is " << discriminant << endl;
  cout << "The equation has two complex roots" << endl;
}
else if (discriminant > 0) {
  cout << "The discriminant is " << discriminant << endl;
  cout << "The eqaution has two real roots" << endl;
}

cout << "The roots of the quadratic equation are x= " << negativeRoot << ", " << positiveRoot << endl;

}
