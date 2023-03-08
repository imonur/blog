---
layout: post
title:  "Pandas ile Veri Okuma"
date:   2023-03-07 13:50:39
categories: pandas
---

---
# Pandas ile Veri Okuma
---
Bu yazı, size **Pandas ile Veri Okuma** hakkında bilgi verecektir.

---

Pandas ile veri okuma ve yazma işlemleri oldukça önemlidir ve sıklıkla kullanılır. 
Pandas, birçok veri kaynağından veri okuma ve yazma için yöntemler sağlar. Bu makalede, pandas ile veri okuma ve yazma işlemleri hakkında ayrıntılı bilgi vereceğiz.

**Veri Okuma**

Pandas, birçok veri kaynağından veri okumayı destekler. İşte pandas ile veri okuma için kullanabileceğiniz bazı yöntemler:

**CSV Dosyalarından Okuma**

CSV (comma-separated values) dosyaları, sütunlar arasına virgül konulmuş bir düz metin dosyasıdır ve pandas tarafından kolayca okunabilir.

```s
import pandas as pd

# CSV dosyasından veri okuma
df = pd.read_csv('data.csv')

# İlk 5 satırı görüntüleme
print(df.head())
```

**Excel Dosyalarından Okuma**

Pandas, Excel dosyalarını okumak için read_excel() fonksiyonunu sağlar.

```s
import pandas as pd

# Excel dosyasından veri okuma
df = pd.read_excel('data.xlsx')

# İlk 5 satırı görüntüleme
print(df.head())
```

**SQL Veritabanından Okuma**

Pandas, SQL veritabanlarından veri okumak için read_sql() fonksiyonunu sağlar.

```s

import pandas as pd
import sqlite3

# Veritabanı bağlantısı oluşturma
conn = sqlite3.connect('mydatabase.db')

# SQL sorgusu
query = "SELECT * FROM mytable"

# SQL veritabanından veri okuma
df = pd.read_sql(query, conn)

# İlk 5 satırı görüntüleme
print(df.head())

```

**JSON Dosyalarından Okuma**

Pandas, JSON dosyalarını okumak için read_json() fonksiyonunu sağlar.

```s

import pandas as pd

# JSON dosyasından veri okuma
df = pd.read_json('data.json')

# İlk 5 satırı görüntüleme
print(df.head())

```

**Veri Yazma**

Pandas, verileri CSV, Excel, SQL veritabanları ve JSON dosyaları gibi birçok farklı formatta yazmanıza olanak sağlar. İşte pandas ile veri yazmak için kullanabileceğiniz bazı yöntemler:

**CSV Dosyalarına Yazma**

CSV dosyalarına veri yazmak için, to_csv() fonksiyonunu kullanabilirsiniz.

```s

import pandas as pd

# CSV dosyasına veri yazma
df.to_csv('data.csv', index=False)
```

**Excel Dosyalarına Yazma**

Excel dosyalarına veri yazmak için, to_excel() fonksiyonunu kullanabilirsiniz.

```s
import pandas as pd

# Excel dosyasına veri yazma
df.to_excel('data.xlsx', index=False)
```

**SQL Veritabanına Yazma**

SQL veritabanına veri yazmak için, pandas to_sql() fonksiyonunu kullanabilir
