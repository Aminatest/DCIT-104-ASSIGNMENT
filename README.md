# DCIT-104-ASSIGNMENT// ABDUL-MAJEED AMINA 10965487
#include <iostream>
using namespace std;
int main(){
    bool isPrime;
    int i, j;
    int sum = 0;
    int num = 300; 

   for (i = 2; i < num; i++) {
      isPrime = true;

     for (int j = 2; j < i; j++) {
        if (i % j == 0) {
            isPrime = false;
        }
     }
     if (isPrime) {
        sum += i;
     }
   }
   cout << "The sum of the prime numbers less than 300 is: " <<sum <<endl;
}
