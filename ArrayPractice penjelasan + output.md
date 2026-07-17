#### **ArrayPractice**



1\. Create an array and traverse

Input :

from array import array

my\_array = array('i',\[1,2,3,4,5])

for i in my\_array:

print(i)



Output : 

1

2

3

4

5



Penjelasan :

\- from array import array = lmport

modul eksternal array

\- my\_array = array('i',\[1,2,3,4,5]) =

Membuat array integer dengan 5 elemen

\- for 'i' in my\_array:= TRAVERSE

(menelusuri setiap elemen)

\- print(i) = Print setiap elemen



2\. Access individual elements through indexes

&#x20;Input : 

print("Step 2") 

print(my\_array\[3])

Output : 

Step 2

4

Penjelasan :

\- Print label "step 2"

\- Akses elemen di index 3 (ke-4 elemen, array mulai dari 0)



3\. Append any value to the array using append() method 

Input : 

print("Step 3") 

my\_array.append(6)

print(my\_array)



Output :

Step 3

array('i', \[1, 2, 3, 4, 5, 6])



Penjelasan :

\- Print label "step 3"

\- Tambah elemen 6 di akhir array

\- Print seluruh array termasuk yang sudah ditambah



4\. Insert value in an array using insert() method

Input :

print("Step 4") 

my\_array.insert(3, 11) 

print(my\_array)

Output :

Step 4

array('i', \[1, 2, 3, 11, 4, 5, 6])

Penjelasan :

\- print label "step 4"

\- sisipkan 11 di index 3, elemen digeser ke kanan

\- print seluruh array termasuk perubahan hasil sisipan tadi/hasil insert



5\. Extend python array using extend() method

Input :

print("Step 5") 

my\_array1 = array('i', \[10,11,12]) my\_array.extend(my\_array1) 

print(my\_array)



Output :

Step 5

array('i', \[1, 2, 3, 11, 4, 5, 6, 10, 11, 12])

Penjelasan :

\- print label "step 5"

\- buat array baru \[10,11,12]

\- menggabungkan my\_array1 ke my\_array

\- print seluruh array + array hasil extend



6\. Add items from list into array using fromlist() method 

Input :

print("Step 6") 

tempList = \[20,21,22] 

my\_array.fromlist(tempList)

print(my\_array)

Output :

Step 6

array('i', \[1, 2, 3, 11, 4, 5, 6, 10, 11, 12, 20, 21, 22])

Penjelasan :

\- print label "step 6"

\- buat list python biasa \[20,21,22]

\- tambahkan semua elemen list ke array

\- print array hasil fromlist



7\. Remove any array element using remove() method

Input :

print("Step 7") 

my\_array.remove(11) 

print(my\_array)

Output :

Step 7

array('i', \[1, 2, 3, 11, 4, 5, 6, 10,12, 20, 21, 22])

Penjelasan :

\- print label "step 7"

\- menghapus kemunculan pertama nilai 11 (pada index 3)

\- print array hasil remove



8\. Remove last array element using pop() method

Input :

print("Step 8") 

my\_array.pop()

print(my\_array)

Output :

Step 8

array('i', \[1, 2, 3, 11, 4, 5, 6, 10, 12, 20, 21])

Penjelasan :

\- print label "step 8"

\- hapus \& return elemen terakhir

\- print array hasil pop()



9\. Fetch any element through its index using index() method

Input :

print("Step 9")

print(my\_array.index(21))

Output :

Step 9

10

Penjelasan :

\- print label "step 9"

\- return index pertama elemen 21



10\. Reverse a python array using reverse() method

Input :

print("Step 10") 

my\_array.reverse() 

print(my\_array)

Output :

Step 10

array('i', \[21, 20, 12, 10, 6, 5, 4, 11, 3, 2, 1])

Penjelasan :

\- print label "step 10"

\- membalik urutan elemen array

\- print array hasil reverse array



11\. Get array buffer information through buffer\_info() method

Input :

print("Step 11") 

print(my\_array.buffer\_info())

Output :

Step 11

(140000000000000, 11)

Penjelasan :

\- print label "step 11"

\- return tuple (alamat\_memory, length)

12\. Check for number of occurrences of an element using count() method

Input :

print("Step 12") 

my\_array.append(11) 

print(my\_array.count(11)) 

print(my\_array)

Output :

Step 12

2

array('i', \[21, 20, 12, 10, 6, 5, 4, 11, 3, 2, 1, 11])

Penjelasan :

\- print label "step 12"

\- tambahkan "11" lagi

\- hitung berapa kali "11" muncul

\- print array



13\. Convert array to string using tostring() method

Input : 

print("Step 13") 

strTemp = my\_array.tostring() 

print(strTemp) 

ints = array('i') 

ints.fromstring(strTemp) 

print(ints)

Output :

Step 13

b'UP ...'

array('i', \[21, 20, 12, 10, 6, 5, 4, 11, 3, 2, 1, 11])

Penjelasan :

\- print label "step 13"

\- konversi array ke bytes object

\- print bytes

\- buat array kosong

\- restore array dari bytes

\- print array hasil restore



14\. Convert array to a python list with same elements using tolist() method

Input :

print("Step 14") 

print(my\_array.tolist())

Output :

Step 14

\[21, 20, 12, 10, 6, 5, 4, 11, 3, 2, 1, 11]

Penjelasan :

\- print label "step 14"

\- konversi array ke python list



15\. Append a string to char array using fromstring() method

Input : (contoh)

print("Step 15")

char\_array = array('c', b'Hello')

char\_array.fromstring(b' World!')  

print(char\_array)



Output :

Step 15

array('b', b'Hello World!')

Penjelasan :

\- print label "step 15"

\- buat char array tipe 'c' 

\- tambah string bytes

\- print char array



16\. Slice Elements from an array



Input : 

print("Step 16")

print(my\_array\[:])

Output : 

Step 16

array('i', \[21, 20, 12, 10, 6, 5, 4, 11, 3, 2, 1, 11])

Penjelasan : 

\- print label "step 16"

\- slice komplet (copy semua elemen)

