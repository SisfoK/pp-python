# Contributing

## Penulisan

- Hanya menggunakan satu h1 atau `#`
- 

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
