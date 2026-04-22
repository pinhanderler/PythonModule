# Degiskenler

### Python'da Değişkenlerin Temel Kavramları

Değişkenler, verileri depolamak ve işlemek için kullanılan temel yapı taşlarıdır. Python'da değişkenler tanımlamak oldukça basittir. Bir değişkeni tanımlamak için isim belirleyip değer atamalısınız. İşte temel kullanımı:

```python
# Değişken tanımlama ve değer atama
isim = "Ahmet"
yas = 25
pi = 3.14
```

Yukarıdaki örnekte `isim`, `yas` ve `pi` değişkenlerine sırasıyla bir metin, bir tamsayı ve bir ondalık sayı atandı.

Python'da değişkenlerin özellikleri şunlardır:

### 1. Değişken İsimleri

Python'da değişken isimlendirmesi yaparken bazı kurallara uymanız gerekmektedir. Bu kurallar, kodunuzun daha anlaşılır ve hatasız olmasını sağlar. İşte Python'da değişken isimlendirmesi için geçerli olan temel kurallar:

1. Değişken isimleri harf (A-Z veya a-z) veya alt çizgi (\_) ile başlamalıdır. Rakam ile başlayamazlar.
2. İsimlerde harf (A-Z veya a-z), rakam (0-9) veya alt çizgi (\_) kullanılabilir.
3. Python büyük küçük harf duyarlı bir dildir. Yani `isim` ve `Isim` farklı değişken isimleridir.
4. Python anahtar kelimeleri (reserved keywords) değişken ismi olarak kullanılamaz. Örneğin `if`, `else`, `while`, `for`, `def`, vb.
5. Değişken isimleri anlamlı ve açıklayıcı olmalıdır. Diğer geliştiricilerin kodunuzu daha iyi anlamasına yardımcı olacak şekilde isimlendirin.
6. İsimler boşluk veya özel karakterler içeremez. Sadece harf, rakam ve alt çizgi kullanılabilir.
7. Uzun değişken isimleri için snake\_case veya camelCase gibi isimlendirme stilleri tercih edilir. snake\_case, kelimeleri küçük harfle ve alt çizgi ile ayırarak yazmayı ifade eder. camelCase ise ilk kelimenin küçük harfle ve sonraki kelimelerin büyük harfle başlamasını ifade eder.

Örnekler:

```python
# Geçerli değişken isimleri
isim = "Ahmet"
yas = 25
not_ortalamasi = 85.5
toplam_kisi_sayisi = 100

# Geçersiz değişken isimleri
5_yil = 5  # Rakamla başlayamaz
if = 10   # Anahtar kelime kullanılamaz
adi soyadi = "Ali Veli"  # Boşluk içeremez
```

Bu kurallara uyarak değişken isimleri oluşturduğunuzda, kodunuzun daha okunaklı ve anlaşılır olmasını sağlarsınız..

Python'da anahtar kelimeler (reserved keywords), özel anlamlara sahip olan ve belirli görevleri yerine getiren kelimelerdir. Bu anahtar kelimeler, Python dilinin sözdizimini ve semantiğini belirleyen yapı taşlarıdır ve değişken veya fonksiyon adları olarak kullanılamazlar. İşte Python'da kullanılamayan anahtar kelimeler:

```python
False      class      finally    is         return
None       continue   for        lambda     try
True       def        from       nonlocal   while
and        del        global     not        with
as         elif       if         or         yield
assert     else       import     pass
break      except     in         raise

```

**Çok Kelimeli Değişken Adları**

Evet, Python'da bir değişken adını birden fazla kelime içerecek şekilde oluşturmanın farklı yaklaşımları bulunur. İşte bunlardan ikisi:

1. **Snake Case:** Bu yaklaşımda, kelimeleri küçük harfle yazıp aralarına alt çizgi (\_) karakteri koyarak değişken adını oluşturursunuz.

```python
not_ortalamasi = 85.5
ogrenci_ad_soyad = "Ahmet Yılmaz"
```

2. **Camel Case:** Bu yaklaşımda, ilk kelimenin küçük harfle, sonraki kelimelerin ise büyük harfle başladığı bir yapı kullanırsınız.

```python
notOrtalamasi = 85.5
ogrenciAdSoyad = "Ahmet Yılmaz"
```

Her iki yaklaşım da geçerlidir ve tercihe bağlıdır. Ancak Python topluluğunda daha yaygın olan yaklaşım genellikle "snake\_case" isimlendirmedir. Bu yaklaşım daha fazla kullanılır ve Python kütüphaneleri, standart kütüphane ve pek çok kaynak bu şekilde isimlendirilmiştir.

