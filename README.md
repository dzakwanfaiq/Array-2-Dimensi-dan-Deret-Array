## Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Dzakwan Faiq Nauval
<br>NIM			: 1227050039
<br>Jurusan		: Teknik Informatika UIN Sunan Gunung Djati Bandung 

## Deskripsi Umum
Pada program kali ini penulis membuat 2 buah program yang mana program ini memiliki fungsi tersendiri.

Program pertama, program ini dibuat menggunakan konsep Array 2 Dimensi yang mana program pertama memiliki fungsi untuk melakukan pertukaran elemen baris menjadi kolom dan elemen kolom menjadi baris.
langkah awalnya yaitu penulis menginputkan banyak baris dan kolom pada matriks, lalu input nilai pada matriks, kemudian data yang telah diinput akan ditampilkan sesusai dengan konsep matriks, lalu ditampilkan juga hasil matriks setelah ditranspose.  

Program kedua, program ini dibuat untuk menentukan suatu bilangan yang tidak habis bisa jika dibagi dengan angka 3,5, dan 7.
Langkah awalnya yaitu penulis menginputkan berapa banyak baris dan kolom pada matriks, lalu input nilai pada pada matriks, setelah itu data yang telah diinputkan akan dipilih secara otomatis mana bilangan yang tidak habis jika dibagi dengan 3,5, dan 7. lalu akan ditampilkan bilangan yang tidak habis dibagi 3,5, dan 7. Namun, apabila nilai habis jika dibagi dengan 3,5, dan 7 maka tidak akan ditampilkan.
## Source Code
- Source Code Soal No.1

#include <iostream>
#include <conio.h>
using namespace std;

int main(){
	int a_baris, b_kolom, i, j;
	int matriks[10][10];
	int transpose[10][10];

	cout << "Mengubah Baris menjadi Kolom"<<endl;
	cout << "Nama:\tDzakwan Faiq Nauval"<<endl;
	cout << "NIM :\t1227050039"<<endl;
	cout << "------------------------------"<<endl;
	
	cout << "Masukkan banyak baris matriks: ";
	cin >> a_baris;
	cout << "Masukkan banyak kolom matriks: ";
	cin >> b_kolom;
	cout << endl;
	
	// input 
	for (i = 0; i < a_baris; i++) {
		for (j = 0; j < b_kolom; j++) {
    		cout << "Nilai Matriks Baris " << i+1 << " Kolom " << j+1 << " = " ;
	  		cin  >> matriks[i][j];
    	}
	}
	cout << endl;

	// proses perhitungan
	cout << "Matriks Awal: "<<endl;
	for (i = 0; i < a_baris; i++){
		for (j = 0; j < b_kolom; j++){
			cout << matriks[i][j] << "\t";
    	}
    		cout << endl;
	}
  
	for (i = 0; i < a_baris; i++){
		for (j = 0; j < b_kolom; j++){
    		transpose[j][i] = matriks[i][j];
    	}
	}
	
	// output
	cout << "Hasil setelah Matriks diTranspose: "<<endl;
	for (i = 0; i < b_kolom; i++){
		for (j = 0; j < a_baris; j++){
      		cout << transpose[i][j] << "\t";
    	}
    	cout << endl;
	}
	getch();
}
- Source Code Soal No.2

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


