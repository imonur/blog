---
layout: post
title:  "Matplotlib Kütüphanesi Nedir?"
date:   2023-03-07 13:50:39
categories: matplotlib
---

---
# Matplotlib Kütüphanesi Nedir?
---
Matplotlib, Python programlama dilinde veri görselleştirme için kullanılan bir kütüphanedir. Matplotlib, grafiklerin çizimini ve düzenlenmesini kolaylaştıran birçok fonksiyon sunar. Bu makalede, Matplotlib kütüphanesi hakkında genel bir bakış sunacağız ve özelliklerine daha ayrıntılı bir şekilde değineceğiz.

---

**Matplotlib Kütüphanesi Nedir?**

Matplotlib, Python programlama dilinde veri görselleştirme için kullanılan bir kütüphanedir. Matplotlib, birçok grafik türünü çizmek için kullanılan bir dizi fonksiyon sunar. Matplotlib kütüphanesi, veri görselleştirme işlemleri için sık kullanılan bir araçtır ve sadece Python dilinde değil, diğer dillerde de kullanılmaktadır.

**Matplotlib Kütüphanesi Özellikleri**

Matplotlib kütüphanesi, veri görselleştirme işlemleri için birçok özellik sunar. İşte Matplotlib'un en sık kullanılan özelliklerinden bazıları:

**Basit Grafikler**

Matplotlib, basit grafikler için kullanılan birçok fonksiyon sunar. Bunlardan bazıları şunlardır:

1.  Line Plot (Çizgi Grafiği)
2.  Scatter Plot (Nokta Grafiği)
3.  Bar Plot (Bar Grafiği)
4.  Histogram
5.  Pie Chart (Pasta Grafiği)

```s
import matplotlib.pyplot as plt

# Line plot (Çizgi grafiği)
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
plt.plot(x, y)

# Scatter plot (Nokta grafiği)
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
plt.scatter(x, y)

# Bar plot (Bar grafiği)
x = ['A', 'B', 'C', 'D', 'E']
y = [10, 8, 6, 4, 2]
plt.bar(x, y)

# Histogram
data = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 5, 5, 5, 5, 5]
plt.hist(data)

# Pie chart (Pasta grafiği)
sizes = [25, 30, 45]
labels = ['A', 'B', 'C']
plt.pie(sizes, labels=labels)

plt.show()
```

**Grafik Stilleri**

Matplotlib, grafiklerin görünümünü değiştirmek için birkaç stil sunar. Bu stiller, grafiklerin daha okunaklı ve profesyonel görünmesine yardımcı olabilir.

```s
import matplotlib.pyplot as plt

# Stil ayarı
plt.style.use('ggplot')

# Line plot (Çizgi grafiği)
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
```
