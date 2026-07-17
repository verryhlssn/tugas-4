#### **List :**



shoppingList = \['Milk', 'Cheese', 'Butter']



**input :**

for i in range(len(shoppingList)):

&#x20;   shoppingList\[i] = shoppingList\[i]+"+"

&#x20;   print(shoppingList\[i])

empty = \[]

for i in empty:

&#x20;   print("I am empty")



**output :**

Milk+

Cheese+

Butter+



**penjelasan :** Membuat list belanja dengan 3 item, lalu menelusuri setiap elemen menggunakan loop for dengan index. Menambahkan tanda "+" di akhir setiap string dan mencetak hasilnya (Milk+, Cheese+, Butter+). Jika Membuat list kosong lalu loop for tidak dieksekusi, itu karena tidak ada elemen (maka tidak ada output).





\# Update/Insert - List 



**input :** myList = \[1,2,3,4,5,6,7]

&#x09;print(myList)

**output :** \[1, 2, 3, 4, 5, 6, 7]

**penjelasan :** Membuat list angka 1-7 dan mencetaknya.





**input :** myList.insert(4,15)

&#x09;print(myList)

**output :** \[1, 2, 3, 4, 15, 5, 6, 7]

**penjelasan :** Menambahkan angka 15 pada indeks ke-4 (posisi 5 karena hitungan array dimulai dari 0), hasil: 1,2,3,4,15,5,6,7





**input :** myList.append(55)

&#x09;print(myList)

**output :** \[1, 2, 3, 4, 15, 5, 6, 7, 55]

**penjelasan :** Menambahkan 55 di akhir list, hasil: 1,2,3,4,15,5,6,7,55





**input :** newList = \[11,12,13,14]

&#x09;myList.extend(newList)

&#x09;print(myList)

**output :** \[1, 2, 3, 4, 15, 5, 6, 7, 55, 11, 12, 13, 14]

**penjelasan :** Membuat list baru \[11,12,13,14], lalu menambahkan semua elemennya ke akhir myList: 1,2,3,4,15,5,6,7,55,11,12,13,14





\#  Searching for an element in the List

**input :** 

myList =  \[10,20,30,40,50,60,70,80,90]



def searchinList(list, value):

&#x20;   for i in list:

&#x20;       if i == value:

&#x20;           return list.index(value)

&#x20;   return 'The value does not exist in the list'



print(myList)



**output :** \[10, 20, 30, 40, 50, 60, 70, 80, 90]

**penjelasan :** Mendefinisikan fungsi pencarian: menelusuri list, jika nilai ditemukan kembalikan indeks pertamanya menggunakan index(), jika tidak kembalikan pesan error.





**input :** print(searchinList(myList, 60))

**penjelasan :** Mencetak list, lalu hasil pencarian 60 (mengembalikan indeks 5).





\#List operations / functions

**input :**

total = 0 

count = 0

while (True):

&#x20;   inp = input('Enter a number: ') 

&#x20;   if inp == 'done': break

&#x20;   value = float(inp)

&#x20;   total = total + value

&#x20;   count = count + 1 

&#x20;   average = total / count

&#x09;				

print('Average:', average)



**output :** 

Enter a number: 1.5

Enter a number: 2.5

Enter a number: done

Average: 2.5

**penjelasan :** Loop while tak terbatas: meminta input angka, akhiri dengan 'done'. Menjumlahkan semua nilai ke 'total', hitung jumlah input di 'count', hitung rata-rata secara real-time. Cetak rata-rata akhir.





**input :**

numlist = list() 

while (True):

&#x20;   inp = input('Enter a number: ') 

&#x20;   if inp == 'done': break

&#x20;   value = float(inp)

&#x20;   numlist.append(value)

&#x09;				

average = sum(numlist) / len(numlist) 

print('Average:', average)



**output :**

Enter a number: 1.5

Enter a number: 2.5

Enter a number: done

Average: 2.5

**penjelasan :** Membuat list kosong 'numlist'. Input angka seperti sebelumnya, simpan ke list dengan 'append()'. Setelah selesai, hitung rata-rata menggunakan 'sum()' dan 'len()'.

