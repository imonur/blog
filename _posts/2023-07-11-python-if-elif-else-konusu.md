---
layout: post
title:  "Python if- elif - else Konusu"
date:   2023-07-11 14:50:39
categories: python
---

---
# Python Python if- elif - else Konusu

Bu yazıda, **Python if- elif - else Konusunu** bulacaksınız.

---
## Python Yazılımında Python if- elif - else Konusu
Python yazılım diline yeni başlıyorsanız öğrenmeniz gereken en önemli konulardan birisi de if-elif-else konusudur. Diğer yazılım dillerinde de bu konu oldukça önemlidir. 
Bu ifadeler programımızda belirli işlemleri yapmamızda kullandığımız koşul ifadeleridir. Şimdi gelelim bu şimdi örnekler ile konuyu açıklamaya. 

---
### if İfadesi
"if" ifadesi, eğer anlamına gelir ve bir durumun doğru mu yoksa yanlış mı olduğunu kontrol eder. ifadenin en basit hali şu şekildedir:

```s
if koşul:
    # Kod bloğu
```
Yukarıdaki ifade belirli bir durumun doğru mu yoksa yanlış mı olduğunu kontrol eder. Eğer doğruysa bir alt satırdan yani "Kod bloğu"
kısmından çalışmaya devam eder. Eğer koşul doğru değilse bu blok atlanır ve program çalışmaya devam eder.

```s
sayi = 10

if sayi > 0:
    print("x pozitif bir sayıdır.")

```
Yukarıdaki örnekte "sayi" adını verdiğimiz değer "0" sayısından büyükse alt kısımdaki **print("x pozitif bir sayıdır.")** ifadesi çalışacaktır ve ekrana **x pozitif bir sayıdır.**
yazısı yazılacaktır. 

### elif İfadesi
"elif" ifadesi, "if" ifadesi ile birlikte kullanılır. Burada amacımız birden fazla koşul kontrol etmek istiyorsak "elif" ifadesinden faydalanırız.
Yani koşul birinci durumda "if" ifadesine bakar doğruysa "if" ifadesindeki koşul çalışır. Değilse "elif" bloğundaki ifade çalışır. Eğer "if" ve "elif" doğru değilse
o zaman en son olarak "else" bloğuna geçer. Aşağıdaki örnekte bu konuyu açıklayalım:

```s
sayi = 10

if x > 0:
    print("sayi pozitif bir sayıdır.")
elif x < 0:
    print("sayi negatif bir sayıdır.")
else:
    print("sayi sıfırdır.")
```

Yukarıdaki örnekte görüldüğü gibi bir sayı ya sıfırdan büyüktür ya da küçüktür. Eğer büyükse ekrana **sayi pozitif bir sayıdır.**
ifadesi yazılacaktır. Değilse **sayi negatif bir sayıdır.** ifadesi yazılacaktır. Eğer bunların hiçbirisi ise sayımız o zaman tek bir seçenek kalıyor
o da "else" koşulu yani **sayi sıfırdır.** Buradaki "if" değilse olan koşul "elif" ile sağlanır.

### else İfadesi
"else" ifadesi bir "if" veya "elif" ifadesinden sonra kullanılır. "else" kullanılmasındaki amaç yukardaki koşulların yani "if" ve "elif" koşullarının hiçbirisi doğru değilse 
artık sadece tek seçenek kalıyor o da "else" demek oluyor. Her zaman "if" sonra "elif" en son "else" gelecek diye bir kural yoktur.
"elif" olmadan direkt olarak "if" ifadesinden sonra da "else" gelebilir.

```s
sayi = 10

if x > 0:
    print("sayi pozitif bir sayıdır.")
else:
    print("sayi sıfırdır veya negatiftir.")
```
Yukarıdaki örnekte olduğu şekliyle de kullanılabilir. Eğer "if" doğru ise altındaki **print("sayi pozitif bir sayıdır.")** ifadesi çalışacaktır. Değilse 
direkt olarak "else" koşulu çalışacaktır ve **print("sayi sıfırdır veya negatiftir.")** ifadesi çalışacaktır.
