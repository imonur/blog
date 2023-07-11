---
layout: post
title:  "Python'da Dosya Açma ve Yazma İşlemleri"
date:   2023-07-08 14:50:39
categories: python
---

---
# Python'da Dosya Açma ve Yazma İşlemleri

Bu yazıda, **Python'da Dosya Açma ve Yazma İşlemlerini** bulacaksınız.

# Dosya Açma ve Yazma İşlemleri
## Dosya Açma İşlemi

Dosya açma işlemlerinde open() fonksiyonunu kullanıyoruz. Yöntemi şu şekildedir: 
open(dosyanin_adi,erisim_kipi)

```s
open("personel_listesi.txt","w")
```
```s
dosya = open("personel_listesi.txt","w")
dosya.close()
```
## Dosyaları Kapatma İşlemi
Program üzerinde çalışırken dosya ile işimiz bittiğinde o dosyanın kapanması gerekmektedir. Aksi takdirde o program açık kaldığı sürece dosya silinemez.

Dosyayı kapatmak için: 
dosya.close()

```s
dosya.close()
```
## w Kipi ile Çalışmak
w kipi ile her çalışma sonunda dosya oluşturulur. Eğer var olan bir dosya varsa bunu silip tekrar oluşturur. Bu yüzden buna dikkat etmelisiniz. Türkçe karakter kullanılacaksa o zaman şu ifadeyi yazmamız gerekmektedir:

encoding = "utf-8"

```s
dosya_2 = open("ogrenci_listesi.txt", "w", encoding="utf-8")
dosya_2.write("Onur Kızılarslan")
dosya_2.close()
```

## a Kipi ile Çalışmak
append yani ekleme fonksiyonudur. Eğer dosya oluşturulmuşsa o dosyaya ekleme yapmamızı sağlar.

```s
dosya_2 = open("ogrenci_listesi.txt", "a", encoding="utf-8")
dosya_2.write("\nKerim Gümrah")
dosya_2.close()
```
```s
dosya_2 = open("ogrenci_listesi.txt", "a", encoding="utf-8")
dosya_2.write("\nKerim Gümrah")
dosya_2.close()
```

## r Kipi ile Çalışmak
Dosyaları okumak ve verileri çekmek için "r" kipiyle çalışıyoruz. Eğer vermiş olduğumuz isimle bir dosya bulunmuyorsa "FileNotFoundError" hatası verecektir.

```s
dosya_3 = open("personel_listesi.txt", "r", encoding="utf-8")
file.close()
```
```s
---------------------------------------------------------------------------
FileNotFoundError                         Traceback (most recent call last)
~\AppData\Local\Temp\ipykernel_16632\299564355.py in <module>
----> 1 dosya_3 = open("personel_listesi.txt", "r", encoding="utf-8")
      2 file.close()

FileNotFoundError: [Errno 2] No such file or directory: 'personel_listesi.txt'
```
```s
try:
    dosya_3 = open("personel_listesi.txt", "r", encoding="utf-8")
    file.close()
except FileNotFoundError:
    print("Bu isimle bir dosya bulunmamaktadır..!")
```
** Bu isimle bir dosya bulunmamaktadır..! **

```s
dosya_4 = open("ogrenci_listesi.txt", "r", encoding="utf-8")

for isim in dosya_4:
    print(isim)

dosya_4.close()
```

```s
dosya_4 = open("ogrenci_listesi.txt", "r", encoding="utf-8")

for isim in dosya_4:
    print(isim, end="")

dosya_4.close()
```

## read () Fonksiyonu
Read fonksiyonu eğer bir değer vermezsek tüm dosya içeriğini okur.

```s
dosya_4 = open("ogrenci_listesi.txt", "r", encoding="utf-8")

bilgi = dosya_4.read()
print("Dosyanın içeriği:\n", bilgi,sep="")
dosya_4.close()
```

## readline() Fonksiyonu
Bu fonksiyon her çağrıldığında tek bir satır okur. Tüm bilgileri almak için her defasında tekrardan çalıştırmak gerekmektedir.

```s
dosya_4 = open("ogrenci_listesi.txt", "r", encoding="utf-8")
print(dosya_4.readline())
```

```s
print(dosya_4.readline())
```

```s
print(dosya_4.readline())
```

```s
print(dosya_4.readline())
```

## readlines() Fonksiyonu
Bu fonksiyonu bütün bilgileri tek seferde bir liste halinde bize verir.

```s
dosya_4 = open("ogrenci_listesi.txt", "r", encoding="utf-8")
dosya_4.readlines()
dosya_4.close()
```

## seek() fonksiyonu
Eğer biz dosyanın belli bir yerine gitmek istiyorsak burada bunu kullanıyoruz. Burada hem okuma hem de yazma işlemini yapmamızı sağlayan fonksiyon r+ kipidir.

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    print(dosya.read())
```

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    dosya.seek(2)
    dosya.write("seek fonksiyonunu buraya yazdım")
```

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    print(dosya.read())
```

```s
with open("ogrenci_listesi.txt", "a", encoding="utf-8") as dosya:
    dosya.write("Suna Destina Kızılarslan\n")
```

```s
with open("ogrenci_listesi.txt", "r", encoding="utf-8") as dosya:
    print(dosya.read())
```

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    print(dosya.readlines())
```

## insert() fonksiyonu
Dosyanın içerisinde istediğimiz satıra ekleme yapar. Eğer en son satır ile arasında boşluk varsa boşlukları oluşturmaz onun yerine en son satıra ekleme yapar.

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    liste = dosya.readlines()
    liste.insert(52,"\nMerhaba Dünya")
    dosya.seek(0)
    for a in liste:
        dosya.write(a)
```

## writelines() fonksiyonu
writelines() fonksiyonu, bir liste veya başka bir iterable (yinelenebilir) nesne üzerinde döngü yaparak, her bir öğeyi bir dosyaya satır olarak yazmak için kullanılır. Bu yöntem, dosyaya birden çok satır eklemek için kullanışlıdır.

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    liste = dosya.readlines()
    liste.insert(2,"Python Eğitimi\n")
    dosya.seek(0)
    dosya.writelines(liste)
```

```s
with open("ogrenci_listesi.txt", "r+", encoding="utf-8") as dosya:
    bilgi = dosya.read()
    print(bilgi)
```

## tell() fonksiyonu
imlecin hangi byte üzerinde olduğunu bize söyleyen fonksiyon.

```s
with open("ogrenci_listesi.txt", "r", encoding="utf-8") as dosya:
    print(dosya.tell())
```

```s
with open("ogrenci_listesi.txt", "r", encoding="utf-8") as dosya:
    dosya.seek(10)
    bilgi = dosya.read(20)
    print(bilgi)
    print(dosya.tell())
```
