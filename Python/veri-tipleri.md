---
layout: default
title: Veri Tipleri
parent: Python Dersleri
nav_order: 3
permalink: /python/veri-tipleri
---

# Python Veri Tipleri
Programlama öğrenirken o dile ait veri veya değişken tiplerini bilmek önemlidir.
Hangi tiple hangi işlemlerin yapılabileceği kavranmalı ve o tiplere ait bazı metod ve özellikler bilinmelidir.
Python'da Veri tipleri aşağıdaki şekildedir:

```
Metin        : str
Sayısal      : int, float, complex
Sıra (dizi)  : list, tuple, range
Mapping      : dict
Set          : set, frozenset
Boolean      : bool
Binary Types : bytes, bytearray, memoryview


```

Daha kolay öğrenebilmek için aşağıdaki şekilde kategorize etmenin  bir sakıncası yoktur.
Python'da veri tipleri genel olarak 4 kategoriye ayrılır: 

````
1- Metin  : str
2- Sayısal: int, float, complex
3- Liste  : list, tuple, range, dict, set, frozenset
4- Diğer  : bool, bytes, bytearray, memoryview
````

### Örnek


````
ÖRNEK                                     VERİ TİPİ
a = "Zafer Demirkol"                         str
a = 14                                       int
a = 14.8                                     float
a = 2j                                       complex
a = ["Mart", "Nisan", "Mayıs"]               list
a = ("Mart", "Nisan", "Mayıs")               tuple
a = range(5)                                 range
a = {"ad": "zafer", "yaş": 51}               dict
a = {"Mart", "Nisan", "Mayıs"}               set
a = ({"Mart", "Nisan", "Mayıs"})             frozenset
a = True                                     bool
a = b"Hello"                                 bytes
a = bytearray(6)                             bytearray
x = memoryview(bytes(6))                     memoryview 
````

Devam eden bölümde ağırlıklı olarak metin, sayı ve liste değişkenlerinin kullanımına ait farklı örnekler verilecek.