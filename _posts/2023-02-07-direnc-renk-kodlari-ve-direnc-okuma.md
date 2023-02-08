---
layout: post
title:  "Direnç Renk Kodları ve Direnç Okuma"
date:   2023-02-02 13:50:39
categories: coding
---
---
# Direnç Renk Kodları ve Direnç Okuma
---
Bu yazı, size **Direnç Renk Kodları ve Direnç Okumayı** gösterecektir.

Her rengin bir sayı değeri, bir çarpan değeri ve bazı renklerin tolerans değerleri vardır. Aşağıdaki tabloda renklerin sayı, çarpan ve tolerans değerleri görülüyor. Mesela Yeşil: Sayı olarak kullanılıyorsa 5, çarpan olarak kullanılıyorsa 105 yani 100.000, tolerans olarak kullanılıyorsa %0,5’i ifade eder.
     
---

![Direnc_Okuma](https://raw.githubusercontent.com/imonur/blog/main/projects/images/direnc_okuma/direnc_okuma.png)

Kırmızının sayı değeri 2, çarpan değeri 102 yani 100, tolerans değeri %2 dir. Sayı değerini bilmek çarpan değerini de bilmek demektir. Çünkü çarpan değeri 10sayı değeri dir. Sayı değeri 2 ise çarpan 102=100 dür, 5 ise çarpan 105=100.000 dir. Renklerin sayı değerlerini kolayca akılda tutmak için “Sokakta Sayamam Gibi” ifadesi ezberlenebilir.

![Direnc_Okuma_2](https://raw.githubusercontent.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc_okuma2.png)

Direnç değerleri renklerle belirlenirken 3, 4, 5 veya 6 renk kullanılabilir.

### 4 Renkli Dirençler:

Direnç üzerinde 4 renk bandı kullanılarak değeri ifade edilir.

![Direnc_Okuma_3](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc.png)

4 renkli kodlamada 1. ve 2. renk sayı, 3. renk çarpan, 4. renk toleranstır.

![Direnc_Okuma_3](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc2.png)

İlk iki sayı yan yana yazılır, çarpanla çarpılır. Bu bize Ohm olarak direnç değerini verir. Bir başka ifade ile 1. ve 2. renklerin sayı değeri yan yana yazılıp, çıkan değer, 3. rengin çarpan değeri ile çarpılır. Çarpım sonucu çıkacak değer direncin ohm olarak değeridir. 4. renk ise tolerans değeridir.

### Yasaklı Renkler:

İlk bant siyah, altın ve gümüş olamaz. Çünkü siyahın sayı değeri 0 dır. Altın ve gümüşün ise sayı değeri yoktur, tolerans değerleri vardır. 4 renkli dirençlerde 3. renk (çarpan rengi) mavi (106) ve daha küçük çarpanlı renkler olabilir. Mesela 3 renk mor olamaz. Mor 107 ile çarpmak demektir. Sayı renklerini en küçük seçsek (kahverengi, siyah) 10×107= 100MOhm elde ederiz. Bu da mümkün değildir. 5 Bantlı dirençlerden 4. Bant (çarpan rengi) yeşil ve daha küçük renkler olmalıdır. (5 Bantlı dirençler aşağıda incelenmiştir)

### Okuma Yönü Nasıl Buluruz:

Renkler soldan sağa doğru okunmalıdır. Okuma yönünü doğru tesbit etmek için aşağıdaki kriterler size yardımcı olacaktır.

* Çarpan ve tolerans renkleri arasındaki mesafe daha fazladır. Bu şekilde tolerans rengi sağa gelecek şekilde okuma yönünü ayarlayabiliriz.
* Altın ve gümüş renkleri tolerans rengi olduğu için daima sağda olmalıdır.
* Bazen de 1. sayı bandı direnç bacağına daha yakındır.
* Yukarıdaki yasaklı renkler kısmı da bu konuda bize yardım edebilir.

### Tolerans:

Tolerans direnç değerindeki üretimden kaynaklanan hata payı demektir. Direncin toleransı %5 ise, bu direncin değeri renklerle kodlanan değerinden %5 oranında küçük veya büyük olabilir. Mesela Bir direnci üzerindeki renklerden 100 Ohm %5 toleranslı okuduk diyelim. %5 fazlası 100+%5=105 Ohm, %5 düşüğü 100-%5=95 Ohm olur. Yani bu direnci ölçtüğümüzde değeri 95-105 Ohm arasında çıkabilir, bu normaldir. Direnci 95 Ohm ölçmüşsek bu direnç bozuk demek değildir.

### 4 Renkli Direnç Okuma Örnekleri:

![Direnc_Okuma_4](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc3.png)

Kahverengi (1) – Siyah (0)- Siyah (100=1)- Altın (%5) 10 Ohm %5 3. renk çarpan olduğu için, 3. renk olan siyahın çarpan değerini yazdık.

![Direnc_Okuma_4](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc4.png)

![Direnc_Okuma_5](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc5.png)

Kırmızı(2) –Mor(7) –Kahverengi(101=10 çünkü 3. renk çarpan) –Altın(tolerans %5) 27×10= 270 Ohm, Toleransı %5

![Direnc_Okuma_6](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc6.png)

Not: Dirençte tolerans rengi yoksa ve 3 renkliyse, 4 renkli direnç gibi okunur. Tolerans rengi olmadığından toleransı %20 kabul edilir.

### 5 Renkli Dirençler:

5 Renkli Dirençlerde, 4 renkliden farklı olarak 3 tane sayı vardır.


![Direnc_Okuma_7](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc7.png)

![Direnc_Okuma_8](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc8.png)

![Direnc_Okuma_9](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc9.png)

### 6 Renkli Dirençler:

6 Renkli dirençlerin okunması 5 renkli dirençlerle aynıdır. Farklı olarak 6. renk sıcaklık katsayısını ifade eder.

### Sıcaklık Katsayısı:

Bu katsayı direncin değerinin sıcaklıkla ne kadar değiştiğini belirtir. Birimi PPM/oC dir. Yani oC (santigrat derecede) milyon başına değişim demektir (PPM=part per million) 1Mohm bir direncin sıcaklık katsayısı 400PPM/ oC ise bunun anlamı şudur 1 oC sıcaklık artışı direncin değerini 400 Ohm değiştirebilir. Azaltabilir veya artırabilir. Sıcaklıkla dirençin değişimini şu şekilde hesaplayabiliriz:

![Direnc_Okuma_10](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc10.png)

ΔR : Dirençteki değişim miktarı (ohm)

TCR : Sıcaklık katsayısı (PPM/ oC)

R0 : T0 da ölçülen direnç değeri (ohm)

R :T de ölçülen direnç değeri (ohm)

T0 : İlk Sıcaklık (oC)

T :Son sıcaklık (oC)

Örnek: Sıcaklık katsayısı 150 PPM/ oC olan 1Kohm luk bir direncin ortam sıcaklığı 25 oC den 30 oC ‘ye çıkarsa direnç değeri ne kadar değişir.

![Direnc_Okuma_11](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc11.png)

Örnek: TCR değeri 200 PPM/ oC olan 10 Kohm bir direncin 15oC sıcaklık artışında değeri ne olur?

![Direnc_Okuma_12](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc12.png)

Sıcaklık arttığından direnç 30 Ohm azalacaktır.

![Direnc_Okuma_13](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc13.png)

Sarı-Kahverengi-Kırmızı-Turuncu-Kahverengi-Mor 412×1000=412Kohm %1, 5ppm

![Direnc_Okuma_14](https://github.com/imonur/blog/blob/main/projects/images/direnc_okuma/direnc14.png)
