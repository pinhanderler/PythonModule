# Veri Tipleri

### Python'da Temel Veri Tipleri

\
Python'da kullanılan temel veri tipleri ve kısa açıklamaları Türkçe olarak:

1. **Tamsayı (int):** Tüm tam sayı değerlerini temsil eder. Örneğin: 1, -5, 1000 gibi.
2. **Ondalık Sayı (float):** Ondalık kesirli sayıları temsil eder. Örneğin: 3.14, -0.5 gibi.
3. **Metin (str):** Metin veya karakter dizilerini temsil eder. Örneğin: "Merhaba", 'Python', "123" gibi.
4. **Mantıksal (bool):** Doğru veya yanlış değerleri temsil eder. Yalnızca iki değeri vardır: True (doğru) veya False (yanlış).
5. **Liste (list):** Birden çok değeri sıralı olarak depolamak için kullanılır. Farklı türde verileri içerebilir.
6. **Demet (tuple):** Liste ile benzerdir, ancak değerler değiştirilemez. Genellikle sabit verileri saklamak için kullanılır.
7. **Sözlük (dict):** Anahtar-değer çiftleriyle verileri depolamak için kullanılır. Anahtarlar benzersiz olmalıdır.
8. **Kümeler (set):** Benzersiz ve sırasız verileri depolamak için kullanılır. Matematiksel kümeler gibi işlemler yapabilirler.
9. **Dizi (array):** Nümerik verileri çok boyutlu diziler şeklinde saklamak ve işlemek için kullanılır. NumPy kütüphanesi ile sağlanır.
10. **Karşılaştırma (comparable):** Sıralanabilir (sortable) verileri saklamak için kullanılır. Özel bir veri tipi değildir, ancak sıralama işlemleri için kullanılan bir kavramdır.

Bu temel veri tipleri, Python'da kullanılan en yaygın ve temel veri tipleridir. Python'un esnek yapısı sayesinde, bu temel veri tiplerini kombinleyerek daha karmaşık yapılar oluşturabilirsiniz.

Python programlamada, çeşitli veri tipleri farklı türdeki verileri temsil etmek için kullanılır. Veri tipleri, programın çalışma şekli ve verilerin işlenmesi konusunda önemli bir rol oynar.

Baslangic olarak bu veri tiplerinden bazilarini inceleyecegiz.

### 1. Sayısal Veri Tipleri

#### a. Tamsayı (int)

Tamsayılar, kesirli olmayan sayıları temsil eder. Örnek:

```python
yas = 25
ogrenci_sayisi = 100
```

#### b. Ondalık Sayı (float)

Ondalık sayılar, kesirli sayıları temsil eder. Örnek:

```python
pi = 3.14
fiyat = 19.99
```

### 2. Metinsel Veri Tipi

#### Metin (str)

Metin veri tipi, metin veya karakter dizilerini temsil eder. Metinler tek tırnak (`'`) veya çift tırnak (`"`) içinde tanımlanabilir. Örnek:

```python
isim = "Ahmet"
soyisim = 'Yılmaz'
```

### 3. Mantıksal Veri Tipi

#### Mantıksal (bool)

Mantıksal veri tipi, doğru (`True`) veya yanlış (`False`) değerleri temsil eder. Genellikle koşullu ifadelerde ve karar yapılarında kullanılır. Örnek:

```python
dogru_mu = True
yanlis_mi = False
```

Bu veri tipleri temel olarak Python programlamada kullanılan en temel veri tipleridir. Ancak daha karmaşık veri tipleri de vardır, örneğin:

* **Listeler**: Birden çok veriyi sıralı bir şekilde depolamak için kullanılır.
* **Demetler (Tuples)**: Listelere benzer, ancak değiştirilemez.
* **Sözlükler (Dictionaries)**: Anahtar-değer çiftleri ile veri depolar.
* **Kümeler (Sets)**: Benzersiz ve sırasız verileri depolamak için kullanılır.

Bu veri tipleri hakkında daha fazla bilgi almak ve daha karmaşık konuları öğrenmek için Python belgelerine ve diğer kaynaklara başvurabilirsiniz.

Python'da bir verinin türünü öğrenmek için `type()` fonksiyonunu kullanabilirsiniz. Bu fonksiyon, bir nesnenin (değişkenin veya değerin) veri tipini döndürür. İşte `type()` fonksiyonunun kullanımı:

```python

x = 5
print(type(x))  # <class 'int'>

isim = "Ahmet"
print(type(isim))  # <class 'str'>

pi = 3.14
print(type(pi))  # <class 'float'>

dogru_mu = True
print(type(dogru_mu))  # <class 'bool'>
```

Bu örnekte, `type()` fonksiyonu, `x` değişkeninin tamsayı (`int`) veri tipine ait olduğunu, `isim` değişkeninin metin (`str`) veri tipine ait olduğunu vb. döndürmektedir. Bu sayede bir verinin türünü belirleyebilir ve programınızı geliştirirken kullanabilirsiniz.

Python'da, bir değişkene atanan degerlerin veri türü listesi:

![](broken-reference)

Python'da bir değişkenin veri tipini değiştirmek, genellikle dönüştürme işlemi ile yapılır. Bu işlem, mevcut bir değeri başka bir veri türüne dönüştürmek anlamına gelir. Python'da veri tipi dönüşümü için bazı fonksiyonlar bulunur. İşte bazı örnekler:

1. **Tamsayıya Dönüştürme (int):**

```python
sayi = "123"
sayi_int = int(sayi)
print(sayi_int)  # 123
```

2. **Ondalık Sayıya Dönüştürme (float):**

```python
ondalik_sayi = "3.14"
ondalik_sayi_float = float(ondalik_sayi)
print(ondalik_sayi_float)  # 3.14
```

3. **Metne Dönüştürme (str):**

<pre class="language-python"><code class="lang-python"><strong>sayi = 123
</strong>sayi_str = str(sayi)
print(sayi_str)  # "123"
</code></pre>

4. **Mantıksal Değer Dönüşümü (bool):**

```python
sayi = 0
sayi_bool = bool(sayi)
print(sayi_bool)  # False
```

Dönüşüm işlemleri, veri türleri arasındaki uygunluğa dikkat ederek gerçekleştirilmelidir. Örneğin, bir metin içinde sadece rakam olan bir değeri tamsayıya dönüştürmek mümkündür, ancak metin içerisinde harf bulunuyorsa dönüşüm hata verebilir.

\-----------------------------------------------------------------------------------------------------
