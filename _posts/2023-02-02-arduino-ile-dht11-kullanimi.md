---
layout: post
title:  Arduino ile DHT11 Kullanımı
date:   2023-02-02 13:50:39
categories: coding
---
# Arduino ile DHT11 Kullanımı
---
Bu yazı, size **DHT11**'i Arduino ile nasıl kullanacağınızı gösterecek.

---

## Bileşenler ve Sarf Malzemeleri
---

|	Sıra		|| |	Bileşen			                                  | ||  Adet  |
|--------	|| |----------------------------------------------| ||--------|	
|   1     || | DHT11 Temperature & Humidity Sensor (3 pins)  | ||    1   |
|	  2   	|| | Jumper wires (generic)	                      | ||	   4   |
|	  3   	|| | Arduino UNO	                                  | || 	 2   |
|	  4   	|| | Breadboard (generic)	                        | ||	   1   |

---

## Proje Açıklaması

Çevrenizdeki hava sıcaklığının ve nem oranının ne kadar olduğunu öğrenmek için **DHT11** sensörünü kullanıyoruz. Bu projede kullanacağımız malzemeleri [STEM Kits](https://www.stemkits.net/)'ten satın alabilirsiniz.

---
## Bağlantı Şeması

Sensörümüzün, Arduino ile bağlantısı şu şekilde olacaktır. Bazı **DHT11** sensörleri 3 bacaklı iken bazıları 4 bacaklıdır. Eğer sizin kullandığınız sensör 4 bacaklı ise bir bacak şemada görüldüğü gibi boşta olacak şekilde bağlantısı kurulmalıdır.

![DHT11 Bağlantısı](https://raw.githubusercontent.com/imonur/blog/main/projects/images/dht11_projects_1/dht11_projects_schema.png)

---
### Kod Yapısı

{% highlight python %}
#include <dht11.h>
#define DHT11PIN 4

dht11 DHT11;

void   setup()
{
  Serial.begin(9600);
 
}

void loop()
{
  Serial.println();

   int chk = DHT11.read(DHT11PIN);

  Serial.print("Humidity (%): ");
   Serial.println((float)DHT11.humidity, 2);

  Serial.print("Temperature   (C): ");
  Serial.println((float)DHT11.temperature, 2);

  delay(2000);

}
{% endhighlight %}

---

Bu projeyi [STEM Kits](https://www.stemkits.net/arduino-bluetooth-2wd-arac-kiti-kod-19/)'ten satın alabilirsiniz. Eğer bu çalışmayı beğendiyseniz, destek olmak için bizleri sosyal medyada takip edebilir ve arkadaşlarınıza tavsiye edebilirsiniz.

---

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
