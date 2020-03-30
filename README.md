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

**_clear_ Terminali temizler**

```shell
clear
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

```shell
'-a' bütün dosyaları görüntülemek için
'-l' dosyaları ayrıntılı liste şeklinde görüntülemek için kullanılır.
```

---

**_ls_ komutu –l seçeneği ile çalıştırıldığında dosya ve dizinler hakkında ayrıntılı bilgi edinilir.**

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

**_cd_ dizinler arasında geçişi sağlar.**

```shell
cd /tmp
```

---

**_mkdir_ dizin yaratmayı sağlar.**

```shell
mkdir yeniDosya
```

---

**_cp_ dosya ya da dizin kopyalama işlemini gerçekleştirir.**

```shell
cp yeni.txt copya.txt
```

---

**_mv_ dosya ya da dizinleri taşıma ya da isim değiştirme işlemini gerçekleştirir.**

```shell
mv yeni.txt /home/yeni

'yeni.txt' dosyasını '/home/yeni' dizinine taşır.
```

```shell
mv kek.txt su.txt

'kek.txt' isimli dosyayı 'su.txt' olarak yeniden adlandırır.
```

---

**_rm_ dosya ya da dizin silme işlemini gerçekleştirir.**

```shell
rm ogrenciler.txt

'ogrenciler.txt' dosyasını siler.
```

```shell
rm -Rf /home/odev/yeni

'yeni' dizinini siler.
'-R' alt dizinleri silmek için,
'f' silme onayı almadan silmek icin kullanılır.
```

---

**_ln_ dosya ya da dizinlerin bağlantılarını oluşturur.**

```shell

ln odev.txt sinav.txt
```

```shell
ln –s /home/odev /tmp/sinav

'/home/odev' dizinine '/tmp/sinav' olarak bir bağlantı oluşturur.
```

---

**_cat_ dosyanın içeriğini görüntülemek için veya içeriğini başka bir dosyaya kopyalamak için kullanılır.**

```shell
cat ogrenciler.txt
```

```shell
cat ilk.txt > yeni.txt

'ilk.txt' içeriğini 'yeni.txt' içine kopyalar.
```

```shell
cat ilk.txt ikinci.txt >> hedef.txt

'ilk.txt' ve 'ikinci.txt' içeriğini birleştirip 'hedef.txt' dosyasının sonuna ekler.
```

---

**_cmp_ iki dosyayı karşılaştırır ve farklılıklarını belirtir.**

```shell
cmp ilk.txt ogrenciler.txt
```

---

**_df_ Bağlanılmış disk bölümlerinin boyut ve doluluk bilgilerini görüntüler.**

---

**_diff_ İki metin dosyasını karşılaştırır.**

```shell
diff metin1 metin2
```

---

**_du_ Dosya ve dizinlerin disk kullanım alanlarını görüntüler.**

---

**_`(ters tırnak)_ karakter dizini içerisinde komut çalıştırılmasını sağlar.**

```shell
echo "Bugünün tarihi `date`"
```

---

**_find_ Dosya ya da dizin arama işlemlerini gerçekleştirir.**

```shell
find /etc -name "host*"
```

---

**_head_, _tail_ Dosyaların ilk ya da son bölümlerinin belirtilen sayıdaki satırlarını görüntüler. Herhangi bir seçenek girilmediğinde 10 satır görüntülenir.**

---

**_host_ Girilen IP/DNS (alan adı kaydı) bilgisinin karşılığını verir.**

```shell
host www.turkaytunc.com
```

---

**_ps_ komutu çalışan uygulamaların uygulama numaralarını (PID) görüntüler. _kill_ komutu PID’si ile belirtilen uygulamayı sonlandırır.Kill komutunda sonlandırmayı zorlamak için _-9_ parametresi kullanılır.**

```shell
ps
```

```shell
kill -9 1245
```

---