Unutmayın ki, hangi yaklaşımı kullanırsanız kullanın, değişken isimlerinizin anlamlı, açıklayıcı ve diğer geliştiricilerin kodunuzu daha iyi anlamasına yardımcı olacak şekilde oluşturulması önemlidir.

### 2. Değişken Türleri

Python'da değişkenlerin türleri otomatik olarak belirlenir. Yani türü belirtmenize gerek yoktur. Temel veri tipleri şunlardır:

* `int` (tamsayı)
* `float` (ondalık sayı)
* `str` (metin)
* `bool` (mantıksal değer - True veya False)

Örnek:

```python
yas = 25        # int
not_ortalamasi = 85.5   # float
isim = "Ahmet"  # str
dogru_mu = True  # bool
```

### 3. Değişkenleri Kullanma

**Degiskene Deger Atama**

Python'da bir değişkene değer atamak oldukça basittir. Değişken tanımladıktan sonra, ona istediğiniz değeri atayabilirsiniz. İşte birkaç örnek:

1. **Tamsayı Değer Atama:**

```python
x = 10
```

2. **Ondalık Sayı Değer Atama:**

```python
pi = 3.14
```

3. **Metin Değer Atama:**

```python
isim = "Ahmet"
```

4. **Mantıksal Değer Atama:**

```python
dogru_mu = True
```

5. **Değişkenler Arası Değer Atama:**

```python
x = 5
y = x  # x'in değerini y'ye atadık
```

6. **İfade Sonuçlarını Atama:**

```python
a = 5
b = 10
toplam = a + b  # İfadelerin sonuçlarını atayabilirsiniz
```

7. **Değerleri Değiştirme:**

```python
x = 5
y = 10

x, y = y, x  # x ve y değişkenlerinin değerlerini değiştirdik
```

Bu örneklerde görüldüğü gibi, bir değişkeni tanımladıktan sonra direkt olarak değer atayabilirsiniz. Python dinamik bir dil olduğu için, değişkenin türünü önceden belirtmeniz gerekmez. Değer ataması yaptığınızda Python otomatik olarak değişkenin türünü belirler.

**Bir Degiskene Farkli Deger Atama**

Python'da bir değişkenin değerini değiştirmek oldukça kolaydır. Değişkeni yeni bir değerle güncellemek için sadece atama işlemini tekrarlayabilirsiniz. İşte birkaç örnek:

```python
x = 5
print("x'in ilk değeri:", x)

x = 10  # x'in değerini güncelledik
print("x'in güncellenmiş değeri:", x)

y = 2
y = y + 3  # y değişkeninin değerini güncelledik (yeni değer: 5)
print("y'nin güncellenmiş değeri:", y)

z = 7
z += 1  # z'nin değerini 1 artırdık (yeni değer: 8)
print("z'nin güncellenmiş değeri:", z)
```

Yukarıdaki örneklerde görüldüğü gibi, bir değişkenin değerini güncellemek için sadece yeni bir değer ataması yapmanız yeterlidir. Ayrıca, kısa formlar kullanarak (örneğin `+=`, `-=`) bir değişkenin değerini artırabilir veya azaltabilirsiniz.

**Değerleri Değiştirme ile Birden Fazla Değişkene Değer Atama:**

```python
x = 10
y = 5
x, y = y, x  # x ve y değişkenlerinin değerlerini değiştirdik
```

Bu şekilde, tek satırda birden fazla değişkeni ve değerini eşleştirerek atayabilirsiniz. Önemli olan, değişken sayısıyla veri sayısının eşleşmesidir. Aksi halde hata alabilirsiniz.

**Birden Fazla Degiskene Tek Satirda Deger Atama**

Python, tek satırda birden fazla değişkene değer atamanıza olanak tanır:

```
a, b, c = 5, 3.2, "Hello"

print (a)
print (b)
print (c)
```

```
5
3.2
Hello
```

**Not:** Değişken sayısının değer sayısıyla eşleştiğinden emin olun, aksi takdirde hata alırsınız.

**Bir Degeri Birden Fazla Degiskene Tek Seferde Atama**

Aynı anda birden fazla değişkene aynı değeri atamak istiyorsak bunu şu şekilde yapabiliriz:

```python

x = y = z = "same"

print (x)
print (y)
print (z)
```

```python
same
same
same
```

Yukarıdaki programda x, y ve z değişkenlerinin tümüne aynı dizeyi atar.

Değişkenleri kullanarak matematiksel işlemler yapabilirsiniz:

```python
a = 10
b = 5
toplam = a + b
carpim = a * b
bolum = a / b
```

\-----------------------------------------------------------------------------------------------------