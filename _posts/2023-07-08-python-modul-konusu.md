---
layout: post
title:  "Python Modül Konusu"
date:   2023-07-08 14:50:39
categories: python
---

---
# Python Modüller (Module) Konusu

Bu yazıda, **Python'da Modüller Konusunu** bulacaksınız.

---
## Python Yazılımında Modüller
Python, ücretsiz, açıık kaynak kodlu, güçlü, hızlı ve genişletilebilir bir programlama dilidir. Bu yazılım dilinin gelişmesi için tüm dünyadan birçok geliştirici eklemeler yaparak dilin genişlemesine ve güçlenmmesine katkı sağlamaktadır. Modüller, python'da yazacağınız programın daha rahat kontrol edilmesine, genişlemesine ve kullanımına olanak sağlar. 

## Modül Nedir?
Modül, bünyesinde fonksiyonları, değişkenleri, sınıfları ve diğer öğeleri içeren dosyalardır. Modüller ile projenizi organize ederek daha düzenli bir şekilde bölmenize ve düzenli bir yapıda saklamanıza imkan tanır. Böylelikle büyük projelerinizi daha okunaklı ve kullanışlı bir şekle sokabilirsiniz.

Birçok modül Python içersinde yerleşik olarak gelmektedir. Bunlar Python tarafından gömülü olarak bilgisayarınıza gömülü olarak gelmektedir. Bu standart modüller Python'ın resmi internet sayfasında açıklamaları ile (https://docs.python.org/3/py-modindex.html) bulunmaktadır. Örneğin "math" modülü ile matematiksel işlemler yapabilirsiniz "os" modülü ile işletim sistemi fonksiyonlarına erişebilirsiniz. Python dışında modüller farklı görevler için geliştirilmiştir. Bunlara üçüncü taraf modüller denilmektedir. Örneğin NumPy ile gelişmiş sayısal işlemler yapmanıza imkan verirken, Request modülü ile HTTP istekleri yapmanızı sağlar. 

## Modülü Programımıza Dahil Etmek
Gerek Python ile gelen modüller olsun gerekse üçüncü taraf modüller olsun projemize dahil edilirken "import" anahtar kelimesi ile eklenir. Örneğin math modülünü projemize dahil edelim. 

```s

import math

# math modülündeki pi sayısını kullanma
print(math.pi)

# math modülündeki cos fonksiyonunu kullanma
print(math.cos(0))

```

Yukarıdaki örnekte "math" modülünü içe aktardık ve modülümüzdeki "pi" sabitini ve "cos" fonksiyonunu kullanıyoruz. Bir modülün içerisindeki fonksiyonlara erişmek için nokta operatöründenfaydalanırız. Bir modülü projemize dahil ettikten sonra içerisindeki tüm fonksiyonlara projemizde erişebiliriz. Ancak bazı zamanlarda projemizde kullanacağımız modülün belirli öğelerini içe aktarırız. Bu tür durumlarda ise "from" anahtar kelimesinden faydalanırız. Örneğin:

```s

from math import pi, cos

# pi sayısını kullanma
print(pi)

# cos fonksiyonunu kullanma
print(cos(0))

```

Yukarıdaki örnekte ise "math" modülü içerisindeki "pi" ve "cos" fonksiyonlarını kullandık.

## Kendi Modülümüzü Nasıl Oluşturabiliriz
Python yazılımında kendi modülünüzü rahatlıkla yazabilirsiniz. Pythonn yazılımı yapısı gereği geliştiricilerin kendi modüllerini yazmasına imkan tanır. Bunun için yapmanız gerekenler oldukça basittir. Kendi modülünüzü yazarken ilk önce yazmış olduğunuz projeyi ".py" uzantısı ile kayıt etmeniz gerekiyor. Daha sonra projenize "import" fonksiyonu ile dahil ediyorsunuz. Örneğin aşağıdaki çalışmayı "selam_modul.py" adında kayıt ediniz.

```s

def selamlama():
    print("Merhaba Ben Örnek Modülüm!")

def selam_python():
    print("Merhaba Python!")


```

Boş bir sayfa açarak yukarıdaki çalışmayı "selam_modul.py" adında kayıt ettikten sonra artık projenize dahil edebileceğiniz bir modülünüz olmuş oldu. Bundan sonraki çalışmalarda bu modülü projenize dahil etmek istiyorsanız import fonksiyonunu kullanmanız gerekiyor. Örneği şu şekilde:

```s

import selam_modul

my_module.selamlama()
my_module.selam_python()

```

## Modüller Hakkında Kısaca Şunları Söyleyebiliriz
* Modüller program içerisinde ücretsiz bir şekilde önceden yüklü olarak gelmektedir. Bunun yanısıra bizim ihtiyacımız olan modülleri kendimiz de yazabilir bunu programa dahil edebiliriz.

* Modüllerin içerisinde birden fazla nesne bulunabilir.

* Modülü programın içerisine dahil ederken import fonksiyonundan faydalanıyoruz. Örneğin : import math ----> Burada matematik modülü projemize dahil edilmiş oldu.

* Bir modülün içerisindeki nesneye ulaşmak için "modül_adı.nesne_adı" şeklinde yazıyoruz. Örneğin : math.pi ----> Burada matematik modülünün pi sayısı nesnesine ulaşmış olduk.

* Modül içerisindeki bir nesneyi projemize dahil etmek istiyorsak "from" anahtarından faydalanırız. Örneğin : from math import pi ----> Burada math kütüphanesinden pi'yi import et demiş olduk.

* Python Modüllerine buradan ulaşabiliriz: https://docs.python.org/3/py-modindex.html
