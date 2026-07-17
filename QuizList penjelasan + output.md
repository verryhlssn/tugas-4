#### **QuizList :**



\# Q-1. What will be the output of the following code block?

**input \& penjelasan :**

a=\[1,2,3,4,5,6,7,8,9] **# list dengan 9 elemen, index dari 0-8**

print(a\[::2]) **# slice start=0, stop=akhir, step=2 -> ambil elemen ke-0,2,4,6,8**



**jawaban \& output :** 1,3,5,7,9





\# Q-2. What will be the output of the following code snippet?

**input \& penjelasan :**

a=\[1,2,3,4,5,6,7,8,9] **# 9 elemen**

a\[::2]=10,20,30,40,50,60 **# slice ::2 butuh 5 elemen (index 0,2,4,6,8)**

print(a) **# gagal/tidak dieksekusi (karena tuple sebelah kanan punya 6 elemen -> ERROR!)**

\# A. ValueError: attempt to assign sequence of size 6 to extended slice of size 5

\# B. \[10, 2, 20, 4, 30, 6, 40, 8, 50, 60]

\# C. \[1, 2, 10, 20, 30, 40, 50, 60]

\# D. \[1, 10, 3, 20, 5, 30, 7, 40, 9, 50, 60]



**jawaban \& output :** A. ValueError: attempt to assign sequence of size 6 to extended slice of size 5





&#x20;

\# Q-3. What will be the output of the following code snippet?

**input \& penjelasan :**

a=\[1,2,3,4,5] **# index : 0=1, 1=2, 2=3, 3=4, 4=5**

print(a\[3:0:-1]) **# start index 3(4), stop sebelum 0, step=-1**

**# jalur: index 3->4, 2->3, 1->2 (stop sebelum 0)**

&#x20;

\# A. Syntax error

\# B. \[4, 3, 2]

\# C. \[4, 3]

\# D. \[4, 3, 2, 1]



**jawaban \& output :** B. \[4,3,2]



&#x20;



\# Q-4. What will be the output of the following code snippet?

**input \& penjelasan :**

def f(value, values): **# value=int (immutable), values=list (mutable)**

&#x20;   v = 1 **# v lokal di fungsi**

&#x20;   values\[0] = 44 **# list mutable -> perubahan permanen!**

t = 3 **# t tetap 3 (int immutable)**

v = \[1, 2, 3] **# v global = list**

f(t, v) **# panggil fungsi**

print(t, v\[0]) **# print output**

\# A. 1 44

\# B. 3 1

\# C. 3 44

\# D. 1 1



**jawaban \& output :** C. 3 44

&#x20;



\# Q-5. What is the correct command to shuffle the following list?

**input \& penjelasan :**

fruit=\['apple', 'banana', 'papaya', 'cherry'] **# list buah** 

**# random.shuffle(fruit) shuffle list secara in-place. Perlu import random dulu.**

\# A. fruit.shuffle()

\# B. shuffle(fruit)

\# C. random.shuffle(fruit)

\# D. random.shuffleList(fruit)



**jawaban \& output :** # C. random.shuffle(fruit)





\# Q-6. What will be the output of the following code snippet?

**input \& penjelasan :**

data = \[\[\[1, 2], \[3, 4]], \[\[5, 6], \[7, 8]]] **# list bersarang (nested list)**

def fun(m): **# fungsi dengan parameter m**

&#x20;   v = m\[0]\[0] **# ambil elemen pertama**

&#x20;   for row in m: **# loop tiap sub-list**

&#x20;       for element in row: **# loop tiap elemen di dalam sub-list**

&#x20;           if v < element: **# jika bertemu nilai lebih besar**

&#x20;               v = element **#** **update v jadi nilai terbesar**

&#x20;   return v **# return nilai terbesar yang ditemukan**

print(fun(data\[0])) **# Output: 4 (max di \[\[1,2],\[3,4]])**

\# A. 1

\# B. 2

\# C. 3 

\# D. 4

\# E. 5

\# F. 6



**jawaban \& output :** D. 4

&#x20;



\# Q-7. What will be the output of the following code snippet?

**input \& penjelasan :** 

