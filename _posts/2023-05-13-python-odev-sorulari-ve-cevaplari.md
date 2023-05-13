---
layout: post
title:  "Python Yazılım Dilinde Değişkenler"
date:   2023-03-07 13:50:39
categories: python
---

---
# Python'da 10 Ödev Sorusu ve Cevapları
---
Bu yazıda, **Python'da 10 Ödev Sorusu ve Cevaplarını** bulacaksınız.

---

Ödev 1: Python'da değişkenlerin kullanımını açıklayan bir program yazın. Kullanıcıdan iki sayı girmesini isteyin ve bu sayıları toplayarak sonucu ekrana yazdırın.
Çözüm:

```s

# Kullanıcıdan iki sayı girmesini isteyin
sayi1 = int(input("Birinci sayıyı girin: "))
sayi2 = int(input("İkinci sayıyı girin: "))

# Sayıları toplayın
sonuc = sayi1 + sayi2

# Sonucu ekrana yazdırın
print("Toplama işleminin sonucu:", sonuc)

```
Bu program, kullanıcıdan iki sayı alır, bu sayıları toplar ve sonucu ekrana yazdırır. İlk olarak, input() fonksiyonu kullanarak kullanıcıdan iki sayıyı alıyoruz. int() fonksiyonunu kullanarak kullanıcının girdiği değerleri tam sayıya dönüştürüyoruz çünkü input() fonksiyonu varsayılan olarak girdiyi bir metin olarak alır.

Daha sonra, sayi1 ve sayi2 adında iki değişken oluşturup kullanıcının girdiği değerleri bu değişkenlere atıyoruz. Ardından, sayi1 ve sayi2 değişkenlerini kullanarak toplama işlemi yapıyor ve sonucu sonuc adlı bir değişkene atıyoruz.

Son olarak, print() fonksiyonunu kullanarak "Toplama işleminin sonucu:" ifadesiyle birlikte sonuc değişkenini ekrana yazdırıyoruz.

Bu programı çalıştırarak kullanıcıdan alınan sayıların toplamını görebilirsiniz.

Ödev 2:  Python'da matematiksel operatörleri kullanarak iki sayı üzerinde farklı işlemler gerçekleştiren bir program yazın. Programın çıktısı olarak bu işlemlerin sonuçlarını ekrana yazdırın.
Çözüm:

```s

# İki sayıyı tanımlayın
sayi1 = 10
sayi2 = 4

# Toplama işlemi
toplam = sayi1 + sayi2
print("Toplama:", toplam)

# Çıkarma işlemi
cikarma = sayi1 - sayi2
print("Çıkarma:", cikarma)

# Çarpma işlemi
carpma = sayi1 * sayi2
print("Çarpma:", carpma)

# Bölme işlemi
bolum = sayi1 / sayi2
print("Bölme:", bolum)

# Tam bölme işlemi
tam_bolum = sayi1 // sayi2
print("Tam Bölme:", tam_bolum)

# Mod alma işlemi
mod = sayi1 % sayi2
print("Mod:", mod)

# Üs alma işlemi
us = sayi1 ** sayi2
print("Üs alma:", us)


```

Bu program, Python'daki matematiksel operatörleri kullanarak iki sayı üzerinde farklı işlemler gerçekleştirir. İlk olarak, sayi1 ve sayi2 adında iki değişken oluşturarak bu sayıları belirliyoruz.

Daha sonra, toplama, çıkarma, çarpma ve bölme işlemlerini gerçekleştiriyoruz. Toplama için + operatörünü, çıkarma için - operatörünü, çarpma için * operatörünü ve bölme için / operatörünü kullanıyoruz.

Ayrıca, tam bölme işlemi için // operatörünü, mod alma işlemi için % operatörünü ve üs alma işlemi için ** operatörünü kullanıyoruz. Tam bölme işlemi, bölme sonucunu tam sayı olarak verirken, mod alma işlemi bölme işleminin kalanını verir.

Son olarak, her işlemin sonucunu ekrana yazdırıyoruz. print() fonksiyonunu kullanarak her işlem sonucunu belirli bir metinle birlikte ekrana yazdırıyoruz.

Bu programı çalıştırarak, iki sayı üzerinde yapılan farklı matematiksel işlemlerin sonuçlarını görebilirsiniz.

Ödev 3:  Python'da veri tipleri arasında dönüşümleri gösteren bir program yazın. Kullanıcıdan bir tam sayı, bir ondalık sayı ve bir metin girmesini isteyin. Bu değerleri farklı veri tiplerine dönüştürerek ekrana yazdırın.

