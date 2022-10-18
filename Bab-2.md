# Bab 2: Conditional Statement
_Conditional statement_ (yang dalam bahasa Indonesia disebut pernyataan bersyarat atau pengkondisian) adalah fitur dari bahasa pemrograman yang melakukan perhitungan atau tindakan yang berbeda tergantung pada kondisi yang ditentukan programmer. Pengkondisian membuat program memiliki cabang yang masing-masing akan tereksekusi jika persyaratannya terpenuhi.

_Conditional statement_ adalah sebuah statement yang mengandung sebuah kondisi. Jika kondisi tersebut bernilai benar, maka statement akan dijalankan. Jika kondisi tersebut bernilai salah, maka statement tidak akan dijalankan. Pengkondisian biasanya dalam bentuk if statement, yaitu salah satu fitur utama dari bahasa pemrograman, tidak terkecuali Python. Hampir tidak ada bahasa pemrograman yang tidak memiliki if statement dan hampir tidak ada cara untuk memprogram tanpa cabang dalam aliran kode (setidaknya jika kode tersebut perlu memecahkan masalah yang kompleks).Pengkondisian dapat digunakan untuk mengontrol jalannya program. Contoh penggunaan pengkondisian adalah untuk menentukan apakah suatu bilangan merupakan bilangan ganjil atau genap.

Bahasa pemrograman seperti C, C++, dan Java setidaknya memiliki fitur conditional statement seperti if statement dan switch case, namun dalam bahasa python switch case baru di adaptasi pada versi 3.10 keatas yang dikenal sebagai “structural pattern matching” atau “match case”. Artinya, pada versi sebelumnya pengkondisian hanya dapat dilakukan menggunakan if statement. Ekspresi terdiri dari satu atau beberapa operator perbandingan dan operator logika yang akan menghasilkan nilai True (benar) atau False (salah).

Pengkondisian biasanya dalam bentuk if statement, yaitu salah satu fitur utama dari bahasa pemrograman, tidak terkecuali Python. Hampir tidak ada bahasa pemrograman yang tidak memiliki if statement dan hampir tidak ada cara untuk memprogram tanpa cabang dalam aliran kode (setidaknya jika kode tersebut perlu memecahkan masalah yang kompleks).

Bahasa pemrograman seperti C, C++, dan Java setidaknya memiliki fitur conditional statement seperti if statement dan switch case, namun dalam bahasa python switch case baru di adaptasi pada versi 3.10 keatas yang dikenal sebagai “structural pattern matching” atau “match case”. Artinya, pada versi sebelumnya pengkondisian hanya dapat dilakukan menggunakan if statement. Ekspresi terdiri dari satu atau beberapa operator perbandingan dan operator logika yang akan menghasilkan nilai True (benar) atau False (salah).

#### Tabel Operator Perbandingan

|Opertor|Arti|Contoh|Hasil|
|:--------:|:--------:|:--------:|:--------:|
|==|Sama dengan|a == b|False|
|!=|Tidak sama dengan|a != b|True|
|>|Lebih besar dari|a > b|False|
|<|Lebih kecil dari|a < b|True|
|>=|Lebih besar atau sama dengan|a >= b|False|
|<=|Lebih kecil atau sama dengan|a <= b|True|

#### Tabel Operator Logika

|Operator|Arti|Contoh|Hasil|
|:--------:|:--------:|:--------:|:--------:|
|and|Jika keduanya benar|a < 5 and b < 10|True|
|or|Jika salah satu benar|a < 5 or b < 4|True|
|not|Jika salah satu benar|not(a < 5 and b < 10)|False|

## A. If-else Statement

1. If statement
   _If statement_ adalah jenis pengkondisian yang paling mendasar, di mana kode dieksekusi apabila ekspresi terpenuhi atau bernilai True (benar). Pernyataan dari if statement harus memiliki indent minimal sepanjang satu spasi di awal tiap baris kode. Suatu pernyataan dapat berupa satu baris atau satu blok kode.
   > If ekspresi :
   > pernyataan/statement(dieksekusi jika ekspresi bernilai True)

   #### Alur Program

    ```mermaid
    flowchart LR
    A([Start]) --> B{Ekspresi <br> <strong>if</strong>}
    B -->|True| C[<strong>perintah</strong> <br> di dalam blok <strong>IF</strong>]
    C --> E[Rethink]
    B ---->|False| E([End])
    ```

>    Contoh 1
>    
>    ```python
>    angka = 5
>    if angka > 0:
>        print(angka,"adalah bilangan positif")
>        print("pernyataan ini benar")
>    ```
>    ```rext
>    Output:
>    >5 adalah bilangan positif
>    >pernyataan ini benar
>    ```
> 

>   Contoh 2
> 
>   ```python
>    angka = 5
>    if angka < 0:
>        print(angka,"adalah bilangan negatif")
>    else:
>        print("pernyataan ini False!")
>    ```
>    ```text
> Output:
> >pernyataan ini False!
>    ```

Contoh 3




    