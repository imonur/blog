---
layout: post
title:  "Python'da Hatalar ve İstisnalar ile İlgili 10 Ödev Sorusu ve Cevapları"
date:   2023-06-08 14:50:39
categories: python
---

---
# Python'da Hatalar ve İstisnalar ( try-except ) ile İlgili 10 Ödev Sorusu ve Cevapları

Bu yazıda, **Python'da Hatalar ve İstisnalar ( try-except ) ile İlgili 10 Ödev Sorusu ve Cevaplarını** bulacaksınız.

---
**Ödev 1:** Sadece bir hata türü yakalama:

**Çözüm:**

```s

try:
    x = 5 / 0
except ZeroDivisionError:
    print("Bir sayıyı sıfıra bölemezsiniz.")


```
**Çıktı:**


```s

Bir sayıyı sıfıra bölemezsiniz.

```
---
**Ödev 2:** Birden fazla hata türü yakalama:

**Çözüm:**

```s
try:
    num = int(input("Bir sayı girin: "))
    result = 10 / num
except ValueError:
    print("Geçerli bir sayı girmediniz.")
except ZeroDivisionError:
    print("Bir sayıyı sıfıra bölemezsiniz.")
```
**Çıktı:**

```s
Bir sayı girin: a
Geçerli bir sayı girmediniz.
```
---
**Ödev 3:** Genel hata yakalama:

**Çözüm:**

```s
try:
    file = open("dosya.txt", "r")
    content = file.read()
    file.close()
except:
    print("Dosya okunurken bir hata oluştu.")
```
**Çıktı:**

```s
Dosya okunurken bir hata oluştu.
```
---
**Ödev 4:** Hata nesnesini yakalama:

**Çözüm:**

```s
try:
    x = 10 / 0
except ZeroDivisionError as err:
    print("Hata:", err)
```
**Çıktı:**

```s
Hata: division by zero
```
---
**Ödev 5:** Birden fazla except bloğunu tek seferde çalıştırma:

**Çözüm:**

```s
try:
    num = int(input("Bir sayı girin: "))
    result = 10 / num
except (ValueError, ZeroDivisionError):
    print("Hata: Geçersiz giriş veya sıfıra bölme.")
```
**Çıktı:**

```s
Bir sayı girin: 0
Hata: Geçersiz giriş veya sıfıra bölme.
```
---
**Ödev 6:** Hata yakalamadan devam etme:

**Çözüm:**

```s
try:
    num = int(input("Bir sayı girin: "))
    result = 10 / num
except ValueError:
    pass
print("Program devam ediyor...")
```
**Çıktı:**

```s
Bir sayı girin: a
Program devam ediyor...
```
---
**Ödev 7:** Birden fazla try-except bloğu:

**Çözüm:**

```s
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Sıfıra bölme hatası.")
try:
    num = int(input("Bir sayı girin: "))
    result = 10 / num
except ValueError:
    print("Geçersiz giriş.")
```
**Çıktı:**

```s
Sıfıra bölme hatası.
Bir sayı girin: a
Geçersiz giriş.
```
---
**Ödev 8:** Hata durumunda programı sonlandırma:

**Çözüm:**

```s
try:
    x = 10 / 0
except ZeroDivisionError:
    print("Sıfıra bölme hatası.")
    raise SystemExit
print("Bu satır çalışmayacak.")
```
**Çıktı:**

```s
Sıfıra bölme hatası.
```
---
**Ödev 9:** else bloğunu kullanma:

**Çözüm:**

```s
try:
    num = int(input("Bir sayı girin: "))
except ValueError:
    print("Geçersiz giriş.")
else:
    print("Girilen sayı:", num)
```
**Çıktı:**

```s
Bir sayı girin: 5
Girilen sayı: 5
```
---
**Ödev 10:** finally bloğunu kullanma:

**Çözüm:**

```s

try:
    file = open("dosya.txt", "r")
    content = file.read()
except FileNotFoundError:
    print("Dosya bulunamadı.")
finally:
    file.close()
    print("Dosya kapatıldı.")

```
**Çıktı:**

```s
Dosya bulunamadı.
Dosya kapatıldı.
```
