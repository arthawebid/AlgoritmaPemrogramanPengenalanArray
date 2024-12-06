### **Materi Perkuliahan: Algoritma Pemrograman**

#### **1. Pengenalan Array Dimensi**
**Array** adalah struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel yang sama. Setiap elemen dalam array disimpan secara berurutan dalam memori dan diakses menggunakan indeks.

Tipe array berdasarkan jumlah dimensinya dibagi menjadi:
- **Array Satu Dimensi** (1D)
- **Array Dua Dimensi** (2D)
- **Array Tiga Dimensi** (3D)
- Dan seterusnya...

**Array 1 Dimensi** adalah array yang menyimpan elemen dalam bentuk garis lurus, misalnya daftar angka, nama, atau data lainnya. Array 1D dapat dianggap sebagai kumpulan data yang tersusun dalam satu baris.

#### **Contoh Array 1 Dimensi**:
Misalkan kita ingin menyimpan 5 angka dalam sebuah array.

```plaintext
int angka[5] = {2, 4, 6, 8, 10};
```

Di sini, `angka` adalah array dengan 5 elemen yang masing-masing berisi nilai 2, 4, 6, 8, dan 10. Setiap elemen dapat diakses melalui indeks.

#### **2. Indeks dan Value Array 1 Dimensi**
- **Indeks** adalah posisi elemen dalam array. Indeks array dimulai dari angka 0 (nol).
- **Value** adalah nilai yang disimpan pada suatu indeks dalam array.

Contoh:
```plaintext
angka[0] = 2     // Elemen pertama (indeks 0) bernilai 2
angka[1] = 4     // Elemen kedua (indeks 1) bernilai 4
angka[2] = 6     // Elemen ketiga (indeks 2) bernilai 6
angka[3] = 8     // Elemen keempat (indeks 3) bernilai 8
angka[4] = 10    // Elemen kelima (indeks 4) bernilai 10
```

**Catatan:**
- Indeks array **mulai dari 0** dan berlanjut hingga `n-1`, di mana `n` adalah jumlah elemen dalam array.
- **Value** adalah nilai yang disimpan di dalam array pada indeks tertentu.

#### **3. Mengakses & Mengisi Array Satu Dimensi**
- **Mengakses Array**: Untuk mengambil nilai dari array, kita cukup menggunakan indeks array yang diinginkan.

Contoh kode untuk mengakses nilai dalam array:
```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[5] = {2, 4, 6, 8, 10};
    
    // Mengakses elemen array dengan indeks
    cout << "Elemen pertama: " << angka[0] << endl;  // Output: 2
    cout << "Elemen kedua: " << angka[1] << endl;    // Output: 4
    cout << "Elemen ketiga: " << angka[2] << endl;   // Output: 6

    return 0;
}
```

- **Mengisi Array**: Untuk mengisi nilai ke dalam array, kita dapat langsung menetapkan nilai pada indeks tertentu atau menggunakan loop.

Contoh kode untuk mengisi array:
```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[5];
    
    // Mengisi array dengan nilai tertentu
    angka[0] = 5;
    angka[1] = 10;
    angka[2] = 15;
    angka[3] = 20;
    angka[4] = 25;
    
    // Menampilkan nilai array
    for (int i = 0; i < 5; i++) {
        cout << "angka[" << i << "] = " << angka[i] << endl;
    }

    return 0;
}
```

**Menggunakan Loop untuk Mengisi Array:**
Loop sering digunakan untuk mengisi array, terutama jika jumlah elemen sangat banyak.

```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[5];

    // Mengisi array menggunakan loop
    for (int i = 0; i < 5; i++) {
        angka[i] = (i + 1) * 5;  // Mengisi dengan kelipatan 5
    }

    // Menampilkan nilai array
    for (int i = 0; i < 5; i++) {
        cout << "angka[" << i << "] = " << angka[i] << endl;
    }

    return 0;
}
```

#### **4. Operasi Dasar pada Array 1 Dimensi**
Beberapa operasi dasar yang sering dilakukan pada array 1 dimensi:
- **Pengisian Nilai (Assignment)**: Menetapkan nilai ke elemen array.
- **Akses Nilai**: Mengambil nilai dari elemen array berdasarkan indeks.
- **Iterasi/Traversing**: Melakukan iterasi untuk mengakses setiap elemen array (sering menggunakan loop seperti `for` atau `while`).
- **Pencarian**: Mencari elemen tertentu dalam array.
- **Pengurutan**: Menyusun array berdasarkan urutan tertentu (misalnya ascending atau descending).
- **Penjumlahan dan Penghitungan**: Melakukan operasi aritmetika pada elemen-elemen array, seperti menjumlahkan semua elemen array.

Contoh program untuk menjumlahkan semua elemen array:
```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[5] = {2, 4, 6, 8, 10};
    int total = 0;
    
    // Menjumlahkan elemen array
    for (int i = 0; i < 5; i++) {
        total += angka[i];
    }

    cout << "Total nilai array: " << total << endl;

    return 0;
}
```

#### **5. Contoh Soal**
Buatlah sebuah program yang:
1. Mendeklarasikan array 1 dimensi dengan ukuran 6 elemen.
2. Mengisi array tersebut dengan angka 10, 20, 30, 40, 50, dan 60.
3. Mencetak elemen-elemen array tersebut satu per satu.
4. Menjumlahkan semua elemen dalam array dan menampilkan hasilnya.

**Jawaban:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int angka[6] = {10, 20, 30, 40, 50, 60};
    int total = 0;
    
    // Mencetak elemen array
    for (int i = 0; i < 6; i++) {
        cout << "angka[" << i << "] = " << angka[i] << endl;
        total += angka[i];
    }

    cout << "Total nilai array: " << total << endl;

    return 0;
}
```

---

### **Kesimpulan:**
- Array 1 dimensi adalah struktur data yang memungkinkan kita menyimpan beberapa nilai dalam satu variabel.
- Elemen-elemen array diakses menggunakan indeks yang dimulai dari 0.
- Kita dapat mengakses dan mengisi nilai array baik secara langsung maupun menggunakan loop.

Semoga materi ini membantu dalam pemahaman tentang array satu dimensi!