Çözüm:


```s

# Kullanıcıdan verileri alın
tam_sayi = input("Bir tam sayı girin: ")
ondalik_sayi = input("Bir ondalık sayı girin: ")
metin = input("Bir metin girin: ")

# Tam sayıyı dönüştürün
tam_sayi = int(tam_sayi)

# Ondalık sayıyı dönüştürün
ondalik_sayi = float(ondalik_sayi)

# Metni dönüştürmeye gerek yok, çünkü zaten bir metin

# Dönüşümleri ekrana yazdırın
print("Tam sayı:", tam_sayi)
print("Ondalık sayı:", ondalik_sayi)
print("Metin:", metin)

```
Bu program, kullanıcıdan bir tam sayı, bir ondalık sayı ve bir metin alır ve bu değerleri farklı veri tiplerine dönüştürerek ekrana yazdırır.

İlk olarak, input() fonksiyonunu kullanarak kullanıcıdan tam sayı, ondalık sayı ve metin girmesini istiyoruz ve bu değerleri tam_sayi, ondalik_sayi ve metin adlı değişkenlere atıyoruz.

Sonra, int() ve float() fonksiyonlarını kullanarak tam_sayi ve ondalik_sayi değişkenlerini sırasıyla tam sayı ve ondalık sayı veri tiplerine dönüştürüyoruz. Bu dönüşümler, kullanıcının girdiği metni sayısal bir değere dönüştürmemizi sağlar.

Metin veri tipinde herhangi bir dönüşüme ihtiyaç duymadığımız için, metin değişkenini olduğu gibi kullanıyoruz.

Son olarak, print() fonksiyonunu kullanarak dönüşümleri ekrana yazdırıyoruz. Her bir dönüşümün sonucunu belirli bir metinle birlikte ekrana yazdırarak hangi veri tipine dönüştürüldüğünü görebiliriz.

Bu programı çalıştırarak, kullanıcının girdiği değerlerin farklı veri tiplerine nasıl dönüştürüldüğünü görebilirsiniz.

Ödev 4: Python'da sözlüklerin kullanımını gösteren bir program yazın. Program, kullanıcıdan bir ülke adı ve başkentini alacak ve bu bilgileri bir sözlükte saklayacak. Daha sonra kullanıcıya bir ülke adı girdiğinde, program bu ülkenin başkentini ekrana yazdıracak.

Çözüm :


```s

# Sözlüğü oluşturun
ulkeler = {}

# Kullanıcıdan ülke adı ve başkentini alın
while True:
    ulke = input("Bir ülke adı girin (çıkmak için 'q' girin): ")
    if ulke == 'q':
        break
    baskent = input("Bu ülkenin başkentini girin: ")

    # Sözlüğe ülke ve başkent ekle
    ulkeler[ulke] = baskent

# Kullanıcıdan bir ülke adı alın ve başkenti ekrana yazdırın
while True:
    ulke = input("Bir ülke adı girin (çıkmak için 'q' girin): ")
    if ulke == 'q':
        break
    if ulke in ulkeler:
        print("Başkent:", ulkeler[ulke])
    else:
        print("Bu ülke sözlükte bulunmuyor.")


```
Bu program, Python'da sözlüklerin nasıl kullanıldığını gösterir. İlk olarak, boş bir sözlük olan ulkeleri oluşturuyoruz.

Daha sonra, kullanıcıdan bir ülke adı ve başkent girmesini isteyen bir döngü oluşturuyoruz. Kullanıcı 'q' girene kadar bu döngü devam eder. Kullanıcının girdiği ülke adını ulke değişkenine, başkenti ise baskent değişkenine atıyoruz. Ardından, ulkeler sözlüğüne bu ülke adını anahtar olarak, başkenti ise değer olarak ekliyoruz.

Son olarak, kullanıcıdan bir ülke adı girmesini isteyen bir başka döngü oluşturuyoruz. Kullanıcı 'q' girene kadar bu döngü devam eder. Kullanıcının girdiği ülke adını ulke değişkenine atıyoruz. Eğer bu ülke sözlükte varsa, ilgili başkenti ekrana yazdırıyoruz. Eğer sözlükte böyle bir ülke yoksa, "Bu ülke sözlükte bulunmuyor." mesajını ekrana yazdırıyoruz.

Bu programı çalıştırarak, kullanıcının girdiği ülke adına karşılık gelen başkenti sözlük üzerinden alabilirsiniz.


