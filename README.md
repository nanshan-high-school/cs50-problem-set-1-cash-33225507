# cs50-problem-set-1-cash-33225507
cs50-problem-set-1-cash-33225507 created by GitHub Classroom
#include <iostream>
using namespace std;
int main() {
    int a = 1;
    int b = 5;
    int c = 10;
    int d = 50;
    int price;
    cout << "請輸入價錢:";
    cin >> price;
    cout << "您需要" << price / 50 
         << "個50元硬幣\n還需要" << price % 50 / 10 
         << "個10元硬幣\n還需要" << price % 50 % 10 / 5 
         << "個5元硬幣\n還需要" << price % 50 % 10 % 5 
         << "個1元硬幣\n";
    cout << "最少要" 
         << price / 50 + price % 50 / 10 + price % 50 % 10 / 5 + price % 50 % 10 % 5 
         << "個硬幣";
}