arr = \[\[1, 2, 3, 4], **# Baris 0: elemen terakhir = 4**

&#x20;      \[4, 5, 6, 7]**, # Baris 1: elemen terakhir = 7**  

&#x20;      \[8, 9, 10, 11], **# Baris 2: elemen terakhir = 11**

&#x20;      \[12, 13, 14, 15]] **# Baris 3: elemen terakhir = 15**

for i in range(0, 4): **# i = 0, 1, 2, 3 (4 iterasi)**

&#x20;   print(arr\[i].pop()) **# pop() hapus \& kembalikan elemen terakhir**

\# A. 1 2 3 4

\# B. 1 4 8 12

\# C. 4 7 11 15 

\# D. 12,13,14,15



**jawaban \& output :** C. 4 7 11 15

&#x20;



\# Q-8. What will be the output of the following code snippet?

**input \& penjelasan :**

def f(i, values = \[]): **# trap! Mutable default argument → satu list sama untuk semua panggilan!**

&#x20;   values.append(i) **# Tambah i ke list yang sama**

&#x20;   print(values) **# Print list saat ini**

&#x20;   return values



f(1) **# values=\[] → append(1) → print(\[1])**

f(2) **# values=\[1] → append(2) → print(\[1,2])**  

f(3) **# values=\[1,2] → append(3) → print(\[1,2,3])**

\# A. \[1] \[2] \[3]

\# B. \[1, 2, 3]

\# C. \[1] \[1, 2] \[1, 2, 3]

\# D. 1 2 3



**jawaban \& output :** C. \[1] \[1, 2] \[1, 2, 3]

&#x20;



\# Q-9. What will be the output of the following code snippet?

**input \& penjelasan :**

arr = \[1, 2, 3, 4, 5, 6] **# Awal: \[1,2,3,4,5,6]**

for i in range(1, 6): **# i=1,2,3,4,5**

&#x20;   arr\[i - 1] = arr\[i] **# geser kiri (1 posisi)**

for i in range(0, 6): **# Step-by-step:**

**i=1: arr\[0] = arr\[1] → \[2,2,3,4,5,6]**

**i=2: arr\[1] = arr\[2] → \[2,3,3,4,5,6]**

**i=3: arr\[2] = arr\[3] → \[2,3,4,4,5,6]**

**i=4: arr\[3] = arr\[4] → \[2,3,4,5,5,6]**

**i=5: arr\[4] = arr\[5] → \[2,3,4,5,6,6]**

&#x20;   print(arr\[i], end = " ") **# 2 3 4 5 6 6**

\# A. 1 2 3 4 5 6

\# B. 2 3 4 5 6 1

\# C. 1 1 2 3 4 5 

\# D. 2 3 4 5 6 6



**jawaban \& output :** D. 2 3 4 5 6 6

&#x20;



\# Q-10. What will be the output of the following code snippet?

**input \& penjelasan :**

fruit\_list1 = \['Apple', 'Berry', 'Cherry', 'Papaya'] **# List asli**

fruit\_list2 = fruit\_list1 **# Reference sama (bukan copy!)**

fruit\_list3 = fruit\_list1\[:] **# Shallow copy (independen)**



fruit\_list2\[0] = 'Guava' **# Ubah list2 → list1 juga berubah!**

**# Sekarang: list1 = list2 = \['Guava','Berry','Cherry','Papaya']**

**# list3 tetap = \['Apple','Berry','Cherry','Papaya']**



fruit\_list3\[1] = 'Kiwi' **# Ubah list3 saja**

**# list3 = \['Apple','Kiwi','Cherry','Papaya']**



sum = 0

for ls in (fruit\_list1, fruit\_list2, fruit\_list3):

&#x20;   if ls\[0] == 'Guava': # **list1\[0]='Guava'  (+1)**

&#x20;                        **# list2\[0]='Guava'  (+1)** 

&#x20;                        **# list3\[0]='Apple'** 

&#x20;       sum += 1 **# sum = 2**

&#x20;   if ls\[1] == 'Kiwi': # **list1\[1]='Berry'** 

&#x20;                       **# list2\[1]='Berry'** 

&#x20;                       **# list3\[1]='Kiwi'  (+20)**

&#x20;       sum += 20 # **sum = 2 + 20 = 22**



print(sum) **# 22**

\# A. 22

\# B. 21

\# C. 0

\# D. 43



**jawaban \& output : A. 22**

