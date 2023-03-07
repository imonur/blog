---
layout: post
title:  "Python Listesini Numpy Dizisine Dönüştürmek"
date:   2023-03-07 13:50:39
categories: numpy
---

---
# Numpy Dizisine Dönüştürmek
---
---
Bir Python listesini **.array()** metodunu kullanarak nasıl Numpy dizisine dönüştürebiliriz?
---

Bir Python listesini NumPy dizisine dönüştürmek için, öncelikle NumPy kütüphanesini yüklemeniz gerekiyor. Ardından, NumPy'nin array() yöntemini kullanarak listeyi NumPy dizisine dönüştürebilirsiniz. Aşağıdaki örnek kod parçası, bu işlemi nasıl gerçekleştireceğinizi gösterir:

```sh
import numpy as np

# Python listesi
my_list = [1, 2, 3, 4, 5]

# NumPy dizisi
my_array = np.array(my_list)

# NumPy dizisini ekrana yazdırma
print(my_array)
```
Yukarıdaki örnek kod parçasında, numpy kütüphanesi np kısaltmasıyla içe aktarılıyor. Daha sonra, my_list adlı bir Python listesi tanımlanıyor. Sonrasında, np.array() yöntemi kullanılarak my_list listesi NumPy dizisine dönüştürülüyor ve my_array adlı bir değişkene atanıyor. En son olarak, print() fonksiyonu kullanılarak my_array NumPy dizisi ekrana yazdırılıyor.

Bu şekilde, bir Python listesini NumPy dizisine kolayca dönüştürebilirsiniz.