Pada laporan parktikum kali ini, Program yang dibuat adalah program sederhana yang meminta instruksi kepada pengguna untuk memasukkan umur, lalu menentukan kategori berdasarkan rentang umur tertentu. Program ini merujuk pada sebuah bioskop yang menerapkan pembatasan film atau tontonan berdasarkan umur penonton.  Jika umur penonton dibawah 13 tahun, maka dikategorikan SU (Semua umur), jika umurnya 17-20 tahun, maka dikategorikan D17, dan jika umurnya 21 atau lebih, maka dikategorikan D21.Program menggunakan operator if-else untuk memeriksa kondisi umur dan menampilkan output yang sesuai. Berikut adalah penjelasan detailnya:
**#include <iostream>** Ini adalah header file. Dalam program, ini harus disertakan untuk memungkinkan program agar dapat menggunakan fungsi input dan output standar, seperti cout (Untuk menampilkan output layar)	
**using namespace std;** Ini adalah deklarasi namespace.Ini memungkinkan program untuk menggunakan fungsi-fungsi standar tanpa harus menambahkan awalan std;	
****int main()** **Ini adalah fungsi utama dari program. Setiap program C++ harus memiliki fungsi main(), Karena ini adalah tempat eksekusi program dimulai.	
**{...}** Kurung kurawal ini mendefinisikan blok kode untuk fungsi main().
**int umur;** Ini mendeklarasikan variabel bernama umur dengan tipe data int (integer), yang digunakan untuk menyimpan nilai umur yang dimasukkan pengguna.
**cout << "Masukkan umur: ";** output yang berfungsi untuk menampilkan "Masukkan umur" ke layar.
**cin >> umur;** input yang berfungsi untuk membaca input dari keyboard.
**if (umur < 13)** Jika umur kurang dari 13, tampilkan "SU".
**else if (umur >= 13 && umur <= 16)** Jika umur antara 13 dan 16, tampilkan "R13". Operator && adalah logika AND, memastikan kedua kondisi benar.
**else if (umur >= 17 && umur <= 20)** Jika umur antara 17 dan 20, tampilkan "D17".
**else if (umur >= 21)** Jika umur 21 atau lebih, tampilkan "D21".
**cout << "SU" << endl;** Menampilkan kategori dan endl untuk pindah ke baris baru.
**return 0;** Mengakhiri program dan mengembalikan nilai 0 yang menunjukkan program berjalan.
Program ini mengelompokkan umur yang di input oleh pengguna kedalam kategori yang ditandai dengan kode ”SU”, ”R13”, ”D17”, dan ”D21” yang berdasarkan pada umur yang ditentukan. Program ini akan berjalan jika input nya sesuai dengan ketentuannya.
Contoh: 
	Input : 8  Output : SU
	Input : 15 Output : R13
	Input : 20 Output : D17
	Input : 25 Output : D21