Ödev 5: Python'da listelerin kullanımını gösteren bir program yazın. Program, kullanıcıdan bir liste elemanı girmesini isteyecek ve bu elemanları bir listeye ekleyecektir. Daha sonra listenin tamamını ekrana yazdıracak ve listenin uzunluğunu hesaplayacaktır.

Çözüm:

```s

# Boş bir liste oluşturun
liste = []

# Kullanıcıdan liste elemanlarını alın
while True:
    eleman = input("Bir liste elemanı girin (çıkmak için 'q' girin): ")
    if eleman == 'q':
        break
    liste.append(eleman)

# Listenin tamamını ekrana yazdırın
print("Liste:", liste)

# Listenin uzunluğunu hesaplayın ve ekrana yazdırın
uzunluk = len(liste)
print("Liste Uzunluğu:", uzunluk)

```

Bu program, Python'da listelerin nasıl kullanıldığını gösterir. İlk olarak, boş bir liste olan listeyi oluşturuyoruz.

Daha sonra, kullanıcıdan bir liste elemanı girmesini isteyen bir döngü oluşturuyoruz. Kullanıcı 'q' girene kadar bu döngü devam eder. Kullanıcının girdiği elemanı eleman değişkenine atıyoruz ve liste.append(eleman) komutunu kullanarak bu elemanı listeye ekliyoruz.

Son olarak, print() fonksiyonunu kullanarak listenin tamamını ekrana yazdırıyoruz. len() fonksiyonunu kullanarak listenin uzunluğunu hesaplıyoruz ve bu uzunluğu uzunluk değişkenine atıyoruz. Son olarak, listenin uzunluğunu ekrana yazdırıyoruz.

Bu programı çalıştırarak, kullanıcının girdiği liste elemanlarını ve listenin uzunluğunu görebilirsiniz.


Ödev 6: Python'da demetlerin kullanımını gösteren bir program yazın. Program, kullanıcıdan bir demet elemanı girmesini isteyecek ve bu elemanları bir demete ekleyecektir. Daha sonra demetin tamamını ekrana yazdıracak ve demetteki bir elemanın kaç kez geçtiğini hesaplayacaktır.

Çözüm:

```s

# Boş bir demet oluşturun
demet = ()

# Kullanıcıdan demet elemanlarını alın
while True:
    eleman = input("Bir demet elemanı girin (çıkmak için 'q' girin): ")
    if eleman == 'q':
        break
    demet += (eleman,)

# Demetin tamamını ekrana yazdırın
print("Demet:", demet)

# Bir elemanın kaç kez geçtiğini hesaplayın ve ekrana yazdırın
eleman = input("Bir eleman girin: ")
sayi = demet.count(eleman)
print("Elemanın Geçtiği Sayı:", sayi)

```

Bu program, Python'da demetlerin nasıl kullanıldığını gösterir. İlk olarak, boş bir demet olan demeti oluşturuyoruz.

Daha sonra, kullanıcıdan bir demet elemanı girmesini isteyen bir döngü oluşturuyoruz. Kullanıcı 'q' girene kadar bu döngü devam eder. Kullanıcının girdiği elemanı bir demete eklemek için demet += (eleman,) komutunu kullanıyoruz. Burada elemanı bir demet olarak oluşturup += operatörüyle mevcut demete ekliyoruz.

Son olarak, print() fonksiyonunu kullanarak demetin tamamını ekrana yazdırıyoruz. Kullanıcıdan bir eleman girmesini isteyerek input() fonksiyonunu kullanıyoruz. Ardından, demet.count(eleman) komutuyla girilen elemanın demette kaç kez geçtiğini hesaplıyoruz ve bu sayıyı sayi değişkenine atıyoruz. Son olarak, sayi değerini ekrana yazdırıyoruz.

Bu programı çalıştırarak, kullanıcının girdiği demet elemanlarını, demetin tamamını ve bir elemanın demette kaç kez geçtiğini görebilirsiniz.


Ödev 7: Python'da stringlerin kullanımını gösteren bir program yazın. Program, kullanıcıdan bir cümle girmesini isteyecek ve bu cümleyi farklı şekillerde manipüle ederek ekrana yazdıracaktır. Program, cümlenin uzunluğunu hesaplayacak, tüm harfleri büyük harfe dönüştürecek, cümledeki boşluk sayısını hesaplayacak ve cümleyi tersten yazdıracaktır.

Çözüm:

