# project6
#include<iostream>
using namespace std;
int main() {
	int lectureNumber;//kullanıcıdan alınacak ders sayısı
	float sumofNotes = 0;//notların toplamın saklamak için
	float note;//her bir ders için girilecek not
	cout << "how many lectures note you will enter?:";
	cin >> lectureNumber;
	//kullanıcıdan notları alma
	for (int i = 1; i <= lectureNumber; i++) {
		cout << "enter " << i << ".lecture note:";
		cin >> note;
		sumofNotes += note;
	}
	//ortalama hesaplama
	float average = sumofNotes / lectureNumber;
	//sonuçlrı ekrna yazdırma
	cout << "average of notes:" << average << endl;
	//basarı durumu belirtme
	if (average >= 50) {
		cout << "congratulations,you passed!" << endl;
	}
	else {
		cout << "unfortunatelly,you failed!" << endl;
	}
}
