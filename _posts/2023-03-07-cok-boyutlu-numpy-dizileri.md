---
layout: post
title:  "Çok Boyutlu Numpy Dizileri"
date:   2023-03-07 13:50:39
categories: numpy
---

---
# Çok Boyutlu Numpy Dizileri
---
Bu yazı, size **Çok Boyutlu Numpy Dizileri** hakkında bilgi verecektir.

---

NumPy, bilimsel hesaplama ve veri analizi uygulamaları için kullanılan bir Python kütüphanesidir. NumPy, yüksek performanslı çok boyutlu diziler için optimize edilmiş birçok fonksiyona sahiptir. Bu fonksiyonlar sayesinde, çok boyutlu verileri kolayca işleyebilirsiniz.

NumPy'de çok boyutlu diziler, birinci boyut, ikinci boyut, üçüncü boyut vb. gibi boyutlara sahip olabilir. NumPy, bir veya daha fazla boyutta sıralanmış elemanların oluşturduğu bir veri yapısı olan ndarray (n-boyutlu dizi) sınıfını kullanır.

Çok boyutlu NumPy dizileri, aşağıdaki özelliklere sahiptir:

Boyut sayısı: NumPy dizileri, bir veya daha fazla boyuta sahip olabilir. Örneğin, 1B, 2B, 3B, 4B, 5B dizileri gibi.

Boyut uzunluğu: NumPy dizileri, her boyutta farklı bir uzunluğa sahip olabilir. Örneğin, 3x3, 3x4, 2x2x2 gibi.

Veri tipi: NumPy dizileri, farklı veri tiplerini (int, float, bool, string vb.) tutabilir.

Yayılım (Broadcasting): NumPy dizileri, farklı şekil ve boyutlarda olsa bile, yayılım mekanizması kullanılarak birbiriyle uyumlu hale getirilebilir.

NumPy'de çok boyutlu bir dizi oluşturmak için, np.array() fonksiyonu kullanılabilir. Aşağıdaki örnek kod parçası, 2 boyutlu bir NumPy dizisi oluşturmak için nasıl kullanılacağını gösterir:

```sh
import numpy as np

# 2 boyutlu bir NumPy dizisi oluşturma
my_array = np.array([[1, 2, 3], [4, 5, 6]])

# NumPy dizisini ekrana yazdırma
print(my_array)
```

Yukarıdaki örnek kod parçasında, numpy kütüphanesi np kısaltmasıyla içe aktarılıyor. Daha sonra, np.array() fonksiyonu kullanılarak 2 boyutlu bir NumPy dizisi oluşturuluyor ve my_array adlı bir değişkene atanıyor. Sonrasında, print() fonksiyonu kullanılarak my_array NumPy dizisi ekrana yazdırılıyor.

Bu şekilde, NumPy'de çok boyutlu dizileri oluşturabilir ve verileri kolayca işleyebilirsiniz. Çok boyutlu NumPy dizileri, büyük veri setleri üzerinde hızlı ve verimli bir şekilde çalışır. Bu nedenle, bilimsel projelerde çok tercih edilir.

NumPy, 2 boyutlu bir veri nesnesi olan "ndarray" (NumPy Array) tipindeki verilerin manipülasyonu için özellikle tasarlanmıştır. Aşağıdaki örnek, NumPy kullanarak 2 boyutlu bir ndarray oluşturma işlemini gösterir:

```sh
import numpy as np

# 2x3 boyutlu bir ndarray oluşturma
my_array = np.array([[1, 2, 3], [4, 5, 6]])

print(my_array)
```

Bu kod, "my_array" adlı 2x3 boyutlu bir ndarray oluşturur ve bu ndarray'yi ekrana yazdırır. Çıktı şöyle görünecektir:

```s
array([[1, 2, 3],
       [4, 5, 6]])
```

Bu örnekte, np.array() yöntemi kullanılarak 2 boyutlu bir ndarray oluşturulmuştur. İlk köşeli parantez çifti, ilk satırdaki elemanları belirtirken, ikinci köşeli parantez çifti ikinci satırdaki elemanları belirtir. İç içe geçmiş köşeli parantezler, bir matrisi temsil etmek için kullanılır.

NumPy dizileri, sadece aynı türden verileri depolamakla kalmaz, aynı zamanda bu verilere matematiksel işlemler uygulama ve hatta birleştirme ve ayırma işlemleri yapma gibi bir dizi farklı işlem yapmak için de kullanılabilirler.