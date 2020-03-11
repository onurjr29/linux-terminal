# Linux Terminal Komutları

&lt;Komut&gt; &lt;seçenek&gt; &lt;argüman&gt;

**Komutların kullanma kılavuzu için**

man &lt;komut&gt;

## Bazı Komutların Kullanımı

**Şifre değiştirme**

```shell
passwd
```

---

**Sistemden çıkma**

```shell
exit or
logout or
Control + D

```

---

**Sistem değişkenleri**

```shell
set
```

---

**Dosya ve klasörleri listeleme**

```shell
ls
```

_Bazı seçenekler_

```shell
ls -a
ls -l
ls -al
ls -a /usr/folder
```

---

**ls komutu –l seçeneği ile çalıştırıldığında dosya ve dizinler hakkında ayrıntılı bilgi edinilir.**

drwxr-xr-x 2 root root 4096 Apr 24 2018 home  
drwxr-xr-x 1 root root 4096 May 23 2017 lib  
drwxr-xr-x 2 root root 4096 Feb 19 01:15 lib64  
drwxr-xr-x 2 root root 4096 Feb 19 01:14 media  
drwxr-xr-x 2 root root 4096 Feb 19 01:14 mnt

Dosya ve dizin hakları chown, chgrp ve chmod komutları ile düzenlenebilir.  
chown, dosya ya da dizinin sahibini değiştirmek için kullanılır. Komutun genel yapısı;  
chown &lt;kullanıcı adı|kullanıcı kodu&gt; &lt;dosya/dizin adı&gt;

[Ayrıntılı Bilgi İçin](https://www.enesusta.tech/articles/linux-file-system-permissons)

---

**cd dizinler arasında geçişi sağlar.**

```shell
cd /tmp
```

**mkdir dizin yaratmayı sağlar.**

```shell
mkdir yeniDosya
```

**mv dosya ya da dizinleri taşıma ya da isim değiştirme işlemini gerçekleştirir.**

```shell
mv yeni.txt /home/yeni
'yeni.txt' dosyasını '/home/yeni' dizinine taşır.
```

```shell
mv kek.txt su.txt
'kek.txt' isimli dosyayı 'su.txt olarak yeniden adlandırır.
```
