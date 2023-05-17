---
layout: post
title:  "Python'da Fonksiyonlar ile İlgili 10 Ödev Sorusu ve Cevapları"
date:   2023-03-07 13:50:39
categories: python
---

---
# Python'da Fonksiyonlar ile İlgili 10 Ödev Sorusu ve Cevapları
---
Bu yazıda, **Python'da Fonksiyonlar ile İlgili 10 Ödev Sorusu ve Cevapları** bulacaksınız.

---
---
**Ödev 1:** İki sayının toplamını döndüren bir fonksiyon yazın.

**Çözüm:**

```s

def toplam(sayi1, sayi2):
    return sayi1 + sayi2

```
---
---
**Ödev 2:** Bir sayının faktöriyelini hesaplayan bir fonksiyon yazın.

**Çözüm:**

```s

def faktoriyel(sayi):
    sonuc = 1
    for i in range(1, sayi + 1):
        sonuc *= i
    return sonuc

```
---
---
**Ödev 3:** Verilen bir listedeki en büyük sayıyı bulan bir fonksiyon yazın.

**Çözüm:**

```s

def en_buyuk(liste):
    en_buyuk_sayi = liste[0]
    for sayi in liste:
        if sayi > en_buyuk_sayi:
            en_buyuk_sayi = sayi
    return en_buyuk_sayi
    
```
---
---
**Ödev 4:** Bir metnin tersten yazılışını döndüren bir fonksiyon yazın.

**Çözüm:**

```s

def tersten_yaz(metin):
    return metin[::-1]
    
```
---
---
**Ödev 5:**  Verilen bir sayının tek mi yoksa çift mi olduğunu belirleyen bir fonksiyon yazın.

**Çözüm:**

```s

def tek_mi_cift_mi(sayi):
    if sayi % 2 == 0:
        return "Çift"
    else:
        return "Tek"
    
```
---
---
**Ödev 6:**  Verilen bir sayının asal olup olmadığını kontrol eden bir fonksiyon yazın.

**Çözüm:**

```s

def asal_mi(sayi):
    if sayi < 2:
        return False
    for i in range(2, int(sayi ** 0.5) + 1):
        if sayi % i == 0:
            return False
    return True
    
```
---
---
**Ödev 7:**  Verilen bir cümledeki kelime sayısını hesaplayan bir fonksiyon yazın.

**Çözüm:**

```s

def kelime_sayisi(cumle):
    kelimeler = cumle.split()
    return len(kelimeler)
    
```
---
---
**Ödev 8:**  Bir sayının rakamlarının toplamını hesaplayan bir fonksiyon yazın.

**Çözüm:**

```s
def rakam_toplami(sayi):
    toplam = 0
    for rakam in str(sayi):
        toplam += int(rakam)
    return toplam
    
```
---
---
**Ödev 9:**  Verilen bir liste içindeki tekrar eden sayıları bulan bir fonksiyon yazın.

**Çözüm:**

```s
def tekrarlayan_sayilar(liste):
    tekrarlar = []
    for sayi in liste:
        if liste.count(sayi) > 1 and sayi not in tekrarlar:
            tekrarlar.append(sayi)
    return tekrarlar
    
```
---
---
**Ödev 10:**  Verilen bir metindeki harflerin frekansını hesaplayan bir fonksiyon yazın.

**Çözüm:**

```s
def harf_frekansi(metin):
    frekanslar = {}
    for harf in metin:
        if harf in frekanslar:
            frekanslar[harf] += 1
        else:
            frekanslar[harf] = 1
    return frekanslar    
```
---
