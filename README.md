# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Fakhruddin AL Farrosy
<br>NIM		:	1227050088
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
  Matriks transpose adalah sebuah matriks yang dihasilkan dari menukar baris dan kolom dari matriks asli. Misalnya, jika matriks asli memiliki ukuran M x N, maka matriks transpose-nya akan memiliki ukuran N x M.

  Untuk menghitung matriks transpose pada C++, kita dapat menggunakan perulangan for untuk mengakses setiap elemen dari matriks asli satu per satu dan menyimpannya pada matriks transpose dengan indeks yang sesuai.
  
## Source Code

#include <iostream>
using namespace std;

const int MAX_SIZE = 100;

int main() {
  // Membuat matriks dengan ukuran m x n
  int m, n;
  cout << "================================================\n";
  cout << "Masukkan ukuran matriks (m x n): ";
  cin >> m >> n;
  cout << "================================================\n";

  int matriks[MAX_SIZE][MAX_SIZE];

  // Menginputkan nilai ke dalam matriks
  cout << "Masukkan elemen matriks:" << endl;
  for (int i = 0; i < m; i++) {
    for (int j = 0; j < n; j++) {
      cin >> matriks[i][j];
    }
  }

  // Menampilkan matriks transpose
  cout << "Matriks transpose:" << endl;
  for (int i = 0; i < n; i++) {
    for (int j = 0; j < m; j++) {
      cout << matriks[j][i] << " ";
    }
    cout << endl;
  }

  return 0;
}

## Output
  ![image](https://user-images.githubusercontent.com/105347617/208528243-5917f1ce-bdb8-4b56-9bcb-a1c29a6ea989.png)
kita membuat matriks asli dengan ukuran M x N dan menginputkan nilai ke dalam matriks tersebut. Kemudian, kita membuat matriks transpose dengan ukuran N x M dan menghitung matriks transpose dengan menukar indeks baris dan kolom dari matriks asli. Setelah itu, kita dapat menampilkan matriks transpose dengan menggunakan perulangan for.
