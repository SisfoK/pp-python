---
title: RegEx
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

RegEx atau Regular Expression adalah susunan karakter yang mendefinisikan suatu
pattern yang ingin dicari. Umumnya penggunaan regex dapat kita temukan saat
melakukan pengecekan inputan apakah termasuk email yang valid atau tidak. Di
dalam bahasa pemrograman Python, kita dapat menggunakan module re untuk bekerja
menggunakan regex. Contoh penggunaan regex dengan menggunakan module re dapat
dilihat pada contoh berikut:

```python
import re

pattern = '^a...s$'
test_string = 'abyss'
result = re.match(pattern, test_string)

if result:
    print("Search successful.")
else:
    print("Search unsuccessful.")
```

Fungsi re.match() untuk mengetes apakah variabel test_string dimulai dengan
huruf a dan diakhiri dengan huruf s serta terdiri dari 5 huruf. Fungsi tersebut
akan mengembalikan sebuah object match jika patternnya sesuai. Jika tidak maka
akan mengembalikan nilai `None`.

## Meta character

| Expression | Arti |
| ---------- | ---- |
| `[abc]` | Cocokkan salah satu dari karakter dalam kurung kotak (a, b atau c) |
| `[^abc]` | Cocokkan karakter kecuali yang ada dalam kurung kotak |
| `[a-d]` | Cocokkan karakter a - d (a, b, c, d) |
| `..` | Cocokkan semua karakter kecuali new line/ baris baru sebanyak jumlah dot (`.`) |
| `^a` | Cocokkan semua karakter yang diawali dengan a |
| `a$` | Cocokkan semua karakter yang diakhiri dengan a |
| `ma*n` | Cocokkan semua yang memiliki m diikuti satu a atau lebih, bahkan tidak ada a, misalnya mn |
| `ma+n` | Cocokkan semua yang memiliki m diikuti satu a atau lebih |
| `ma?n` | Cocokkan semua yang memiliki pola sebelum ?, misalnya man, mn, woman |
| `a|b` | Cocokkkan a atau b |
| `a{3}` | Cocokkan a yang pas 3 kali berurutan |
| `a{3, }` | Cocokkan a yang pas 3 kali atau lebih secara berurutan |
| `a{3, 5}` | Cocokkan a yang pas 3 kali sampai pas 5 kali secara berurutan |
| `(a|b|c)d` | Cocokkan semua yang memiliki a atau b atau c kemudian diikuti d |
| `\$a` | `\` digunakan untuk escape character, `\$a` berarti mencari yang cocok dengan `$a` |

## Special sequence

Special sequences digunakan untuk mencari sebuah string berdasarkan lokasi di mana
string tersebut berada. Special sequences membuat pola yang umum digunakan lebih
mudah untuk ditulis.

| Expression | Arti |
| \A | true jika karakter ditemukan di awal string |
| \b | true jika karakter ditemukan di awal kata |
| \B | true jika karakter ditemukan di akhir kata |
| \d | true jika ditemukan angka pada kata |
| \D | true jika tidak ditemukan angka pada kata |
| \s | true jika string ditemukan spasi |
| \S | true jika tidak mengandung spasi |
| \w | true jika ditemukan [a-z]|[0-9]|[_] |

Silahkan latihan di [regex101](https://regex101.com/).

## Python RegEx

Python memiliki sebuah modul bernama `re` yang digunakan untuk menjalankan perintah
regex. Untuk menggunakannya kita perlu mengimport modul `re`.

```python
import re

string = 'Hello 1234. Welcome 4523 Kaito 1412'
pattern = '\d+'

result = re.findall(pattern, string)
print(result)
```

Output:

```bash
['1234', '4523', '1412']
```
