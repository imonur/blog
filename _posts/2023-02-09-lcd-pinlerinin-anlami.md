---
layout: post
title:  "LCD Pinlerinin Anlamı"
date:   2023-02-02 13:50:39
categories: coding
---
---
# LCD Pinlerinin Anlamı
---
Bu yazı, size **LCD Pinlerinin Anlamını** gösterecektir.

---
![LCD_Pinlerini_Okuma](https://raw.githubusercontent.com/imonur/blog/main/projects/images/lcd_pinleri_okuma/lcd_pinleri_okuma.png)
---

| **Sıra** | **Kısa Adı**        | **Açıklaması**                                                                                           |
|:--------:|---------------------|----------------------------------------------------------------------------------------------------------|
|     1    | VSS Girişi          | GND girişidir. Negatif gerilim bağlanır.                                                                 |
|     2    | VDD(5V) Girişi      | 5 volt pozitif gerilim bağlanır.                                                                         |
|     3    | VE Girişi           | Ekrandaki yazının netliğini ayarlamak için kullanılan voltaj girişidir.                                  |
|     4    | RS(Register Select) | LCD ekranın ne yapacağını, register da bir değer olup olmadığını kontrol eder.                           |
|     5    | R/W(Read/Write)     | Pinlerin modlarını okuma veya yazma olarak değiştirmek için kullanılır                                   |
|     6    | E (Enable)          | Pinleri okuma modunda aktif hale getirir                                                                 |
|  7 - 14  | D0 – D7             | Bit olarak aldığı değerleri okur. Buradan ekrana yazdırılacak yazılar bit olarak  gönderilir.      |
|  15 - 16 | Cathode - Anode     | Sonda bulunan bu iki girişe + ve – olmak üzere voltaj uygulanır. Bu sayede LCD'nin arka plan ışığı yanar veya söner. |

---
