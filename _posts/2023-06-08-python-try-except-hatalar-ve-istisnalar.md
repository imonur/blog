---
layout: post
title:  "Python'da Hatalar ve İstisnalar Konusu ( try-except bloğu )"
date:   2023-06-08 13:50:39
categories: python
---

---
# Python'da Hatalar ve İstisnalar Konusu ( try-except bloğu )
---
Bu yazıda, **Python'da Hatalar ve İstisnalar Konusunu ( try-except bloğu )** bulacaksınız.

---
## Giriş

Bir programcı olarak, yazdığınız kodun her zaman sorunsuz çalışmasını ve beklenmedik hatalarla karşılaşılmamasını umarsınız. Ancak, bazen beklenmedik durumlar ortaya çıkabilir ve kodunuz çalışırken hatalar meydana gelebilir. İşte bu noktada Python'daki "try-except" ifadesi devreye girer. "try-except" ifadesi, programınızın hata oluşturan kod bloklarını ele almasına ve uygun şekilde tepki vermesine olanak tanır.

---
## try-except Bloğu Nedir?

Python'da "try-except" ifadesi, bir bloğun içinde potansiyel hata üretebilecek kodu denemek ve bu hataları ele almak için kullanılır. "try" bloğunda yer alan kodlar çalıştırıldığında herhangi bir hata oluşursa, program "except" bloğuna geçer ve burada tanımlanan hata yönetimi işlemlerini gerçekleştirir.

---
## try-except Bloğunun Yapısı:

```s
try:
# Hataya sebep verecek kodlar
except Hata1:
# Hata1 ile ilgili hata yönetimi işlemleri
except Hata2:
# Hata2 ile ilgili hata yönetimi işlemleri
...
else:
# Hata oluşmazsa çalışacak kodlar
```

try bloğunda hata oluşturabilecek olan kodlar yer alır. Eğer bir hata oluşursa, program except bloğuna geçer ve ilgili hata adıyla eşleşen except bloğunda tanımlanan hata yönetimi işlemlerini gerçekleştirir. Birden fazla except bloğu kullanarak farklı hata türlerine özgü hata yönetimi işlemleri tanımlayabilirsiniz. Ayrıca, bir hata oluşmazsa çalışacak kodları else bloğu içine de yazabilirsiniz.

---
## try-except Bloğu Kullanımı:

Aşağıda, bir dosyayı açmak ve dosyadaki içeriği okumak için try-except bloğunu kullanarak örnek bir kod parçası bulunmaktadır:

```s
try:
    dosya = open("dosya.txt", "r")
    icerik = dosya.read()
    print(icerik)
    dosya.close()
    except FileNotFoundError:
        print("Dosya bulunamadı.")
        except IOError:
            print("Dosya okunurken bir hata oluştu.")
            else:
                print("Dosya okuma işlemi başarıyla tamamlandı.")

```

Bu örnekte, try bloğu içinde dosya açma, içeriği okuma ve ekrana yazdırma işlemleri gerçekleştirilmektedir. Eğer dosya bulunamazsa FileNotFoundError türünde bir hata oluşacak ve bu durumda except FileNotFoundError bloğu çalışacaktır. Benzer şekilde, dosya okunurken bir hata oluşursa IOError türünde bir hata yakalanacak ve except IOError bloğu çalışacaktır. Her iki durumda da dosya.close() ifadesi except bloğu içinde yer almasa bile çalıştırılır. Eğer herhangi bir hata oluşmazsa, else bloğu çalışacak ve "Dosya okuma işlemi başarıyla tamamlandı." mesajı ekrana yazdırılacaktır.

**Sonuç:**

Python'da "try-except" ifadesi, programınızın hata oluşturan kodları yönetmesine ve beklenmedik hatalarla başa çıkmasına yardımcı olan önemli bir araçtır. Bu makalede, try-except bloğunun temel yapısını ve kullanımını açıkladık. try-except ifadesini kullanarak kodunuzu daha güvenli ve sağlam hale getirebilir ve kullanıcı dostu hata mesajları sunabilirsiniz. Hatalarla başa çıkmak için farklı hata türlerine özgü except blokları oluşturabilir ve uygun hata yönetimi işlemleri gerçekleştirebilirsiniz.

Unutmayın, hatalar programlama sürecinin doğal bir parçasıdır ve doğru bir şekilde ele alınarak daha sağlam bir yazılım geliştirmenize yardımcı olurlar. try-except ifadesini kullanarak programınızın hata toleransını artırabilir ve daha güvenilir bir kod tabanı oluşturabilirsiniz.
