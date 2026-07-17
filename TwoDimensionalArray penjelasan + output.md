#### **TwoDimensionalArray :**



**input :** import numpy as np

**penjelasan :** Mengimpor pustaka NumPy dengan alias "np" untuk operasi array efisien.





**input :** twoDArray = np.array(\[\[11, 15, 10, 6], \[10, 14, 11, 5], \[12, 17, 12, 8], \[15, 18, 14, 9] ])

print(twoDArray)

**output :**

\[\[11 15 10  6]

&#x20;\[10 14 11  5]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]]

**penjelasan :** Membuat array 2D berukuran 4x4 dari list of lists, lalu mencetaknya





**input :** newTwoDArray = np.insert(twoDArray, 1, \[\[1,2,3,4]], axis=0)

print(newTwoDArray)

**output :** 

\[\[11 15 10  6]

&#x20;\[ 1  2  3  4]

&#x20;\[10 14 11  5]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]]

**penjelasan :** Menambahkan baris \[1,2,3,4] pada posisi indeks 1 (baris kedua) dengan axis-0 (arah baris), menghasilkan array 5x4.





**input :** print(len(twoDArray))

**output :** 4

**penjelasan :** Mencetak jumlah baris array twoDArray (4). 





**input :** newTwoDArray = np.append(twoDArray, \[\[1,2,3,4]], axis=0)

print(newTwoDArray)

**output :**

\[\[11 15 10  6]

&#x20;\[10 14 11  5]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]

&#x20;\[ 1  2  3  4]]

**penjelasan :** Menambahkan baris \[1,2,3,4] di akhir array asli, menghasilkan array 5x4 baru.





**input :** print(len(newTwoDArray)) **output :** 5

**input :** print(len(newTwoDArray\[0])) **output :** 4

**penjelasan :** Mencetak jumlah baris (5) dan kolom (4) dari newTwoDArray.





**input :** def accessElements(array, rowIndex, colIndex):

&#x20;   if rowIndex >= len(array) or colIndex >= len(array\[0]):

&#x20;       print('Incorrect Index')

&#x20;   else:

&#x20;       print(array\[rowIndex]\[colIndex])



**penjelasan :** Mendefinisikan fungsi untuk mengakses elemen di baris rowIndex dan kolom colIndex, dengan pengecekan batas array.





**input :** accessElements(newTwoDArray, 3, 1)

**output :** 18

**penjelasan :** Memanggil fungsi untuk mengakses elemen di baris 3. kolom 1 (hasil: 18)





**input :** def traverseTDArray(array):

&#x20;   for i in range(len(array)):

&#x20;       for j in range(len(array\[0])):

&#x20;           print(array\[i]\[j])



**penjelasan :** Mendefinisikan fungsi untuk mencetak semua elemen array secara berurutan menggunakan nested loop.



**input :** traverseTDArray(twoDArray)

**output :**

11

15

10

6

10

14

11

5

12

17

12

8

15

18

14

9

**penjelasan :** Memanggil fungsi untuk mencetak semua elemen twoDArray.





**input :** def searchTDArray(array, value):

&#x20;   for i in range(len(array)):

&#x20;       for j in range(len(array\[0])):

&#x20;           if array\[i]\[j] == value:

&#x20;               return 'The value is located index '+str(i)+" "+str(j)

&#x20;   return 'The element no found'



**penjelasan :** Mendefinisikan fungsi pencarian nilai value di "array" mengembalikan posisi jika ditemukan, atau pesan error.





**input :** print(twoDArray)

**output :**

\[\[11 15 10  6]

&#x20;\[10 14 11  5]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]]

**penjelasan :** Mencetak array asli (tidak berubah karena twoDArray tetap utuh).



**input :** print(searchTDArray(twoDArray, 11))

**output :** The value is located index 0 0

**penjelasan :** Mencetak array lalu hasil pencarian nilai 11 (ditemukan di indeks ).





**input :** newTDArray = np.delete(twoDArray, 1, axis=0)

&#x09;print(newTDArray)

**output :** 

\[\[11 15 10  6]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]]

**penjelasan :** Menghapus baris pada indeks 1 dari twoDArray, menghasilkan array 3x4 baru.





**input :** print(twoDArray)

**output :**

\[\[11 15 10  6]

&#x20;\[10 14 11  5]

&#x20;\[12 17 12  8]

&#x20;\[15 18 14  9]]

**penjelasan :** Mencetak array asli (tidak berubah karena twoDArray tetap utuh).

