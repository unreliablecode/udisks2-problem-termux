# udisks2-problem-termux

Cara mengatasi masalah package udisks2 tidak dapat di install pada distro linux yang teleh di install pada termux semisal Andronix, untuk memperbaiki masalah ini kita harus menghapus satu file bernama udisks2.postinst yang berada pada direktori /var/lib/dpkg/info kita harus menghapusnya karena udisks2 tidak dapat digunakan oleh proot

untuk mengatasi lebih cepat anda dapat menyalin perintah berikut

```
rm -rf /var/lib/dpkg/info/udisks2.postinst

And

dpkg --configure -a
```
Dengan meng eksekusi tiap command secara individual.
