---
layout: default
title: Sanal Ortam Oluşturma
parent: Python Dersleri
nav_order: 3
permalink: /python/sanal-ortam-olusturma-linux
---

# Linux (Ubuntu) için Python'da Sanal Çalışma Alanı Oluşturma

Python’da sanal çalışma ortamları oluşturabilirsiniz.
Sanal ortam oluşturmanın amacı, çalıştığınız ortamın paketlerini ve koşullarını global(ana) ortamdan ayırmaktır.

Böylece kendinize yalıtılmış bir alan oluşturur ve ana sistemin veya diğer ortamların paketlerinden bağımsız kendi çalışma ortamınızı oluşturabilirsiniz.

Python yoğun bir şekilde programsal kütüphaneler, modüller ve/veya paketler kullanan bir dildir. Her bir konuya ait paket/modül ve sürümleri farklı olabilir.

Eğer belirli paketler ve onların sürümlerinden oluşan bir alan yaratmak isterseniz aşağıdaki komutlarla bu mümkün. Böylece hem global paketlerinizi bozmamış olursunuz, hem de kendi sanal ortamınızda istediğiniz paketlerle uygulama geliştirebilirsiniz.

Linux Ubuntu 'da Sanal ortam oluşturmak için şunların olması gerekir:

```bash
Python > 3.4 ve pip >= 19.0

python3 --version
pip3 --version
virtualenv --version

#eğer virtualenv kurulu değilse

> sudo apt update
> sudo apt install python3-dev python3-pip
> sudo pip3 install -U virtualenv  # system-wide install

# Sanal ortamı oluşturmak burada "sanalOrtam" isminde bir klasör oluşturup alan için gereken dosya, klasörleri oluşturur

> virtualenv --system-site-packages -p python3 ./sanalOrtam

# oluşturduğu klasörler içinde bir "bin" isminde bir klasör vardır ve onun içinde "activate" isminde bir dosya bulunur, bunu çalıştırmalıyız:

> source ./sanalOrtam/bin/activate

# Artık sanal ortamımız aktif hale gelmiştir. Komut satırında sanal ortamımızın ismi parantez içinde yazar. Bunun anlamı, artı python komutlarını bu ortamda veriyoruz, bu ortamın paket ve/veya modüllerini kullanabiliyoruz. Yine bu ortama paket ve/veya modüller ekliyoruz demektir.

> (sanalOrtam) (base) zafer@ubuntu:~$

# Ana sistem kurulumunu etkilemeden paketleri sanal bir ortama kurmak.

> pip install --upgrade pip

# yüklü paketleri görmek için:

> pip list

# Sanal ortamdan çıkmak için "deactivate" komutu kullanılır:

> deactivate


# Yeni bir paket yüklemek için örneğin TensorFlow 2

> pip install --upgrade tensorflow

> import tensorflow as tf
> print (tf.__version__)


# Eğer sanal ortama jupyter notebook'da yüklemek istiyorsanız

> pip install -I jupyter

# Aşağıdaki sorgulamalar yapılarak sistemde kurulu ortamların yol tanımları elde edilebilir
which python
which ipython

```
