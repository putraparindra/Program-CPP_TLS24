Nyquist Alfito Putra Parindra

3.1.1 DEKLARASI MATRIKS
cpp
int matriks_A[2][2], matriks_B[2][2], hasil[2][2];

Matriks A dan B: matriks_A dan matriks_B dideklarasikan sebagai array 2 dimensi dengan ukuran 2x2. Masing-masing elemen dalam array ini dapat diakses menggunakan indeks baris dan kolom (misalnya, matriks_A untuk elemen pertama baris pertama).
Hasil Penjumlahan: hasil juga dideklarasikan sebagai array 2 dimensi dengan ukuran 2x2 untuk menyimpan hasil penjumlahan matriks A dan B.

3.1.2 INPUT ELEMEN MATRIKS
cpp
// Input elemen matriks A
cout << "Masukkan elemen matriks A:" << endl;
for (int i = 0; i < 2; i++) {
    		for (int j = 0; j < 2; j++) {
        			cout << "Baris " << i + 1 << ", Kolom " << j + 1 << ": ";
        			cin >> matriks_A[i][j];
    		}
}

// Input elemen matriks B
cout << "\nMasukkan elemen matriks B:" << endl;
for (int i = 0; i < 2; i++) {
    		for (int j = 0; j < 2; j++) {
        			cout << "Baris " << i + 1 << ", Kolom " << j + 1 << ": ";
        			cin >> matriks_B[i][j];
    		}
}

Perulangan Bersarang: digunakan untuk meminta pengguna memasukkan elemen-elemen matriks A dan B secara berurutan. Perulangan ini terdiri dari dua loop: satu loop luar (i) yang mengontrol baris dan satu loop dalam (j) yang mengontrol kolom.
Output Prompt: program menampilkan prompt untuk memasukkan elemen-elemen matriks A dan B, dengan label baris dan kolom yang jelas.

3.1.3 PENJUMLAHAN MATRIKS
cpp
// Penjumlahan matriks A dan B
for (int i = 0; i < 2; i++) {
    		for (int j = 0; j < 2; j++) {
    		    hasil[i][j] = matriks_A[i][j] + matriks_B[i][j];
    		}
}

Perulangan Bersarang: digunakan untuk melakukan penjumlahan elemen-elemen matriks A dan B secara berurutan. Perulangan ini sama seperti saat input elemen matriks.
Penjumlahan Elemen: setiap elemen hasil (hasil[i][j]) dihitung sebagai penjumlahan dari elemen yang sama pada matriks A dan B (matriks_A[i][j] + matriks_B[i][j]).

3.1.4 HASIL YANG DITAMPILKAN
cpp
// Tampilkan hasil penjumlahan
cout << "\nHasil Penjumlahan Matriks A dan B:" << endl;
for (int i = 0; i < 2; i++) {
    		for (int j = 0; j < 2; j++) {
        		cout << hasil[i][j] << " ";
    	}
    	cout << endl;
}

Perulangan Bersarang: digunakan untuk menampilkan hasil penjumlahan matriks A dan B secara berurutan.
Output Hasil: program menampilkan hasil penjumlahan matriks A dan B dengan format yang jelas.
