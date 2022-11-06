---
title: File IO
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

- [Membuka file](#membuka-file)
- [Menulis File](#menulis-file)

Pada bahasa pemrograman Python, operasi pada file
terjadi sesuai urutan berikut:

1. Membuka file
2. Membaca atau menulis
3. Menutup file

## Membuka file

Python memiliki built-in function yakni `open()` yang berfungsi untuk membuka
sebuah file. Fungsi tersebut akan mengembalikan sebuah objek file. Fungsi
tersebut menerima 2 argumen yaitu path dari file dan mode yang digunakan saat
membuka file. Daftar mode yang tersedia dapat dilihat pada tabel berikut:

|                                                          | mode | deskripsi                                                                 |
|:--------------------------------------------------------:|:----:|:-------------------------------------------------------------------------:|
|                                                          | r    | Membuka file untuk operasi baca (default)                                 |
|                                                          | w    | Membuka file untuk operasi tulis. Membuat file baru apabila file tersebut |
| tidak ada atau menghapus isi file bila file tersebut ada |      |                                                                           |
|                                                          | x    | Membuat file secara exclusive. Mengembalikan kesalahan jika file ada      |
|                                                          | a    | Membuka file dan meletakkan kursor di akhir file tanpa menghapus isi file |
| tersebut. Membuat file baru jika file tersebut tidak ada |      |                                                                           |
|                                                          | t    | Membuka file dalam text mode (default)                                    |
|                                                          | b    | Membuka file dalam binary mode                                            |
|                                                          | +    | Membuka file dengan operasi baca dan tulis                                |

Misalnya:

```python
file = open("test.txt")
print(file.read())
file.close()
```

```bash
Hello world
This is the content of test.txt
```

Untuk membaca konten dari sebuah file, kita dapat menggunakan method `read()`
dari objek file yang kita miliki. Perlu diperhatikan bahwa setelah kita selesai
menggunakan objek file untuk membaca atau menulis sebuah file, kita perlu
memanggil method `close()` dari objek file tersebut. Hal ini dilakukan untuk
menutup file tersebut setelah selesai digunakan.

Terdapat cara lain untuk mengakses file pada Python tanpa perlu memanggil method
`close()` secara eksplisit yakni menggunakan keyword `with`.

```python
with open("test.txt") as file:
print(file.read())
```

Output:

```bash
Hello world
This is the content of test.txt
```

## Menulis File

Untuk menulis file pada Python, kita menggunakan method `open()` dengan
menggunakan mode `w`.

```python
with open("buah.txt", "w") as file:
file.write("Apel\n")
file.write("Mangga\n")
file.write("Jeruk\n")
file.write("Pisang\n")
file.write("Jambu\n")
```
