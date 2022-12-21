## Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Dzakwan Faiq Nauval
<br>NIM		:	1227050039
<br>Jurusan		: Teknik Informatika UIN Sunan Gunung Djati Bandung 

## Deskripsi Umum

## Source Code
#include <iostream>
#include <conio.h>
using namespace std;

int main() {
	int a_baris, b_kolom, i, j, res;
	
	cout << "Menentukan bilangan yang tidak habis jika dibagi dengan 3,5,7"<<endl;
	cout << "Nama:\tDzakwan Faiq Nauval"<<endl;
	cout << "NIM :\t1227050039"<<endl;
	cout << "-------------------------------------------------------------"<<endl;
	
	cout << "Masukkan banyak baris: "; cin >> a_baris;
	cout << "Masukkan banyak kolom: "; cin >> b_kolom;
	cout << endl;
	
	int angka[a_baris][b_kolom];
	
	// input
	for (i = 1; i <= a_baris; i++) {
		for (j = 1; j <= b_kolom; j++) {
			cout << "Nilai Baris " << i << " Kolom " << j << " = ";
			cin >> angka[i][j];
		}
	}
	cout << endl;
	
	// proses perhitungan
	for (i = 1; i <= a_baris; i++) {
		for (j = 1; j <= b_kolom; j++) {
			if (angka[i][j] % 3 != 0 && angka[i][j] % 5 != 0 && angka[i][j] % 7 != 0) {
				cout << "Bilangan yang tidak habis jika dibagi dengan 3,5,7 = " << angka[i][j] << endl;
			} 
		}
	}
	getch();
}
## Output
- Soal No.1
 <img width="597" alt="Screenshot_20221221_001655" src="https://user-images.githubusercontent.com/121118106/208793694-f979ac9a-802b-40b1-b377-913b2fd4191a.png">

- Soal No.2 
 <img width="598" alt="Screenshot 2022-12-21 002005" src="https://user-images.githubusercontent.com/121118106/208793791-29a21e2c-c76d-4f4e-8ab6-a064b7d327ef.png">


