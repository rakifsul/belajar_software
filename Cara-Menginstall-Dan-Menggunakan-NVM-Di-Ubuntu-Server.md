# Cara Menginstall Dan Menggunakan NVM Di Ubuntu Server

## Perbedaan Ubuntu Desktop dan Ubuntu Server

Ubuntu desktop sudah disertai GUI untuk menggunakannya, sedangkan Ubuntu Server tidak.

Oleh karena itu, dalam penggunaan Ubuntu Server, digunakan terminal baik secara lokal maupun remote.

Ubuntu Desktop dan Ubuntu Server adalah varian dari sistem operasi Ubuntu yang dikembangkan oleh Canonical.

Berikut adalah beberapa perbedaan utama lainnya:

-   Antarmuka Pengguna:
    -   Ubuntu Desktop: Dirancang untuk penggunaan umum, Ubuntu Desktop dilengkapi dengan antarmuka pengguna grafis (GUI) yang disebut GNOME (meskipun versi-versi sebelumnya menggunakan Unity). Ini memberikan pengalaman pengguna yang ramah dan mudah digunakan dengan fitur-fitur seperti tata letak desktop, ikon, dan manajemen jendela.
    -   Ubuntu Server: Tidak memiliki antarmuka pengguna grafis secara default. Ubuntu Server biasanya diinstal tanpa GUI untuk mengurangi penggunaan sumber daya dan fokus pada administrasi melalui antarmuka baris perintah (CLI) atau akses jarak jauh melalui SSH.
-   Paket Perangkat Lunak Terinstal:
    -   Ubuntu Desktop: Dilengkapi dengan berbagai aplikasi dan perangkat lunak yang cocok untuk penggunaan sehari-hari, seperti peramban web, pengolah kata, perangkat lunak grafis, dan multimedia player.
    -   Ubuntu Server: Instalasi minimal dengan hanya paket dasar yang diperlukan untuk menjalankan server. Pengguna dapat menambahkan paket perangkat lunak tambahan sesuai kebutuhan, seperti server web (misalnya Apache), basis data (misalnya MySQL), atau server aplikasi.
-   Penggunaan Sumber Daya:
    -   Ubuntu Desktop: Didesain untuk bekerja pada desktop dan laptop dengan dukungan untuk perangkat keras umum, antarmuka grafis, dan penggunaan sumber daya yang lebih tinggi dibandingkan dengan server.
    -   Ubuntu Server: Dirancang untuk digunakan sebagai server, fokus pada kinerja dan efisiensi sumber daya. Tidak memiliki beban GUI bawaan membuatnya cocok untuk penggunaan di lingkungan server dengan sumber daya terbatas.
-   Tujuan dan Penggunaan:
    -   Ubuntu Desktop: Dibuat untuk penggunaan umum, desktop Ubuntu cocok untuk pekerjaan sehari-hari, hiburan, dan penggunaan pribadi.
    -   Ubuntu Server: Dirancang khusus untuk menjalankan aplikasi server dan menyediakan layanan di lingkungan server. Digunakan untuk keperluan seperti hosting web, basis data, aplikasi bisnis, atau layanan jaringan.
-   Keamanan:
    -   Ubuntu Desktop: Fokus pada keamanan pengguna individu dan menyertakan firewall dan alat keamanan standar untuk melindungi pengguna secara pribadi.
    -   Ubuntu Server: Lebih difokuskan pada keamanan jaringan dan server. Memiliki konfigurasi keamanan yang lebih ketat dengan menutup port yang tidak diperlukan dan memberikan kontrol yang lebih besar melalui antarmuka baris perintah.

Meskipun ada perbedaan ini, baik Ubuntu Desktop maupun Ubuntu Server masih memiliki dasar sistem operasi yang sama.

Pengguna dapat menyesuaikan instalasi mereka untuk memenuhi kebutuhan spesifik mereka dengan menambahkan atau menghapus paket perangkat lunak sesuai kebutuhan.

## Mengenal NVM

NVM merupakan singkatan dari Node.js Version Manager.

Artinya, kita bisa memanajemen versi Node.js dengan aplikasi tersebut.

Sebagai contoh, kita bisa install, remove, dan use Node.js dari berbagai versi melalui aplikasi tersebut.

## Perbedaan NVM dan NVM Windows

NVM Windows adalah untuk Windows dan NVM untuk Linux dan Mac.

Karena Ubuntu Server merupakan Linux, maka kita bisa menggunakannya di Ubuntu Server.

## Apakah NVM sulit diinstall?

Sama sekali tidak.

Walaupun proses install-nya via terminal, perintahnya cukup sederhana.

## Apakah NVM gratis?

Ya, NVM gratis dan open source.

## Langkah-Langkah Peng-install-an NVM

Berikut ini adalah langkah-langkah untuk meng-install NVM di Ubuntu Server.

Pertama, jalankan Ubuntu Server Anda.

Selanjutnya, buka terminal.

Selanjutnya, jika Anda belum install curl, jalankan:

```
sudo apt install curl
```

Jika sudah, jalankan perintah ini:

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

Tunggu sebentar, kemudian jalankan perintah ini:

```
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" # This loads nvm
```

Sekarang, Anda bisa menggunakannya.

Untuk mengecek bahwa proses install berhasil, jalankan:

```
nvm -v
```

## Contoh Penggunaan NVM secara Sederhana

Setelah di-install, kita bisa menggunakan NVM.

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

## Penutup dan Tips Tambahan

Setelah menginstal Node Version Manager (NVM) di sistem Anda, sebaiknya Anda mengenal beberapa tips penggunaan.

Pertama, gunakan perintah nvm ls-remote untuk melihat versi Node.js yang tersedia.

Untuk menginstal versi tertentu, gunakan nvm install [nomor versi].

Setelah instalasi, aktifkan versi yang diinginkan dengan perintah nvm use [nomor versi].

Untuk mengatur versi Node.js default, gunakan nvm alias default [nomor versi].

Penting untuk diingat bahwa setiap kali Anda membuka terminal baru, Anda mungkin perlu menjalankan nvm use [nomor versi] untuk beralih ke versi Node.js yang diinginkan.

Dengan menggunakan NVM, Anda dapat dengan mudah mengelola dan beralih antara versi Node.js, memungkinkan fleksibilitas dalam pengembangan dan pengujian aplikasi Anda.
