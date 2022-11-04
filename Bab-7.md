---
title: RegEx
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

RegEx atau Regular Expression adalah susunan karakter yang mendefinisikan suatu
pattern yang ingin dicari. Umumnya penggunaan regex dapat kita temukan saat melakukan
pengecekan inputan apakah termasuk email yang valid atau tidak. Di dalam bahasa
pemrograman Python, kita dapat menggunakan module re untuk bekerja menggunakan regex.
Contoh penggunaan regex dengan menggunakan module re dapat dilihat pada contoh berikut

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

Fungsi re.match() untuk mengetes apakah variabel test_string dimulai
dengan huruf a dan diakhiri dengan huruf s serta terdiri dari 5 huruf. Fungsi tersebut akan
mengembalikan sebuah object match jika patternnya sesuai. Jika tidak maka akan
mengembalikan nilai None.