# Cara Pin File Non Exe Ke Taskbar Di Windows 11

## Pendahuluan

Taskbar di Windows 11 adalah elemen yang sangat membantu memudahkan kita mengakses aplikasi.

Umumnya, aplikasi yang ditempelkan icon-nya ke taskbar dilakukan melalui menu "Pin to Taskbar".

Sayangnya, ini tidak bisa dilakukan untuk file selain executable yang berformat ".exe".

Jika dilakukan pun, maka yang di-pin adalah executable-nya bukan file nya.

Dengan kata lain, jika pin tadi dipaksakan tanpa trik tertentu, maka saat pin tersebut diklik, ia tidak akan membuka file yang kita targetkan.

Namun, ada trik yang dapat memecahkan masalah tersebut.

## Caranya

Pertama, siapkan dulu file dari jenis apapun asalkan bukan exe.

Pastikan aplikasi default untuk membuka file tersebut telah ditentukan.

Selanjutnya, file tadi di-rename menjadi berekstensi exe.

Misalnya, file "index.html" diubah menjadi "Artikel Menarik.exe".

Selanjutnya pada file exe tadi, klik kanan, show more options, pin to taskbar.

Nanti file tersebut akan menempel di taskbar.

Dari taskbar, klik kanan pada iconnya, kemudian klik kanan lagi pada icon di atasnya, kemudian properties.

Nanti akan muncul property window.

Di bagian target, isi path absolut dari FILE yang kita target.

Di bagian start in, isi dengan path absolut dari FOLDER yang memiliki file tadi.

Misal, ini target:

```
D:\Local\Web-Bundling\index.html
```

Maka, start in:

```
D:\Local\Web-Bundling
```

Sampai di situ selesai dan Anda akan dapat mengakses file target tadi dengan mengklik iconnya di taskbar.

Jika Anda ingin mengganti icon-nya, Anda bisa klik tombol "Change Icon" pada property window tadi.

Mungkin saja icon tidak akan langsung berubah. Jika demikian, sign out dan sign in lagi atau restart pc Anda.

## Penutup

Dengan sedikit trik, kemudahan mengakses file dari taskbar bisa terwujud.

Sekian...