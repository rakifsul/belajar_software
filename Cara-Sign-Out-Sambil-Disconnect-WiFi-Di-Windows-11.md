# Cara Sign Out Sambil Disconnect WiFi Di Windows 11

Sign out Windows 11 adalah sangat bisa dilakukan.

Caranya pun dapat dibilang mudah.

Cukup pergi ke menu kiri bawah dan pilih sign out.

Namun, jika kita ingin sign out dan disconnect wifi secara otomatis, mungkin perlu trik khusus.

Caranya adalah dengan menggunakan batch.

Sekarang, kami akan membahas cara tersebut.

Pertama, buat file baru di folder manapun bernama sign-out.bat.

Kemudian, buka file tersebut dengan notepad.

Kemudian isi dengan script ini:

```
netsh wlan disconnect
timeout /t 3 /nobreak
shutdown /l
```

Save file tersebut, kemudian buat shortcutnya, kemudian letakkan shortcut tersebut ke desktop.

Jika Anda ingin sign out dan disconnect wifi bersamaan, tinggal double click shortcut tersebut.
