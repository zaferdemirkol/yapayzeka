---
layout: default
title: Markdown
nav_order: 2
has_children: false
permalink: /markdown
---

# Markdown

Markdown, web üzerinde metin biçimlendirmenin bir yöntemidir. Aynen HTML gibi ama daha az bildirime ve daha kolay bir kullanıma sahiptir. Özellikle GitHub, Jupyter Notebook gibi programsal arabirimlerde yaygın olarak kullanılıyor.

Bir metni bold, italik yazmak, resim, başlık eklemek, listeler, tablolar ve bunun gibi biçimsel görünümler oluşturmak istiyorsanız Markdown kullanımı son derece basittir.

# Başlıklar

Bir metni başlık olarak yazmak için başına # işaretleri koymalısınız, koyacağınız # sayısı kadar başlık büyüklüğü değişmektedir.

```markdown
# Bu başlık ifadesi <h1> e eşittir

## Bu başlık ifadesi <h2> e eşittir

###### Bu başlık ifadesi <h6> e eşittir
```

# Vurgular (Emphasis)

Bir metni kalın (bold) veya eğik (italic) yazmak için aşağıdaki ifadeler kullanılır:

Eğik metin yazdırmak için başına ve sonuna \* veya \_ konur:

```
*Bu metin eğik(italic) yazılır*

_Bu şekilde de eğik(italic) yazdırabilirsiniz_

```

Kalın (Bold) metin yazdırmak için başına ve sonuna \*\* veya \_\_ konur:

```
**Bu metin kalın(bold) yazılır**

__Bu metin de kalın(bold) yazılır__

```

İkisini bir arada kullanabilirsiniz:

`_Bu hem eğik hem de **burası kalın(bold)** yazılmış bir metindir_`

# Listeler

Sıralı veya sırasız listeler oluşturabilirsiniz.

### Sırasız liste:

```
* Birim 1
* Birim 2
  * Birim 2a
  * Birim 2b
```

```
- Birim 1
- Birim 2
  - Birim 2a
  - Birim 2b
```

### Sıralı liste:

```
1. Birim 1
2. Birim 2
    1. Birim 2a
    2. Birim 2b
3. Birim 3

```

1. Birim 1
2. Birim 2
   1. Birim 2a
   2. Birim 2b
3. Birim 3
