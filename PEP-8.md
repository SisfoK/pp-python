---
title: PEP-8
layout: default
author: "@deovaliandro dan @BobChrismansyah"
---

PEP-8 Mengatur tentang coding style, artinya saran yang baik untuk dipatuhi:

1. Gunakan indentasi 4-spasi, bukan <kbd>tab</kbd>,
2. Batasi jumlah karakter dalam satu baris sehingga tidak lebih dari 79
   karakter. Ini untuk memudahkan dalam membaca kode dalam ukuran layar yang
   besar atau kecil,
3. Gunakan blank line (baris baru) untuk memisahkan fungsi dengan class dan
   blok banyak kode di dalam fungsi,
4. Letakkan komen dengan jelas,
5. Gunakan `docstring`
6. Gunakan <kbd>space</kbd> di antara operator dan setalah koma, tetapi tidak
   untuk `()` konstruktor, misalnya `a = f(1, 2) + g(3, 4)`,
7. Gunakan penggunaan nama konsisten, UpperCamelCase untuk class dan
   lowercase_with_underscores untuk fungsi dan method. Selalu gunakan `self`
   sebagai nama argument pertama,
8. Gunakan UTF-8 atau ASCII, jangan gunakan fancy encodings,
9. Jangan gunakan karakter non-ASCII sebagai identifier.
