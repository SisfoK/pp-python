## Modul Python

# Bab 1 : Intro to Python

Python sebagai bahasa pemrograman yang populer dan komprehensif dengan menggabungkan kapabilitas, sintaksis kode yang jelas serta dilengkapi pustaka standar yang mempunyai fungsionalitas sangat besar. Python termasuk dari jajaran bahasa pemrograman tingkat tinggi seperti bahasa pemrograman C, C++, Java, Perl dan Pascal.

## A. Keywords

Keywords adalah kata yang dicadangkan oleh Python sehingga tidak boleh digunakan sebagai nama variabel, fungsi atau identifier lainnya. Keywords sendiri digunakan untuk mendefinisikan sintaks dan struktur dari bahasa Python. Keyword dalam Python merupakan case sensitive.

Python 3.7 memiliki 33 keywords yang tidak dapat digunakan sebagai nama variabel, fungsi, atau objek lainnya.Semua keywords selain True, False, dan None ditulis dalam lowercase dan harus ditulis apa adanya. Berikut ini adalah daftar keywords yang ada pada Python:

<table align="center">
    <tr>
        <td align="center">False</td>
        <td align="center">await</td>
        <td align="center">else</td>
        <td align="center">import</td>
        <td align="center">pass</td>
    </tr>
    <tr>
        <td align="center">None</td>
        <td align="center">break</td>
        <td align="center">except</td>
        <td align="center">in</td>
        <td align="center">raise</td>
    </tr>
    <tr>
        <td align="center">True</td>
        <td align="center">class</td>
        <td align="center">finally</td>
        <td align="center">is</td>
        <td align="center">return</td>
    </tr>
    <tr>
        <td align="center">and</td>
        <td align="center">continue</td>
        <td align="center">for</td>
        <td align="center">lambda</td>
        <td align="center">try</td>
    </tr>
    <tr>
        <td align="center">as</td>
        <td align="center">def</td>
        <td align="center">from</td>
        <td align="center">nonlocal</td>
        <td align="center">while</td>
    </tr>
    <tr>
        <td align="center">assert</td>
        <td align="center">del</td>
        <td align="center">global</td>
        <td align="center">not</td>
        <td align="center">with</td>
    </tr>
    <tr>
        <td align="center">async</td>
        <td align="center">elif</td>
        <td align="center">if</td>
        <td align="center">or</td>
        <td align="center">yield</td>
    </tr>
</table>

## B. Identifiers

Identifiers merupakan nama yang diberikan kepada variabel, fungsi, kelas, modul atau objek lainnya. Identifiers dalam Python tidak boleh diawali dengan angka, tetapi boleh mengandung angka. Identifiers juga tidak boleh mengandung spasi atau karakter khusus, kecuali underscore (_) dan dollar sign ($). Identifiers juga bersifat case sensitive, artinya identifier yang ditulis dengan huruf besar dan huruf kecil berbeda.

Aturan dalam penamaan identifiers:

   1. Identifiers dapat berupa kombinasi dari huruf dalam lowercase (a-z) atau uppercase (A-Z) atau digit (0-9) atau underscore (_).
   Contoh:

        ```python
        myClass, var_1, this_is_a_long_variable
        ```

   2. Identifiers tidak boleh diawali dengan digit angka.
    Contoh:

        ```python
        1variable #penulisan salah
        variable1 #penulisan benar
        ```

   3. Keywords tidak dapat digunakan sebagai identifiers.

        ```python
        True = 1 #penulisan salah
        ```

        Maka outputnya akan error:

        ```text
        File "e:\SISFOK\tes.py", line 1
        True = 1
        ^^^^
        SyntaxError: cannot assign to True
        ```

   4. Tidak diperbolehkan menggunakan symbol special seperti !, @, #, $, %, dll
    Contoh :

        ```python
        x$ = 1 #penulisan salah
        ```

        Outputnya:

        ```text
        File "e:\SISFOK\tes.py", line 1
        x$ = 1
        ^
        SyntaxError: invalid syntax
        ```

   5. Sebuah identifier dapat memiliki panjang berapapun.
   6. Identifier Class harus diawali dengan huruf kapital sedangkan semua identifier lainnya harus diawali dengan huruf kecil.

        Contoh:

        ```python
        class Vehicle:
            wheels = 4

        car = Vehicle()
        print(car.wheels)
       ```

   7. Identifier yang dimulai dengan underscore (_) menandakan identifier tersebut merupakan identifier private.

       Contoh:

       ```python
       class Base:
        # Declaring private method
        def _fun(self):
         print ("Private method")
       ```

   8. Identifier yang dimulai dengan dua buah underscore (__) menandakan identifier tersebut merupakan identifier yang sangat private.

        Contoh:

        ```python
        class Base:
         # Declaring private method
         def __fun(self):
          print ("Private method")
        ```

   9. Jika identifier tersebut juga diakhiri dengan dua buah underscore (____), identifier tersebut merupakan nama yang telah ditetapkan Python.

        Contoh:

        ```python
        class Base:
        # Declaring private method
        def __init__(self):
         print ("Private method")
        ```

> Hal yang perlu diperhatikan dalam penamaan identifiers adalah:
>
>   1. Identifiers tidak boleh diawali dengan angka.
>   2. Identifiers tidak boleh mengandung spasi atau karakter khusus, kecuali underscore (_) dan dollar sign ($).
>   3. Identifiers bersifat case sensitive, artinya identifier yang ditulis dengan huruf besar dan huruf kecil berbeda.
>   4. Identifiers tidak boleh menggunakan keywords.