```s

# Kullanıcıdan bir cümle alın
cumle = input("Bir cümle girin: ")

# Cümlenin uzunluğunu hesaplayın ve ekrana yazdırın
uzunluk = len(cumle)
print("Cümlenin Uzunluğu:", uzunluk)

# Tüm harfleri büyük harfe dönüştürün ve ekrana yazdırın
buyuk_cumle = cumle.upper()
print("Büyük Harfli Cümle:", buyuk_cumle)

# Cümledeki boşluk sayısını hesaplayın ve ekrana yazdırın
bosluk_sayisi = cumle.count(" ")
print("Boşluk Sayısı:", bosluk_sayisi)

# Cümleyi tersten yazdırın ve ekrana yazdırın
ters_cumle = cumle[::-1]
print("Ters Cümle:", ters_cumle)

```

Bu program, Python'da stringlerin nasıl kullanıldığını gösterir. İlk olarak, input() fonksiyonunu kullanarak kullanıcıdan bir cümle girmesini istiyoruz ve bu cümleyi cumle değişkenine atıyoruz.

Daha sonra, len() fonksiyonunu kullanarak cumle değişkeninin uzunluğunu hesaplıyoruz ve bu uzunluğu uzunluk değişkenine atıyoruz. Sonrasında print() fonksiyonunu kullanarak cümlenin uzunluğunu ekrana yazdırıyoruz.

Ardından, upper() metodu kullanılarak cumle değişkenindeki tüm harfleri büyük harfe dönüştürüyoruz ve bu dönüştürülmüş cümleyi buyuk_cumle değişkenine atıyoruz. Sonrasında print() fonksiyonunu kullanarak büyük harfli cümleyi ekrana yazdırıyoruz.

Daha sonra, count() metodu ile cumle değişkenindeki boşlukların sayısını hesaplıyoruz ve bu sayıyı bosluk_sayisi değişkenine atıyoruz. Sonrasında print() fonksiyonunu kullanarak boşluk sayısını ekrana yazdırıyoruz.

Son olarak, [::-1] dilimleme yöntemini kullanarak cumle değişkenini tersten yazdırıyoruz ve bu ters cümleyi ters_cumle değişkenine atıyoruz.


Ödev 8: Python'da karşılaştırma operatörlerinin nasıl kullanıldığını gösteren bir program yazın. Program, kullanıcıdan iki sayı girmesini isteyecek ve bu sayıları karşılaştırarak ekrana sonucu yazdıracaktır. Program, iki sayının birbirine eşit olup olmadığını, bir sayının diğerinden büyük veya küçük olup olmadığını kontrol edecektir.

Çözüm:

```s

# Kullanıcıdan iki sayı alın
sayi1 = float(input("Birinci sayıyı girin: "))
sayi2 = float(input("İkinci sayıyı girin: "))

# İki sayının birbirine eşit olup olmadığını kontrol edin
if sayi1 == sayi2:
    print("İki sayı birbirine eşittir.")
else:
    print("İki sayı birbirine eşit değildir.")

# Bir sayının diğerinden büyük veya küçük olup olmadığını kontrol edin
if sayi1 < sayi2:
    print("Birinci sayı, ikinci sayıdan küçüktür.")
elif sayi1 > sayi2:
    print("Birinci sayı, ikinci sayıdan büyüktür.")
else:
    print("İki sayı birbirine eşittir.")

```

Bu program, Python'da karşılaştırma operatörlerinin nasıl kullanıldığını gösterir. İlk olarak, input() fonksiyonunu kullanarak kullanıcıdan iki sayı girmesini istiyoruz ve bu sayıları sayi1 ve sayi2 değişkenlerine float türünde atıyoruz.

Daha sonra, == operatörünü kullanarak sayi1 ile sayi2'nin birbirine eşit olup olmadığını kontrol ediyoruz. Eğer eşitse, "İki sayı birbirine eşittir." mesajını ekrana yazdırıyoruz. Eğer eşit değillerse, "İki sayı birbirine eşit değildir." mesajını ekrana yazdırıyoruz.

Ardından, < ve > operatörlerini kullanarak sayi1'in sayi2'den küçük veya büyük olup olmadığını kontrol ediyoruz. Eğer sayi1 küçükse, "Birinci sayı, ikinci sayıdan küçüktür." mesajını ekrana yazdırıyoruz. Eğer sayi1 büyükse, "Birinci sayı, ikinci sayıdan büyüktür." mesajını ekrana yazdırıyoruz. Eğer her iki durum da geçerli değilse, "İki sayı birbirine eşittir." mesajını ekrana yazdırıyoruz.

