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