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
| `..` | Cocokkan semua karakter kecuali new line/ baris baru |
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
