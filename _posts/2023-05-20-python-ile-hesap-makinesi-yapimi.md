---
layout: post
title:  "Python ile Hesap Makinesi Yapımı"
date:   2023-03-07 13:50:39
categories: python
---

---
# Python ile Hesap Makinesi Yapımı
---
Bu yazıda, **Python ile Hesap Makinesi Yapımını** bulacaksınız.
---
---
Bu projemizde, kullanıcıya dört temel matematiksel işlem (toplama, çıkarma, çarpma ve bölme) seçeneği sunan bir hesap makinesi uygulaması oluşturuyoruz. Kullanıcı, klavyeden istediği işlemi seçerek iki sayı girebilir ve sonucunu ekranda görüntüleyebilir. Program, kullanıcıya devam etmek isteyip istemediğini sorarak uygulamayı tekrar çalıştırmayı sağlar.

```s

def toplama(x, y):
    return x + y

def cikarma(x, y):
    return x - y

def carpma(x, y):
    return x * y

def bolme(x, y):
    if y != 0:
        return x / y
    else:
        return "Geçersiz işlem: Sıfıra bölme hatası!"

print("Hesap Makinesi")
print("İşlemler:")
print("1. Toplama")
print("2. Çıkarma")
print("3. Çarpma")
print("4. Bölme")

while True:
    secim = input("Bir işlem seçin (1/2/3/4): ")

    if secim in ['1', '2', '3', '4']:
        num1 = float(input("Birinci sayıyı girin: "))
        num2 = float(input("İkinci sayıyı girin: "))

        if secim == '1':
            print("Sonuç:", toplama(num1, num2))
        elif secim == '2':
            print("Sonuç:", cikarma(num1, num2))
        elif secim == '3':
            print("Sonuç:", carpma(num1, num2))
        elif secim == '4':
            print("Sonuç:", bolme(num1, num2))
        
        devam = input("Devam etmek istiyor musunuz? (E/H): ")
        if devam.upper() == 'H':
            break
    else:
        print("Geçersiz bir seçim yaptınız. Lütfen tekrar deneyin.")


```

---
---

Program çalıştırıldığında kullanıcı şu şekilde bir ekran ile karşılaşacaktır:

```s

Hesap Makinesi
İşlemler:
1. Toplama
2. Çıkarma
3. Çarpma
4. Bölme
Bir işlem seçin (1/2/3/4): 1
Birinci sayıyı girin: 5
İkinci sayıyı girin: 3
Sonuç: 8.0
Devam etmek istiyor musunuz? (E/H): E
Bir işlem seçin (1/2/3/4): 3
Birinci sayıyı girin: 4.5
İkinci sayıyı girin: 2
Sonuç: 9.0
Devam etmek istiyor musunuz? (E/H): H


```
