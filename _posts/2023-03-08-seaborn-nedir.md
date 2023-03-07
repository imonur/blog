---
layout: post
title:  "Seaborn Nedir?"
date:   2023-03-07 13:50:39
categories: seaborn
---

---
# Seaborn Paketi
---
Bu yazı, size **Seaborn Kütüphanesi** hakkında bilgi verecektir.

---

Seaborn, Python programlama dilinde veri görselleştirme için kullanılan bir kütüphanedir. Seaborn, Matplotlib kütüphanesi üzerine kurulmuştur ve daha yüksek düzeyde bir arayüz sunar.
Bu makalede, Seaborn kütüphanesi hakkında genel bir bakış sunacağız ve özelliklerine daha ayrıntılı bir şekilde değineceğiz.

**Seaborn Kütüphanesi Nedir?**

Seaborn, Matplotlib kütüphanesi üzerine inşa edilen bir veri görselleştirme kütüphanesidir. Seaborn, Matplotlib'in sunduğu temel grafik işlevlerine ek olarak, önceden oluşturulmuş stiller ve rengin seçimi, grafik nesnelerinin ayarları ve daha birçok özellik sunar. Seaborn, özellikle istatistiksel grafikler oluşturmak için kullanılır ve veri görselleştirme için birçok yararlı özellik sunar.

**Seaborn Kütüphanesi Özellikleri**

Seaborn kütüphanesi, veri görselleştirme için birçok özellik sunar. İşte Seaborn'un en sık kullanılan özelliklerinden bazıları:

**Veri Seti Yükleme**

Seaborn kütüphanesi, çeşitli veri setlerini yüklemek için birçok fonksiyon sağlar. Bu veri setleri, Seaborn kütüphanesinin özelliklerini göstermek için kullanılabilir. Örneğin, iris veri seti, sık kullanılan bir veri setidir ve Seaborn kütüphanesi ile birlikte gelir.


```s
import seaborn as sns

# Iris veri seti yükleme
iris = sns.load_dataset("iris")

# İlk 5 satırı görüntüleme
print(iris.head())
```

**Veri Görselleştirme**

Seaborn kütüphanesi, birçok görselleştirme işlevi sağlar. Seaborn ile basitçe görselleştirebileceğiniz bazı özellikler:

1.  Histogramlar
2.  Yoğunluk Grafikleri
3.  Çizgi Grafikleri
4.  Kutu Grafikleri
5.  Isı Haritaları
6.  Scatterplotlar
7.  FacetGrid'ler

```s
import seaborn as sns
import matplotlib.pyplot as plt

# İris veri setini yükleme
iris = sns.load_dataset("iris")

# Yoğunluk grafiği çizimi
sns.kdeplot(iris['sepal_length'], shade=True)

# Grafiği gösterme
plt.show()

```

**Stiller**

Seaborn, önceden tanımlanmış birkaç stil sunar. Bu stiller, grafiklerin görünümünü değiştirmenize olanak tanır.

```s
import seaborn as sns
import matplotlib.pyplot as plt

# Stil ayarı
sns.set_style("darkgrid")

# Veri seti yükleme
tips = sns.load_dataset("tips")
```