Bu programı çalıştırarak, kullanıcının girdiği sayıları karşılaştırabilir ve sonuçları ekranda görebilirsiniz.

Ödev 9: Python'da if, elif, else ifadelerinin kullanımını gösteren bir program yazın. Program, kullanıcıdan bir not girmesini isteyecek ve bu nota göre karne notunu ekrana yazdıracaktır. Program, aşağıdaki kriterlere göre notları değerlendirecektir:

90 ve üzeri: AA
80-89 arası: BA
70-79 arası: BB
60-69 arası: CB
50-59 arası: CC
40-49 arası: DC
30-39 arası: DD
0-29 arası: FF


```s

# Kullanıcıdan bir not alın
notu = int(input("Bir not girin: "))

# Nota göre karne notunu belirleyin ve ekrana yazdırın
if notu >= 90:
    print("Karne Notu: AA")
elif notu >= 80:
    print("Karne Notu: BA")
elif notu >= 70:
    print("Karne Notu: BB")
elif notu >= 60:
    print("Karne Notu: CB")
elif notu >= 50:
    print("Karne Notu: CC")
elif notu >= 40:
    print("Karne Notu: DC")
elif notu >= 30:
    print("Karne Notu: DD")
else:
    print("Karne Notu: FF")

```

Bu program, Python'da if, elif ve else ifadelerinin nasıl kullanıldığını gösterir. İlk olarak, input() fonksiyonunu kullanarak kullanıcıdan bir not girmesini istiyoruz ve bu notu notu değişkenine int türünde atıyoruz.

Daha sonra, girilen nota göre karne notunu belirlemek için if, elif ve else ifadelerini kullanıyoruz. Her bir elif ifadesi, bir önceki ifadenin koşulunu kontrol eder. İlk olarak, notu >= 90 koşulunu kontrol ederiz. Eğer bu koşul doğruysa, "Karne Notu: AA" mesajını ekrana yazdırırız. Eğer koşul yanlışsa, bir sonraki elif ifadesine geçeriz ve bu şekilde devam ederiz. En son else ifadesi ise, hiçbir koşulun sağlanmadığı durumlar için kullanılır. Bu durumda, "Karne Notu: FF" mesajını ekrana yazdırırız.

Bu programı çalıştırarak, kullanıcının girdiği nota göre karne notunu ekranda görebilirsiniz.

Ödev 10: Python'da integer, float ve string veri tiplerini kullanarak basit bir hesap makinesi programı yazın. Program, kullanıcıdan iki sayı ve bir işlem türü (toplama, çıkarma, çarpma, bölme) girmesini isteyecek. Ardından, bu işlemi gerçekleştirerek sonucu ekrana yazdıracaktır.

Çözüm:


```s

# Kullanıcıdan sayıları ve işlem türünü alın
sayi1 = float(input("Birinci sayıyı girin: "))
sayi2 = float(input("İkinci sayıyı girin: "))
islem = input("İşlem türünü girin (+, -, *, /): ")

# İşlemi gerçekleştirerek sonucu hesaplayın
if islem == "+":
    sonuc = sayi1 + sayi2
elif islem == "-":
    sonuc = sayi1 - sayi2
elif islem == "*":
    sonuc = sayi1 * sayi2
elif islem == "/":
    sonuc = sayi1 / sayi2
else:
    print("Geçersiz işlem türü!")
    exit()

# Sonucu ekrana yazdırın
print("Sonuç:", sonuc)


```

Bu program, Python'da integer, float ve string veri tiplerini nasıl kullanacağınızı gösterir. İlk olarak, float() fonksiyonunu kullanarak kullanıcıdan iki sayıyı ve input() fonksiyonunu kullanarak işlem türünü alıyoruz. Sayıları float türüne dönüştürerek sayi1 ve sayi2 değişkenlerine atıyoruz.

Daha sonra, if, elif ve else ifadelerini kullanarak kullanıcının girdiği işlem türüne göre doğru işlemi gerçekleştiriyoruz. Eğer işlem türü "+" ise, sayi1 ve sayi2'yi topluyoruz. Eğer işlem türü "-" ise, sayi1'den sayi2'yi çıkarıyoruz. Eğer işlem türü "*" ise, sayi1 ve sayi2'yi çarpıyoruz. Eğer işlem türü "/" ise, sayi1'i sayi2'ye bölüyoruz.
