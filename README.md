#include <iostream>
#include <cmath>
using namespace std;

int main() {

string user, pass;

for (int c = 0; c <= 3; ){
cout << "Enter Username :";
cin >> user;
cout << "Enter Password :";
cin >> pass;
if (user == "oka" && pass == "oka123" ){
  cout << "Access has granted\n";
  float x0, y0, x1, y1, x2, y2, area;
  cout << "Enter coefficients x0, y0, x1, y1, x2, and y2: ";
  cin >> x0 >> y0 >> x1 >> y1 >> x2 >> y2;
  
  area = abs(x0*(y1-y2)+x1*(y2-y0)+x2*(y0-y1))/2;
 
  cout<<"Area of triangle is : " << area;
  return 0;
}
else if (user != "oka" || pass != "oka123"){
  cout << "you only have "<< 3-c << "chance left\n"; 
  c++;
}
}
 cout << "Access has restricted";
 exit (0);
}

