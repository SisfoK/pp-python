---
title: Function
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

Function atau fungsi didefinisikan sebagai sekumpulan baris perintah atau kode
yang dikelompokkan menjadi satu kesatuan dan dapat dipanggil atau digunakan
berkali-kali. Sebuah function bisa menerima parameter, bisa mengembalikan suatu
nilai, dan bisa dipanggil berkali-kali secara independen. Tujuan dari function
adalah untuk memecah program yang besar dan kompleks menjadi bagian-bagian kecil
dengan tugasnya masing-masing.

> Fungsi dan method sering ditukar, method adalah fungsi yang terikat pada
> sebuah objek, sedangkan fungsi bebas.

Fungsi dibuat dengan menggunakan:

```python
def func(param):
    ...
```

Dan dapat dipanggil dengan:

```python
func()
```

## Parameter

Parameter adalah nilai yang dikirim ke fungsi. Contohnya

```python
def say_hello(name):
    print("Hello", name)
```

Misalnya dipanggil dengan:

```python
say_hello("Alice")
```

akan menghasilkan:

```bash
Hello Alice
```

Parameter harus diisi dan berurutan sesuai dengan urutan parameter yang diminta,
jika tidak akan memunculkan:

```bash
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: say_hello() missing 1 required positional argument: 'bob'
```

### Default parameter

Kita bisa memberikan nilai default pada parameter, misalnya dengan:

```python
def say_hello(name="Alicee"):
    print(name)
```

jika nilai name tidak diberikan, maka akan menggunakan default parameter yaitu
`Alicee`.

## Return value

Pengembalian nilai berfungsi untuk mengembalikan nilai hasil operasi sebuah
fungsi. Contohnya:

```python
def add_value(a, b):
    return a + b
```

fungsi `add_value` tersebut akan mengembalikan nilai hasil penambahan 2
parameter yang diberikan.

## Fungsi Rekursif

> Coba cari kata `recursion` di google, hasilnya?

Rekursif adalah rekursif :D.

Rekursif adalah fungsi yang memanggil dirinya sendiri. Dalam matematika,
dikatakan bahwa fungsi tersebut _isomorphic_ terhadap dirinya sendiri.

Rekursif digunakan untuk melakukan sebuah fungsi yang berulang, misalnya:

```python
def fib(n):
    if n in {0, 1}:
        return n
    return fib(n - 1) + fib(n - 2)
```

Kemudian dipanggil:

```python
fib(10)
```

proses ini akan menjalankan fungsi `fib()` secara berkali-kali.
