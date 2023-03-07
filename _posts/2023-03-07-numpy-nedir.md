---
layout: post
title:  "Numpy Nedir?"
date:   2023-03-07 13:50:39
categories: numpy
---

---
# Numpy Paketi
---
Bu yazı, size **Numpy Paketleri** hakkında bilgi verecektir.

---

NumPy, Python'da bilimsel hesaplama yapmak için kullanılan bir kütüphanedir. NumPy, matris ve dizi işlemleri için optimize edilmiş birçok fonksiyona sahiptir. Bu fonksiyonlar sayesinde, bilimsel hesaplama ve veri analizi uygulamaları için çok verimli bir şekilde çalışabilirsiniz.

NumPy, ayrıca çok boyutlu diziler için temel veri yapısı olarak da kullanılır. Bu nedenle, NumPy, veri analizi, imge işleme, sayısal hesaplama, makine öğrenmesi ve daha birçok alanda kullanılır.

NumPy'nin ana özellikleri arasında şunlar yer alır:

Yüksek performanslı çok boyutlu diziler
Temel matematiksel işlemler için optimize edilmiş işlevler
Diziler üzerinde hızlı işlemler yapmak için uyarlanabilir yayılım (broadcasting) mekanizması
Dizileri dosyaya yazmak ve dosyadan okumak için işlevler
Çok boyutlu dizileri kolayca oluşturmak için aralık oluşturma fonksiyonları
NumPy, özellikle büyük veri setleri üzerinde çalışırken hızlı bir şekilde çalışır ve diğer veri yapılarından daha az bellek tüketir. Bu nedenle, büyük veri analizi projelerinde sıklıkla kullanılır.

NumPy, Python için açık kaynaklı bir projedir ve BSD lisansı altında dağıtılır. Bu, NumPy'yi ücretsiz olarak kullanabileceğiniz anlamına gelir.

Sonuç olarak, NumPy, Python programlama dilinde bilimsel hesaplama yapmak için kullanılan en önemli kütüphanelerden biridir. Yüksek performansı ve optimize edilmiş işlevleri ile bilim insanları, araştırmacılar, mühendisler ve öğrenciler tarafından sıklıkla kullanılır.

Python normal liste veri yapıları ile matematik işlemi yapamamaktadır. Örneğin şöyle bir işlem yapmış olsak alacağımzı hata şu olacaktır:

vize = [10, 20, 30, 40]
final = [2, 60, 32, 50]
(vize+final)/2

---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
~\AppData\Local\Temp\ipykernel_23012\1856997934.py in <module>
      1 vize = [10, 20, 30, 40]
      2 final = [2, 60, 32, 50]
----> 3 (vize+final)/2

TypeError: unsupported operand type(s) for /: 'list' and 'int'