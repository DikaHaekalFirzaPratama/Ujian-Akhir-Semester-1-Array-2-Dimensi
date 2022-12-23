# Ujian Akhir Semester 
<br>Mata Kuliah : Dasar Pemrograman 
<br>Nama	      : Dika Haekal Firza Pratama
<br>NIM		      :	1227050036
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Tema utama dari source code yang satu ini adalah untuk membuat array 2 dimensi menggunakan bahasa C++.
Tujuan utama dari source code ini adalah mengubah letak nilai yang tadinya sebuah baris menjadi sebuah kolom, begitupun sebaliknya.
Algoritma dari Source code ini yaitu :

1. User menginputkan berapa banyak baris pada array.
2. User menginputkan berapa banyak kolom dari baris pada array.
3. User menginputkan satu persatu nilai array,dimulai dari baris 1 dan kolom 1.
4. Jika sudah,Nilai dalam array tersebut di tampilkan sesuai aturan matriks.
5. Lalu ditampilkan juga nilai dalam array yang sudah dibalik,dari baris menjadi kolom dan sebaliknya.

## Source Code
	#include <iostream>
	using namespace std;
	void garis(){
	cout << "=======================================" << endl;}
	int main(){
	garis();
	int input [100][100];
	int baris, kolom, i, j;
	
	cout << "Imputkan berapa banyak baris yang ingin di imputkan : ";
	cin >> baris;
	cout << "Imputkan berapa banyak kolom yang ingin di imputkan : ";
	cin >> kolom;
	
	garis();
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << "baris ke-" << i+1 << " kolom ke-" << j+1 << " = ";
			cin >> input[i][j];
		}
	garis();
	}
	
	cout << "Hasil : " << endl;
	garis();
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << " " << input [i][j];
		}
		cout << endl;
	}
	garis();
	
	for (i = 0; i < kolom; i++){
		for (j = 0; j < baris; j++){
			cout << " " << input[j][i];
		}
		cout << endl;
	}
	garis();
	
	return 0;
	}
  
## Output
![Uas 2 dimensi](https://user-images.githubusercontent.com/121142632/209268979-b7ed709e-6988-4634-b961-9524640318c1.png)
