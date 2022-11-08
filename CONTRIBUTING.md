# Contributing

## Penulisan

- Hanya menggunakan satu h1 atau `#`,
- Tidak menggunakan urutan A, B, C, tetapi menggunakan heading misalnya
  `A. Judul 1` diganti menjadi `## Judul 1`,
- Batas vertikal mematuhi peraturan `80-char`.

## Code

### Tata Penulisan

Tata penulisan menggunakan standar dari [PEP-8](https://peps.python.org/pep-0008/).

### Docstrings

#### Penggunaan docstring

Penggunaan docstring bertujuan untuk memudahkan pembaca membaca dan
mengimplementasikan algoritma.

Docstring yang baik:

```Python
def adding(num1, num2):
    """
    menambahkan kedua bilangan
    num1 dan num2 dan dikembalikan hasilnya
    num1 = integer
    num2 = integer
    mengembalikan hasil yang berupa integer
    >>> adding(2, 50)
    52
    >>> adding(3, 2)
    5
    """
    return num1 + num2
```

Docstring yang buruk:

```Python
def adding(num1, num2):
    """
    num1 + num2
    """
    return num1 + num2
```

### Lint Test

Instalasi

Kami menggunakan flake8 untuk lint testing agar penulisan kode jadi lebih baik.

#### Installasi flake8

```bash
pip install flake8
```

#### Testing

Untuk lint testing, kami menyarankan kamu untuk melakukan tes lokal dengan flake8:

```Python
flake8 perubahan_kamu.py

flake8 .
```

Untuk doctests:

```Python
pytest . --doctest-modules

pytest perubahan_kamu.py --doctest-modules --ignore=Basic/
```
