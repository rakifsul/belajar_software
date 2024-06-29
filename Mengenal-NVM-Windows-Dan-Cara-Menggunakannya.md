# Mengenal NVM Windows Dan Cara Menggunakannya

## Windows, apakah Windows itu?

Mungkin, Windows adalah sistem operasi yang sedang Anda gunakan jika saat ini Anda tidak sedang menggunakan Linux, Android, iOS, dan Mac OS.

Windows adalah sistem operasi (OS) yang dikembangkan oleh perusahaan teknologi Microsoft.

Sejak peluncurannya pada tahun 1985, Windows telah menjadi salah satu OS yang paling dominan di dunia, digunakan oleh jutaan orang dan organisasi di berbagai perangkat.

Windows menawarkan antarmuka grafis yang user-friendly, memungkinkan pengguna untuk berinteraksi dengan komputer menggunakan ikon, jendela, dan menu.

Windows menyediakan lingkungan yang mendukung berbagai aplikasi dan perangkat keras, membuatnya kompatibel dengan berbagai jenis komputer.

Berbagai versi Windows telah dirilis, termasuk Windows 3.1, Windows 95, XP, 7, 8, dan yang terbaru pada pengetahuan terakhir saya, Windows 11.

Windows menyediakan aplikasi bawaan seperti Explorer, Microsoft Edge, dan Microsoft Office, serta kemampuan untuk mengunduh dan menginstal aplikasi pihak ketiga.

Dengan dukungan untuk berbagai fitur seperti keamanan, konektivitas cloud, dan peningkatan performa, Windows tetap menjadi salah satu sistem operasi yang paling banyak digunakan di seluruh dunia.

## NVM, apakah NVM itu?

NVM adalah singkatan dari Node.js Version Manager.

Dengan NVM, pengguna Node.js dapat berganti-ganti versi Node.js dengan mudah.

NVM berjalan via command line, jadi, pemahaman dan pengalaman menggunakan command line dibutuhkan.

Dengan NVM, kita bisa menginstall, me-remove, dan menggunakan versi-versi Node.js.

## Node.js, apakah Node.js itu?

Node.js adalah runtime environment yang dapat digunakan untuk membuat website, aplikasi web, dan aplikasi desktop dengan menggunakan bahasa pemrograman JavaScript.

Node.js saat ini sudah cukup popular dan module-nya sudah cukup banyak.

Node.js dapat digunakan baik dengan module tambahan maupun tidak.

Module Node.js disediakan dalam bentuk package dan dapat diperloleh di www.npmjs.com via perintah npm.

npm itu sendiri berjalan di command line dan sudah disertakan saat kita menginstall Node.js.

## Version Manager itu apa, dan kenapa Node.js ada Version Manager-nya?

Node.js sejak di-release pertama kali sudah ada banyak versinya.

Tiap-tiap versi mungkin memiliki perilaku yang berbeda.

Node.js, tanpa version manager bisa saja diinstall, tapi, jika ingin lebih mudah dalam memanajemen versinya, digunakan version manager.

Di Linux dan Mac, version managernya adalah NVM.

Sedangkan, di Windows, version managernya adalah NVM Windows.

Walaupun keduanya memiliki kata “NVM”, namun keduanya merupakan aplikasi yang berbeda.

## Apakah kita bisa menggunakan NVM di Windows?

Sebenarnya, NVM (saja) tidak bisa digunakan di Windows. Hanya bisa di Linux dan Mac.

Tapi, kini ada solusi manajemen versi Node.js untuk Windows.

Namanya NVM Windows.

NVM Windows bekerja seperti halnya NVM di Linux dan Mac.

Hanya saja, untuk menginstallnya lebih mudah menurut saya.

## OK. Jadi itu bedanya NVM dengan NVM Windows?

Iya. NVM untuk Linux dan Mac, NVM Windows untuk Windows.

## Apakah proses install NVM Windows itu rumit?

Sama sekali tidak.

Kita hanya perlu download installernya, kemudian menjalankan installernya untuk meng-install-nya.

## Apakah NVM Windows itu gratis?

Ya. NVM Windows itu gratis dan open source.

## OK. Sekarang saya mulai paham. Lalu, bagaimana cara meng-install NVM Windows?

Untuk meng-install NVM Windows, download installer-nya di sini:

https://github.com/coreybutler/nvm-windows/releases

Pilih yang ekstensinya .exe, kemudian download.

Selanjutnya, jalankan installer tersebut dengan next dan finish.

## Saya sudah meng-install-nya. Bagaimana cara meyakinkan saya bahwa NVM Windows telah sukses di-install?

Untuk memastikannya, buka PowerShell atau Terminal, kemudian ketikkan:

```
nvm -v
```

Kemudian enter.

Jika versi NVM Windows-nya muncul, berarti sudah berhasil.

## Ternyata sudah berhasil. Sekarang, bagaimana cara penggunaan dasarnya?

OK. Sekarang saya akan membahas cara penggunaan NVM Windows.

Tapi yang dasar saja ya…

Untuk selengkapnya, Anda bisa kunjungi repository GitHub NVM Windows.

Ini adalah cara meng-install Node.js versi tertentu. Contohnya versi 18:

```
nvm install 18
```

Perintah itu akan meng-install Node.js versi 18 yang terbaru.

Ini adalah cara untuk me-listing versi-versi Node.js yang sudah ter-install:

```
nvm list
```

Ini adalah cara menggunakan Node.js versi tertentu. Contohnya versi 18:

```
nvm use 18
```

Setelah Anda menjalankan perintah tadi, Anda bisa cek versi Node.js nya dengan:

```
node -v
```

Jika versi Node.js yang muncul di terminal adalah 18, berarti berhasil.

Ini adalah cara untuk meng-uninstall Node.js versi tertentu.

```
nvm uninstall <versi lengkapnya, misal 18.13.0>
```

Perintah-perintah tadi kemungkinan akan men-trigger UAC di Windows.

Jika itu terjadi, izinkan saja.

## OK. Sekarang saya semakin paham. Terima kasih ya…

Sama-sama.
