---
title: Collection
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

Collection adalah kumpulan dari beberapa nilai baik itu angka, string, bahkan variable
dalam satu grup. Collection terbagi menjadi tiga yaitu List, Tuples, Dictionary, Set.

## List

List digunakan untuk menyimpan beberapa item dalam satu variabel. List adalah salah
satu dari 4 tipe data bawaan dalam Python yang digunakan untuk menyimpan kumpulan
data.

Untuk membuat list:

```python
listExample = [1, 2, 3]
```

Dan untuk mengaksesnya menggunakan:

```python
listExample[0]
```

Untuk mengubah data list:

```python
listExample[1] = 10
```

### Built-In Function pada List

#### Append

```python
listExample.append(4)
```

digunakan untuk menambah data.

#### Extend

```python
listExample.extend([5, 6, 7])
```

digunakan untuk menambah list ke dalam list.

#### Remove

```python
listExample.remove(10)
```

digunakan untuk menghapus data.

#### Pop

```python
listExample.pop(1)
```

digunakan untuk menghapus data pada index i, tetapi jika tidak diberikan nilai i
maka akan mengambil nilai terakhir.

#### Insert

```python
listExample.insert(1, 2)
```

untuk menambah data pada posisi tertentu.

Untuk fungsi lainnya bisa dilihat pada: [Dokumentasi Resmi](https://docs.python.org/3/tutorial/datastructures.html)

## Dictionary

Dictionary adalah kumpulan nilai kunci, yang digunakan untuk menyimpan nilai data
key dan value, tidak seperti list yang hanya menyimpan satu nilai sebagai elemen.

Untuk membuat dictionary:

```python
dictExample = {
    "name": "Fatwa",
    "age": 22,
    "hobby": "Playing Onet",
}
```

### Operasi pada Dictionary

Untuk Mengambil data dictionary kita bisa melakukannya seperti pada list

```python
dictExample["name"]
```

Untuk mengupdate data pada dictionary kita hanya perlu mengintansinya kembali.

```python
dictExample["hobby"] = "Playing sudoku"
```

Begitu pula untuk menambah data pada dictionary kita hanya perlu menginstansiasinya.

```python
dictExample["graduationYear"] = 2022
```

## Tuple

Tuple digunakan untuk menyimpan beberapa item dalam satu variabel. Tuple adalah
kumpulan item dan tidak dapat diubah.

Penulisan tuple di mulai dan ditutup dengan tanda kurung. Contoh:

```python
tupleExample = ("Coding", True, False, "Adakah")
```

Tuple kumpulan beberapa item dan tidak dapat diubah lagi. Tetapi kita bisa
melakukan manipulasi tuple tersebut, dengan cara melakukan konversi tipe
data tuple ke list, lalu data list yang kita ubah, setelah diubah, dilakukan
kembali konversi data dari list ke tuple.

```python
tupleExample = ("Coding", True, False, "Adakah")
tupleToList = list(tupleExample)
tupleToList[0] = "Dari Tuple Ke List"
tupleExample = tuple(tupleToList
```

## Set

Set adalah kumpulan yang tidak berurutan, tidak dapat diubah, dan tidak terindeks dan
tidak ada anggota yang terduplikat. Sama halnya dengan tuple, set juga bisa memiliki
item yang berbeda tipe datanya serta juga dapat diketahui panjangnya atau banyaknya
item di dalam set dengan menggunakan fungsi len()

Set diinisiasi dengan cara membungkus data menggunakan kurung kurawal

```python
setExample = {"Tes", 1, 2, "Mantap"}
```

Set adalah kumpulan beberapa item dan tidak dapat diubah lagi.
Tetapi kita bisa melakukan manipulasi set tersebut, dengan cara
melakukan konversi tipe data set ke list, lalu data list yang kita ubah, setelah
diubah, dilakukan kembali konversi data dari list ke set.