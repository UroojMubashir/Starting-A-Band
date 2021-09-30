#include <iostream>
#include <string>
using namespace std;

int main();

bool musical_friend(string n){
	if (n == "no") {
		return false;
	}
	else {
		return true;
	}
}
void join_band(string n) {
	if (musical_friend(n) == false) {
		cout << "Sorry ! you cannot join the band\n";
	}
	else {
		cout << "What instrument you can play?:\n";
		string instrument;
		cin >> instrument;
		if (instrument == "drum" || instrument == "guitar") {
			cout << "Welcome! to the band.\n";
		}
		else {
			cout << "Sorry! You cannot join the band \n.";
		}
	}
}
int main() {
	cout << "Do You have a musical friend ?:\n ";
	string n;
	cin >> n;
	join_band(n);
}
