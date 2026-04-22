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

\-----------------------------------------------------------------------------------------------------# Dictionaries

### Dictionary nedir?


Python'da dictionary (sözlük), anahtar-değer çiftlerini saklayan bir veri yapısıdır. Her bir anahtar, bir değeri ilişkilendiren bir indeks görevi görür. Dictionary'ler, birçok programlama dilinde "harita", "hash tablosu" veya "associative array" olarak da adlandırılırlar.

Dictionary'lerin anahtar(key) özellikleri:

1. **Anahtarlar Benzersizdir:** Her bir anahtar, dictionary içinde yalnızca bir defa bulunabilir. Aynı anahtara sahip iki çift eklenemez.
2. **Değiştirilebilir (Mutable) Veri Yapısı:** Dictionary'ler, eklenen, değiştirilen veya silinen anahtar(key)-değer(value) çiftleri ile dinamik olarak güncellenebilir.
3. **Sırasız (Unordered) Veri Yapısı:** Python 3.7 ve sonraki sürümlerden itibaren dictionary'lerde ekleme sırası korunur. Ancak, dictionary'lerin içeriği sırasızdır ve indeksleme kullanılamaz.

Dictionary'ler, birçok farklı veri türünü gruplamak veya ilişkilendirmek için kullanışlıdır. Örneğin, bir kişinin adını, yaşını ve e-posta adresini saklayabilirsiniz.

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}
```

Bu örnekte, `person` adlı dictionary, "name", "age" ve "email" adlı anahtarları ilgili değerlerle ilişkilendirir.

### Dictionary nasıl oluşturulur?

Python'da dictionary (sözlük) oluşturmanın farklı yolları bulunmaktadır. İşte bu yöntemlerden bazıları:

**1. Süslü Parantezler `{}` ile Dictionary Oluşturma:**

```python
person = {
    "name": "Mike",
    "age": 60,
    "email": "mikejones@example.com"
}
```

Bu yöntemle süslü parantezler içine anahtar-değer çiftlerini yazarak bir dictionary oluşturabilirsiniz.

**2. dict() Fonksiyonu ile Dictionary Oluşturma:**

```python
person = dict(name="John", age=30, email="john@example.com")
```

`dict()` fonksiyonu kullanarak anahtarları ve değerleri argümanlar olarak geçerek bir dictionary oluşturabilirsiniz.

**3. Liste ve Tuple Kullanarak Dictionary Oluşturma:**

```python
keys = ["name", "age", "email"]
values = ["John", 30, "john@example.com"]
person = dict(zip(keys, values))
```

`zip()` fonksiyonu ile anahtarları ve değerleri içeren liste veya tuple'ları birleştirerek dictionary oluşturabilirsiniz.

**4. fromkeys() Metodu ile Anahtarları Değerle İlişkilendirme:**

```python
keys = ["name", "age", "email"]
default_value = "N/A"
person = dict.fromkeys(keys, default_value)
```

`fromkeys()` metodu, belirtilen anahtarları belirtilen varsayılan değerle ilişkilendiren bir dictionary oluşturmanızı sağlar.

Bu yöntemler, dictionary oluşturmanın farklı yollarını gösterir. Hangi yöntemi kullanırsanız kullanın, anahtarlar benzersiz olmalıdır ve dictionary'lerde anahtarlar sırasız (unordered) olarak saklanır.

### Dictionary Örnekleri:

Dictionary içerisinde farklı veri tiplerine sahip değerler kullanabileceğiniz bazı örnekler aşağıda verilmiştir:

**1. String ve Sayılar:**

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}
```

**2. Liste ve Tuple:**

```python
student = {
    "name": "Alice",
    "grades": [85, 90, 78, 95],
    "info": ("Computer Science", "Sophomore")
}
```

**3. Nested Dictionary:**

```python
school = {
    "name": "XYZ School",
    "location": "City A",
    "students": {
        "Alice": {
            "age": 16,
            "grade": 11
        },
        "Bob": {
            "age": 17,
            "grade": 12
        }
    }
}
```

**4. Bool ve None:**

```python
settings = {
    "debug_mode": True,
    "logging": False,
    "api_key": None
}
```

**5. Karışık Veri Tipleri:**

```python
data = {
    "name": "Jane",
    "age": 28,
    "scores": [95, 88, 72],
    "info": {
        "city": "New York",
        "country": "USA"
    }
}
```

Bu örneklerde, dictionary içerisinde farklı veri tiplerine sahip değerleri görebilirsiniz. Dictionary'ler, farklı veri tiplerini gruplamak ve ilişkilendirmek için oldukça kullanışlıdır.

### Dictionary içerisindeki elemanlara erişme

Bir Python dictionary'sindeki (sözlük) elemanlara anahtarları kullanarak erişebilirsiniz. İşte bir dictionary'deki elemanlara nasıl erişeceğinize dair örnekler:

```python
person = {
    "name": "John",
    "age": 30,
    "email": "john@example.com"
}

# Anahtarları kullanarak elemanlara erişim
name = person["name"]
age = person["age"]
email = person["email"]

print(name)   # John
print(age)    # 30
print(email)  # john@example.com
```

Bu örnekte, dictionary içindeki elemanlara erişmek için anahtarları kullanıyoruz. Anahtarları kullanarak değerlere erişirken şu noktalara dikkat edin:

1. Eğer belirtilen anahtar dictionary içinde bulunmuyorsa, `KeyError` hatası alırsınız. Bu nedenle, var olmayan bir anahtara erişmeden önce `in` anahtar kelimesini kullanarak kontrol etmek iyi bir uygulamadır.

```python
if "address" in person:
    address = person["address"]
else:
    address = "N/A"
```

2. Eğer anahtarı kontrol etmek yerine `get()` metodunu kullanırsanız, var olmayan bir anahtar için hata almak yerine belirlediğiniz bir varsayılan değer dönebilir.

```python
address = person.get("address", "N/A")
```

Bu şekilde, var olmayan bir anahtar durumunda `address` değeri "N/A" olacaktır.

###

### Bir dictionary içerisine eleman ekleme veya var olan elemanı güncelleme

Python'da bir dictionary'ye (sözlüğe) yeni bir eleman eklemek için mevcut bir anahtarla ilişkilendirilen yeni bir değer atamanız gerekmektedir. İşte bir dictionary'ye eleman eklemek için kullanabileceğiniz yöntemlerden birkaçı:

**1. Mevcut Anahtarla Eleman Güncelleme:**

```python
person = {
    "name": "John",
    "age": 30
}

person["age"] = 31  # "age" anahtarına sahip elemanın değerini güncelleme
```

**2. Yeni Anahtar ve Değer Eklemek:**

```python
person = {
    "name": "John",
    "age": 30
}

person["email"] = "john@example.com"  # Yeni anahtar ve değeri eklemek
```

**3. setdefault() Metodu ile Eleman Eklemek:**

```python
person = {
    "name": "John",
    "age": 30
}

person.setdefault("email", "john@example.com")  # Eğer "email" anahtarı yoksa ekler
```

**4. update() Metodu ile Birden Fazla Eleman Eklemek:**

```python
person = {
    "name": "John",
    "age": 30
}

new_data = {
    "email": "john@example.com",
    "city": "New York"
}

person.update(new_data)  # Birden fazla eleman eklemek
```

Bu yöntemlerden herhangi birini kullanarak bir dictionary'ye yeni bir eleman ekleyebilirsiniz.

### Diğer Dictionary Methodları

Python'da dictionary (sözlük) veri yapısı için kullanabileceğiniz bazı önemli metodları örneklerle açıklamayalım:

**1. keys():** Dictionary içindeki tüm anahtarları bir liste olarak döndürür.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
keys = person.keys()
print(keys)  # dict_keys(['name', 'age', 'email'])
```

**2. values():** Dictionary içindeki tüm değerleri bir liste olarak döndürür.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
values = person.values()
print(values)  # dict_values(['John', 30, 'john@example.com'])
```

**3. items():** Dictionary içindeki tüm anahtar-değer çiftlerini bir liste olarak döndürür.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
items = person.items()
print(items)  # dict_items([('name', 'John'), ('age', 30), ('email', 'john@example.com')])
```

**4. get():** Belirtilen anahtarın değerini döndürür. Eğer anahtar yoksa belirtilen varsayılan değeri döndürür.

```python
person = {"name": "John", "age": 30}
email = person.get("email", "N/A")
print(email)  # N/A
```

**5. pop():** Belirtilen anahtara sahip elemanı çıkarır ve değerini döndürür. Anahtar yoksa belirtilen varsayılan değeri döndürür.

```python
person = {"name": "John", "age": 30}
email = person.pop("email", "N/A")
print(email)  # N/A
```

**6. popitem():** Son eklenen anahtar-değer çiftini çıkarır ve tuple olarak döndürür.

```python
person = {"name": "John", "age": 30, "email": "john@example.com"}
last_item = person.popitem()
print(last_item)  # ('email', 'john@example.com')
```

**7. clear():** Dictionary içeriğini temizler, yalnızca boş bir dictionary bırakır.

```python
person = {"name": "John", "age": 30}
person.clear()
print(person)  # {}
```

**8. copy():** Dictionary'nin bir kopyasını döndürür.

```python
person = {"name": "John", "age": 30}
person_copy = person.copy()
```

Bu metodlar, dictionary veri yapısını işlemek ve manipüle etmek için kullanabileceğiniz bazı önemli araçlardır.

### Dictionary Comprehensions

Dictionary comprehensions, Python'da yeni bir dictionary oluşturmanın hızlı ve kompakt bir yoludur. List comprehensions'a benzer şekilde çalışırlar, ancak sonuç olarak bir dictionary üretirler. Dictionary comprehension kullanarak, mevcut bir iterable'dan (liste, tuple, vb.) anahtar-değer çiftleri oluşturabilirsiniz.

Dictionary comprehension yapısı şu şekildedir:

```python
new_dict = {key_expression: value_expression for element in iterable}
```

İşte birkaç örnek:

**1. Kareler Dictionary'si:**

```python
numbers = [1, 2, 3, 4, 5]
squares_dict = {num: num**2 for num in numbers}
print(squares_dict)  # {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

**2. Harf Sayısı Dictionary'si:**

```python
text = "hello world"
char_count_dict = {char: text.count(char) for char in text}
print(char_count_dict)  # {'h': 1, 'e': 1, 'l': 3, 'o': 2, ' ': 1, 'w': 1, 'r': 1, 'd': 1}
```

**3. Sadece Çift Sayılar Dictionary'si:**

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_dict = {num: num**2 for num in numbers if num % 2 == 0}
print(even_dict)  # {2: 4, 4: 16, 6: 36, 8: 64, 10: 100}
```

Dictionary comprehension kullanarak, daha karmaşık işlemleri tek satırda gerçekleştirebilir ve veriyi farklı bir şekilde gruplayabilirsiniz.

### Bir elemanın Dictionary içerisinde olup olmadığını kontrol etme

\
Bir elemanın bir Python sözlüğü (dict) içinde olup olmadığını kontrol etmek için, `in` anahtar kelimesini kullanabilirsiniz. İşte bunu nasıl yapacağınıza dair bir örnek:

```python
my_dict = {"anahtar1": "değer1", "anahtar2": "değer2", "anahtar3": "değer3"}

aranan_eleman = "anahtar2"

if aranan_eleman in my_dict:
    print(f"{aranan_eleman} sözlükte bulundu: {my_dict[aranan_eleman]}")
else:
    print(f"{aranan_eleman} sözlükte bulunamadı.")
```

Bu örnekte, `aranan_eleman` değişkeninin sözlükte olup olmadığı kontrol ediliyor. Eğer aranan eleman sözlükte bulunuyorsa, sözlükteki değer de ekrana yazdırılıyor. Eğer bulunmuyorsa, bir mesaj yazdırılıyor.

### Bir Dictionary içerisindeki elemanları döngü kullanarak nasıl gezme(Iterating through a Dictionary)

Bir sözlük içinde dolaşmak için Python'da `for` döngüsünü kullanabilirsiniz. Sözlüğün anahtarlarına veya değerlerine erişmek için kullanabileceğiniz iki yaygın yöntem vardır. İşte her iki yöntemin de örnekleri:

1. Anahtarları üzerinde döngü:

```python
my_dict = {"anahtar1": "değer1", "anahtar2": "değer2", "anahtar3": "değer3"}

for anahtar in my_dict:
    deger = my_dict[anahtar]
    print(f"Anahtar: {anahtar}, Değer: {deger}")
```

2. Değerleri üzerinde döngü:

```python
my_dict = {"anahtar1": "değer1", "anahtar2": "değer2", "anahtar3": "değer3"}

for deger in my_dict.values():
    print(f"Değer: {deger}")
```

3. Hem anahtarları hem de değerleri üzerinde döngü:

```python
my_dict = {"anahtar1": "değer1", "anahtar2": "değer2", "anahtar3": "değer3"}

for anahtar, deger in my_dict.items():
    print(f"Anahtar: {anahtar}, Değer: {deger}")
```

Bu örneklerde, `for` döngüsü ile sözlük içindeki öğeleri sırayla dolaşıyoruz. İlk örnekte, her bir döngü adımında anahtarı alıyoruz ve bu anahtarı kullanarak değeri elde ediyoruz. İkinci örnekte, `values()` metodu ile sadece değerlere erişiyoruz. Üçüncü örnekte ise `items()` metodu ile hem anahtarları hem de değerleri alabiliyoruz.

### Dictionary'de  bazı built-in fonksiyonlar(yerleşik işlevler):

Tabii, bazı yerleşik işlevleri ve bu işlevlerin nasıl kullanıldığını örneklerle açıklayalım:

1. `all()`: Verilen bir iterable (liste, demet, vb.) içindeki tüm öğeler `True` değerini döndürüyorsa, `True` döndürür; aksi halde `False` döndürür.

```python
values = [True, True, False, True]
result = all(values)
print(result)  # Çıktı: False
```

2. `any()`: Verilen bir iterable içinde en az bir öğe `True` değerini döndürüyorsa, `True` döndürür; tüm öğeler `False` ise `False` döndürür.

```python
values = [False, False, True, False]
result = any(values)
print(result)  # Çıktı: True
```

3. `len()`: Bir iterable'ın (liste, demet, dize, vb.) uzunluğunu döndürür.

```python
my_list = [1, 2, 3, 4, 5]
length = len(my_list)
print(length)  # Çıktı: 5
```

4. `sorted()`: Bir iterable'ı sıralar ve sıralanmış bir liste döndürür. İlk argüman olarak sıralanacak iterable'ı alır, opsiyonel olarak `reverse` argümanı ile ters sıralama yapılabilir.

```python
my_list = [4, 2, 1, 3, 5]
sorted_list = sorted(my_list)
print(sorted_list)  # Çıktı: [1, 2, 3, 4, 5]
```

# Döngüler

Python'da döngüler, belirli bir işlemi tekrarlamak için kullanılan önemli bir yapıdır. İşte döngülerin farklı türlerini ve örneklerini anlatan birkaç örnek:

### 1. `for` Döngüsü

`for` döngüsü, belirli bir liste, dizi veya dizi benzeri veri yapısı üzerinde dolaşmak için kullanılır.

#### Örnek 1: Liste Elemanlarını Yazdırmak

```python
colors = ["kırmızı", "mavi", "yeşil", "sarı"]

for color in colors:
    print(color)
```

#### Örnek 2: Sayıları Toplamak

```python
numbers = [1, 2, 3, 4, 5]
total = 0

for num in numbers:
    total += num

print("Toplam:", total)
```

### 2. `while` Döngüsü

`while` döngüsü, belirli bir koşul doğru olduğu sürece bir işlemi tekrarlamak için kullanılır.

#### Örnek 3: Sayı Tahmin Oyunu

```python
import random

target_number = random.randint(1, 100)
guess = None

while guess != target_number:
    guess = int(input("Tahmininizi girin: "))
    if guess < target_number:
        print("Daha yüksek bir sayı tahmin edin.")
    elif guess > target_number:
        print("Daha düşük bir sayı tahmin edin.")
    else:
        print("Tebrikler! Doğru tahmin:", target_number)
```

#### Örnek 4: Faktöriyel Hesaplama

```python
number = int(input("Faktöriyelini hesaplamak istediğiniz sayıyı girin: "))
factorial = 1
i = 1

while i <= number:
    factorial *= i
    i += 1

print(f"{number} sayısının faktöriyeli:", factorial)
```

Döngüler, belirli bir görevi tekrarlamak ve veri işlemek için önemli bir araçtır. Örnekler, `for` ve `while` döngülerini kullanarak farklı senaryolarda nasıl kullanabileceğinizi göstermektedir.

İç içe geçmiş döngüler, bir döngü içinde başka bir döngü kullanma anlamına gelir. Bu tür döngüler, daha karmaşık yapılar oluşturmak ve verileri daha derinlemesine işlemek için kullanışlıdır. İşte iç içe geçmiş döngülerin açıklamaları ve örnekleri:

### İç İçe Geçmiş `for` Döngüleri

#### Örnek 1: Çarpım Tablosu

```python
for i in range(1, 6):
    for j in range(1, 6):
        print(i * j, end="\t")
    print()
```

Bu örnekte, 1'den 5'e kadar olan sayıların çarpım tablosunu oluşturuyoruz. İç içe geçmiş iki `for` döngüsü kullanarak her bir çarpım sonucunu yazdırıyoruz.

### İç İçe Geçmiş `while` Döngüleri

#### Örnek 2: Yıldız Üçgen

```python
size = 5
row = 1

while row <= size:
    col = 1
    while col <= row:
        print("*", end="")
        col += 1
    print()
    row += 1
```

Bu örnekte, yıldızlarla oluşturulan üçgen bir desen oluşturuyoruz. İç içe geçmiş iki `while` döngüsü kullanarak yıldızları doğru sırayla yazdırıyoruz.

### Kombine `for` ve `while` Döngüleri

#### Örnek 3: Matris Transpozisyonu

```python
matrix = [[1, 2, 3],
          [4, 5, 6],
          [7, 8, 9]]

transposed = []

for i in range(len(matrix[0])):
    row = []
    for j in range(len(matrix)):
        row.append(matrix[j][i])
    transposed.append(row)

for row in transposed:
    print(row)
```

Bu örnekte, bir matrisin transpozisyonunu hesaplıyoruz. İç içe geçmiş `for` döngüleri kullanarak matrisin sütunlarını satırlara dönüştürüyoruz.

İç içe geçmiş döngüler, daha karmaşık desenler oluşturmak veya verileri daha derinlemesine işlemek için kullanışlıdır. Ancak bu tür döngülerin anlaşılması ve yönetilmesi daha karmaşık olabilir, bu yüzden dikkatli ve mantıklı bir şekilde kullanılmalıdır.

Sonsuz döngüler, bir döngünün belirli bir koşul yerine hiç sonlanmadan sürekli olarak çalıştığı durumlardır. Bu tür döngüler, genellikle programcı hatalarından kaynaklanır ve istem dışı programların takılmasına neden olabilir. Sonsuz döngülerin bir örneğini inceleyelim:

```python
while True:
    print("Bu döngü sonsuz bir döngüdür!")
```

Yukarıdaki örnekte, `while True:` ifadesi sonsuz bir döngü oluşturur. Döngü her zaman doğru olduğu için, içerisindeki kod sürekli olarak çalışacaktır ve program hiçbir zaman bu döngüden çıkamayacaktır. Bu tür bir döngü programın donmasına neden olur.

Sonsuz döngüleri önlemek için, döngü koşullarını doğru bir şekilde ayarlamak veya döngü içerisinde uygun bir çıkış mekanizması kullanmak önemlidir. Örneğin:

```python
while True:
    user_input = input("Çıkmak için 'q' tuşuna basın: ")
    if user_input == 'q':
        break
    else:
        print("Geçersiz giriş.")
```

Yukarıdaki örnekte, kullanıcı "q" tuşuna basana kadar kullanıcıdan giriş alacak bir döngü bulunmaktadır. Kullanıcı "q" tuşuna bastığında `break` ifadesi ile döngü sonlandırılır.

Sonsuz döngülerden kaçınmak ve döngülerinizi mantıklı bir şekilde kontrol etmek, programınızın düzgün çalışmasını sağlamak için önemlidir.

Python'da `for` döngüsü genellikle bir sıralı veri yapısındaki öğeleri tek tek işlemek için kullanılır. Ancak, normalde bir döngüyü sonlandıran bir koşul belirtilmezse, `for` döngüsü sonsuz bir döngü haline gelebilir. Bu duruma "for sonsuz döngüsü" denir.

Sonsuz bir `for` döngüsü örneğine bakalım:

```python
for i in range(5):
    print("Bu döngü sonsuz bir döngüdür!")
```

Burada, normalde `range(5)` ifadesi ile 0'dan 4'e kadar olan sayıları dolaşan bir `for` döngüsü beklenir. Ancak, burada döngünün içinde herhangi bir koşul veya çıkış mekanizması olmadığı için bu döngü sonsuz bir şekilde çalışacaktır.

Bu tür bir hata yapmaktan kaçınmak için, `for` döngülerini kullanırken döngü koşulunu doğru bir şekilde ayarlamak ve döngüyü sonlandıran bir mekanizma sağlamak önemlidir. Örneğin:

```python
for i in range(5):
    user_input = input("Döngüden çıkmak için 'q' tuşuna basın: ")
    if user_input == 'q':
        break
    print(f"{i} işlem tamamlandı.")
```

Burada, kullanıcı "q" tuşuna basarsa `break` ifadesi ile döngü sonlandırılır. Aksi takdirde, her iterasyonda bir işlem gerçekleştirilir.

Sonsuz bir `for` döngüsünden kaçınmak ve döngülerinizi kontrol etmek, programınızın düzgün ve beklenen şekilde çalışmasını sağlamak için önemlidir.

`break` ve `continue`, Python'daki döngülerde kontrol akışını değiştirmek için kullanılan iki anahtar kelimedir. Bu iki ifade, döngülerin davranışını etkiler ve belirli koşullar altında döngüleri durdurmak veya atlamak için kullanılır.

### `break` İfadesi

`break` ifadesi, bir döngüyü aniden sonlandırmak için kullanılır. Eğer belirli bir koşul gerçekleşirse, döngü anında sona erer.

#### Örnek 1: Sayı Tahmin Oyunu

```python
target_number = 42

while True:
    guess = int(input("Tahmininizi girin: "))
    if guess == target_number:
        print("Tebrikler, doğru tahmin!")
        break
    else:
        print("Yanlış tahmin, tekrar deneyin.")
```

Bu örnekte, kullanıcı doğru tahmini yaptığında `break` ifadesi kullanılarak sonsuz `while` döngüsü sonlandırılır.

### `continue` İfadesi

`continue` ifadesi, bir döngü içerisinde belirli bir koşulu sağlayan iterasyonları atlamak için kullanılır. Koşul sağlandığında, döngünün geri kalan kısmı atlanır ve bir sonraki iterasyona geçilir.

#### Örnek 2: Çift Sayıları Yazdırma

```python
for i in range(1, 11):
    if i % 2 == 1:
        continue
    print(i, "çift sayıdır.")
```

Bu örnekte, `continue` ifadesi kullanılarak sadece çift sayılar yazdırılır. Tek sayılar atlanır ve döngünün bir sonraki iterasyonuna geçilir.

`break` ve `continue` ifadeleri, döngülerin içerisinde belirli koşullara bağlı olarak akışı kontrol etmek için kullanışlı araçlardır. Ancak, bu ifadelerin aşırı kullanımı veya karışık bir kod akışı oluşturması kodun anlaşılabilirliğini zorlaştırabilir. Bu yüzden dikkatli bir şekilde kullanılmalıdır.
# Lists

## List Nedir?

Python'da, "list" veri tipi, birden çok değeri saklamak ve bu değerlere erişim sağlamak için kullanılan bir veri yapısıdır. Listeler, farklı veri tiplerini (örneğin, sayılar, metinler, diğer listeler vb.) içerebilir ve bu değerlere indeksler aracılığıyla erişilebilirler.

Bir liste oluşturmak için köşeli parantezleri `[]` kullanabilirsiniz. Örneğin:

```python
my_list = [1, 2, 3, 4, 5]
```

Bu örnek, 1'den 5'e kadar olan sayıları içeren bir liste oluşturur.

Listeler değiştirilebilir (mutable) olduğundan, içerikleri programın ilerleyen aşamalarında değiştirilebilir.&#x20;

### Nasıl oluşturabiliriz?

\
Python'da bir liste oluşturmak için köşeli parantezleri `[]` kullanmanız gerekmektedir. İşte farklı şekillerde listeler oluşturmanızı gösteren örnekler:

1. **Boş Bir Liste Oluşturmak:**

```python
empty_list = []
```

2. **Elemanlarla Dolu Bir Liste Oluşturmak:**

```python
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "orange"]
mixed_list = [1, "apple", True, 3.14]
```

3. **`list()` Fonksiyonunu Kullanarak Liste Oluşturmak:**

```python
numbers = list([1, 2, 3, 4, 5])
```

4. **`range()` Fonksiyonunu Kullanarak Liste Oluşturmak:**

```python
number_range = list(range(1, 6))  # 1'den 5'e kadar (5 dahil değil) sayıları içeren liste.
```

5. **Liste İfadesi ile Liste Oluşturmak (`list comprehension`):**

```python
squared_numbers = [x**2 for x in range(1, 6)]  # 1'den 5'e kadar sayıların karesini içeren liste.
```

6. **`*` Operatörünü Kullanarak Tekrarlanan Elemanlarla Liste Oluşturmak:**

```python
repeated_list = ["hello"] * 3  # "hello"yı üç kez içeren liste.
```

Bu örnekler, farklı yöntemlerle nasıl liste oluşturabileceğinizi göstermektedir. Listeler değiştirilebilir olduğundan (mutable), içeriklerini sonradan güncelleyebilirsiniz.

#### Nested List Nedir?

Nested list (iç içe geçmiş liste), bir listenin içinde başka listeleri bulunduran bir liste yapısıdır. Bu, verileri hiyerarşik olarak düzenlemek ve daha karmaşık veri yapıları oluşturmak için kullanılır. İşte birkaç örnek:

**Örnek 1: Matris Temsili**

```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

Bu örnek, 3x3 boyutlarında bir matrisi temsil eder. Her bir iç liste, matrisin bir satırını ifade eder.

**Örnek 2: Öğrenci Bilgileri**

```python
students = [
    ["Alice", 23, "Computer Science"],
    ["Bob", 21, "Mathematics"],
    ["Eve", 22, "Physics"]
]
```

Bu örnek, öğrenci bilgilerini iç içe geçmiş listelerle temsil eder. Her iç liste, bir öğrencinin adını, yaşını ve bölümünü içerir.

**Örnek 3: Film Listesi**

```python
movie_list = [
    ["The Matrix", 1999, ["Keanu Reeves", "Laurence Fishburne"]],
    ["Inception", 2010, ["Leonardo DiCaprio", "Joseph Gordon-Levitt"]],
    ["Jurassic Park", 1993, ["Sam Neill", "Laura Dern"]]
]
```

Bu örnek, film bilgilerini iç içe geçmiş listelerle temsil eder. Her iç liste, bir filmin adını, yayın yılını ve başrol oyuncularını içerir.

**Örnek 4: Tic Tac Toe Oyun Tahtası**

```python
tic_tac_toe = [
    ["X", "O", "X"],
    ["O", "X", "O"],
    ["X", "X", "O"]
]
```

Bu örnek, bir Tic Tac Toe oyun tahtasını iç içe geçmiş listelerle temsil eder. Her iç liste, bir sıranın durumunu ifade eder.

Nested list'ler, verilerin daha karmaşık şekillerde düzenlenmesi ve işlenmesi gereken durumlarda oldukça kullanışlı olabilir.

## List içerisindeki bir elemana nasıl ulaşabiliriz?

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

Python'da bir listedeki belirli bir elemana ulaşmak için indeksleri kullanabilirsiniz. Listelerde indeksler 0'dan başlar, yani listenin ilk elemanı indeks 0'e, ikinci elemanı indeks 1'e ve böyle devam eder. İşte birkaç örnek:

```python
my_list = [10, 20, 30, 40, 50]

first_element = my_list[0]  # Listenin ilk elemanını alır (10).
second_element = my_list[1]  # Listenin ikinci elemanını alır (20).
third_element = my_list[2]   # Listenin üçüncü elemanını alır (30).
```

Ayrıca, negatif indeksler kullanarak listenin sonundan başlayarak geriye doğru sayabilirsiniz:

```python
last_element = my_list[-1]  # Listenin son elemanını alır (50).
second_last_element = my_list[-2]  # Listenin sondan ikinci elemanını alır (40).
```

Eğer belirli bir aralıktaki elemanlara ulaşmak isterseniz, slicing (dilimleme) yöntemini kullanabilirsiniz:

```python
sub_list = my_list[1:4]  # 1. indeksten 3. indekse kadar olan elemanları içeren alt liste.
```

Bu şekilde, listenin belirli bir aralığındaki elemanlara ulaşabilirsiniz. Unutmayın ki indeksler sınırlar dahil değil, yani yukarıdaki örnekteki `sub_list` aslında 1. indeksten 3. indekse kadar (3. indeks dahil değil) elemanları içerir.

#### Nested List içindeki bir elemana nasıl ulaşırım?

Aşağıda iç içe geçmiş bir liste örneği ve bu iç içe geçmiş listedeki belirli bir elemana nasıl ulaşılacağına dair örnekler bulabilirsiniz:

```python
nested_list = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]

# İç içe geçmiş listeye erişim örnekleri
element_1_1 = nested_list[1][1]  # İkinci satırın ikinci elemanı (5)
element_0_2 = nested_list[0][2]  # İlk satırın üçüncü elemanı (3)
element_2_0 = nested_list[2][0]  # Üçüncü satırın ilk elemanı (7)

print(element_1_1)  # Çıktı: 5
print(element_0_2)  # Çıktı: 3
print(element_2_0)  # Çıktı: 7
```

Yukarıdaki örnekte, `nested_list[1][1]` ifadesi iç içe geçmiş listenin ikinci satırına (indeks 1) ve ikinci elemanına (indeks 1) ulaşır, yani sonuç olarak `5` elde edilir.

### Listeye eleman eklemek / çıkarmak ve var olan elemanı değiştirmek:

Bir Python listesine eleman eklemek ve çıkarmak için çeşitli yöntemler ve metodlar kullanabilirsiniz. İşte temel olarak kullanabileceğiniz bazı yöntemler:

**Eleman Ekleme:**

1. **`append()` Metodu:** Listenin sonuna yeni bir eleman eklemek için `append()` metodunu kullanabilirsiniz.

   ```python
   my_list = [1, 2, 3]
   my_list.append(4)  # Listenin sonuna 4 ekler.
   ```
2. **`insert()` Metodu:** Belirli bir indekse yeni bir eleman eklemek için `insert()` metodunu kullanabilirsiniz.

   ```python
   my_list = [1, 2, 3]
   my_list.insert(1, 5)  # İkinci indekse 5 ekler.
   ```
3. **`extend()` Metodu:** Bir listeyi diğer bir listeyle birleştirmek ve elemanları eklemek için `extend()` metodunu kullanabilirsiniz.

   ```python
   my_list = [1, 2, 3]
   new_elements = [4, 5, 6]
   my_list.extend(new_elements)  # Listenin sonuna [4, 5, 6] ekler.
   ```

**Eleman Çıkarma:**

1. **`pop()` Metodu:** Belirli bir indeksteki elemanı çıkarmak için `pop()` metodunu kullanabilirsiniz. Eğer indeks belirtilmezse, son eleman çıkarılır.

   ```python
   my_list = [1, 2, 3, 4, 5]
   popped_element = my_list.pop(2)  # Üçüncü elemanı (3) çıkarır ve çıkarılan elemanı döndürür.
   ```
2. **`remove()` Metodu:** Belirli bir değere sahip olan ilk elemanı çıkarmak için `remove()` metodunu kullanabilirsiniz.

   ```python
   my_list = [1, 2, 3, 2, 4]
   my_list.remove(2)  # İlk değeri 2 olan elemanı çıkarır.
   ```
3. **Elemanın Değeri ile Çıkarma:** Eğer çıkarılacak elemanın değerini biliyorsanız, indeks kullanmadan doğrudan `remove()` ile çıkarabilirsiniz.

   ```python
   my_list = [1, 2, 3, 4, 5]
   my_list.remove(3)  # Değeri 3 olan elemanı çıkarır.
   ```
4. **`del` Anahtarı ile Çıkarma:** `del` anahtar kelimesini kullanarak belirli bir indeksteki elemanı çıkarabilirsiniz.

   ```python
   codemy_list = [1, 2, 3, 4, 5]
   del my_list[1]  # İkinci elemanı (indeks 1) çıkarır.
   ```
5. **`del` Anahtarı ile Listeyi silme:** `del` anahtar kelimesini kullanarak belirli bir indeksteki elemanı çıkarabilirsiniz.

   ```python
   my_list = [1, 2, 3, 4, 5]
   del my_list  # Tüm listeyi siler.
   # print(my_list)  # Hata! my_list artık tanımlı değil.
   ```

**Lístedeki bir elemanı değiştirme:**

```python
my_list = [1, 2, 3, 4, 5]
my_list[0] = 10  # İlk elemanı 10 ile değiştirir.
# print(my_list)  # Sonuç :[10,2,3,4,5]
```

Unutmayın ki, listeden bir elemanı çıkardığınızda liste otomatik olarak yeniden düzenlenir ve indeksler güncellenir.

### List Methodları

Python'da listelerle çalışırken kullanabileceğiniz bazı yaygın liste metotlarını aşağıda örneklerle açıklıyabiliriz:

1. **append()**: Listenin sonuna eleman ekler.

```python
my_list = [1, 2, 3]
my_list.append(4)
# Sonuç: [1, 2, 3, 4]
```

2. **extend()**: Bir listenin sonuna başka bir listenin elemanlarını ekler.

```python
my_list = [1, 2, 3]
new_elements = [4, 5, 6]
my_list.extend(new_elements)
# Sonuç: [1, 2, 3, 4, 5, 6]
```

3. **insert()**: Belirli bir indekse eleman ekler.

```python
my_list = [1, 2, 3]
my_list.insert(1, 5)
# Sonuç: [1, 5, 2, 3]
```

4. **remove()**: Belirli bir değere sahip ilk elemanı çıkarır.

```python
my_list = [1, 2, 3, 2, 4]
my_list.remove(2)
# Sonuç: [1, 3, 2, 4]
```

5. **pop()**: Belirli bir indeksteki elemanı çıkarır ve çıkarılan elemanı döndürür.

```python
my_list = [1, 2, 3, 4, 5]
popped_element = my_list.pop(2)
# Sonuç: my_list = [1, 2, 4, 5], popped_element = 3
```

6. **clear()**:Bir listenin içindeki tüm elemanları kaldırarak listenin boş hale getirir.

```python
my_list = [1, 2, 3, 4, 5]
my_list.clear()  # Tüm elemanları temizler.
print(my_list)   # Çıktı: []
```

7\.  **index()**: Belirli bir değere sahip ilk elemanın indeksini döndürür.

```python
my_list = [10, 20, 30, 20, 40]
index = my_list.index(20)
# Sonuç: index = 1
```

8. **count()**: Belirli bir değerin listede kaç kez geçtiğini sayar.

```python
my_list = [10, 20, 30, 20, 40]
count = my_list.count(20)
# Sonuç: count = 2
```

9. **sort()**: Listeyi küçükten büyüğe sıralar (listede kalıcı değişiklik yapar).

```python
my_list = [4, 1, 3, 2]
my_list.sort()
# Sonuç: my_list = [1, 2, 3, 4]
```

10. **reverse()**: Listeyi tersine çevirir (listede kalıcı değişiklik yapar).

```python
my_list = [1, 2, 3, 4]
my_list.reverse()
# Sonuç: my_list = [4, 3, 2, 1]
```

11. **copy()**: Listenin bir kopyasını oluşturur.

<pre class="language-python"><code class="lang-python">my_list = [1, 2, 3]
<strong>new_list = my_list.copy()
</strong># Sonuç: new_list = [1, 2, 3]
</code></pre>

12. **len():** Listenin eleman sayısını verir.

```python
my_list = [1, 2, 3]
length = len(my_list)
# Sonuç: 3
```

13. **sorted():**&#x42;ir listenin öğelerini sıralar ve sıralanmış bir liste döndürür.

```python
my_list = [4, 2, 1, 3, 5]
sorted_list = sorted(my_list)
print(sorted_list)  # Çıktı: [1, 2, 3, 4, 5]
```

Bu sadece bazı temel liste metotlarıdır. Python dokümantasyonu veya diğer kaynaklar, daha fazla liste metodu ve detayı hakkında bilgi sağlayabilir.

### List Comprehensions

List comprehensions (liste anlama yapıları), Python'da listenin daha kısa ve okunabilir bir şekilde oluşturulmasını sağlayan bir yapıdır. List comprehension'lar, mevcut bir liste, dizi veya veri kümesi üzerinde döngü işlemleri yaparak yeni bir liste oluşturmanıza olanak tanır.

List comprehension'lar genel olarak şu şekilde yapılandırılır:

```python
new_list = [expression for item in iterable if condition]
```

* `expression`: Oluşturulacak yeni elemanın ifadesi.
* `item`: Iterable (örneğin liste, dizi veya range) içindeki her bir öğe.
* `iterable`: Üzerinde döngü yapılacak olan veri yapısı.
* `condition` (isteğe bağlı): Bir koşula bağlı olarak elemanları filtrelemek için kullanılır.

Örneklerle açıklamak gerekirse:

**Örnek 1: Kareler Listesi**

```python
numbers = [1, 2, 3, 4, 5]
squared_numbers = [x ** 2 for x in numbers]
# squared_numbers: [1, 4, 9, 16, 25]
```

**Örnek 2: Çift Sayıları Filtreleme**

```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [x for x in numbers if x % 2 == 0]
# even_numbers: [2, 4, 6, 8, 10]
```

**Örnek 3: Harf Dizisi Oluşturma**

```python
word = "Python"
letters = [char for char in word]
# letters: ['P', 'y', 't', 'h', 'o', 'n']
```

**Örnek 4: İç İçe List Comprehension**

```python
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flattened = [num for row in matrix for num in row]
# flattened: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

List comprehension'lar, kodunuzu daha kısa ve anlaşılır hale getirmenin yanı sıra, döngü işlemleri ve eleman seçimleri gibi işlemleri tek satırda yapmanıza olanak tanır.

#### Bir elemanın listede olup olmadığını sorgulama

Elemanların bir liste içerisinde yer alıp almadığını sorgulamamız mümkümdür.Örneğin:

```
my_list = ['p', 'r', 'o', 'b', 'l', 'e', 'm']

# Output: True
print('p' in my_list)

# Output: False
print('a' in my_list)

# Output: True
print('c' not in my_list)
```
# Print-Input Fonksiyonlari

## <mark style="color:blue;">**Print Fonksiyonu**</mark>

Python'daki `print()` fonksiyonu, metin veya değerleri konsol veya çıktı akışına yazdırmak için kullanılan bir fonksiyondur. Bu fonksiyon, programınızın çalışma durumunu izlemek, hata ayıklamak veya kullanıcıyla etkileşimde bulunmak gibi amaçlarla kullanılır. İşte `print()` fonksiyonunun temel kullanımı ve örnekleri:

Temel kullanım:

```python
print("Merhaba, dünya!")
```

Değişkenlerle kullanım:

```python
isim = "Ahmet"
yas = 25
print("Merhaba,", isim, ". Sen", yas, "yaşındasın.")
```

Farklı veri tiplerini yazdırma:

```python
sayi = 42
ondalik_sayi = 3.14
metin = "Python"
dogru_mu = True

print("Tamsayı:", sayi)
print("Ondalık Sayı:", ondalik_sayi)
print("Metin:", metin)
print("Mantıksal:", dogru_mu)
```

Çıktıları aynı satırda yazdırma:

```python
print("Merhaba,", end=" ")
print("Dünya!")
```

Birden fazla değeri bir arada yazdırma:

```python
isim = "Ahmet"
yas = 25
print("Merhaba,", isim, ". Sen", yas, "yaşındasın.", sep="-")
```

Bu örneklerde görüldüğü gibi, `print()` fonksiyonu metinleri ve değişkenleri virgülle ayırarak alır. Varsayılan olarak, her `print()` çağrısı yeni bir satırda yazdırılır. Ancak `end` parametresini kullanarak bu davranışı değiştirebilirsiniz. Ayrıca, `sep` parametresi ile değerler arasına hangi karakterin geleceğini de belirleyebilirsiniz.

`print()` fonksiyonu özellikle geliştirme aşamasında değerleri ve sonuçları görmek için kullanışlıdır. Hata ayıklama ve programın akışını anlamak için kullanılan temel bir araçdır.

**`print()` fonksiyonunun parametrelerini:**

1. `objects`: Yazdırılacak nesneleri ifade eder. Birden fazla nesne virgülle ayrılarak yazılabilir. Örnek:

```python
isim = "Ahmet"
yas = 25
print("Benim adım", isim, "ve", yas, "yaşındayım.")
# Çıktı: Benim adım Ahmet ve 25 yaşındayım.
```

2. `sep`: Nesneler arasında kullanılacak ayırıcı karakteri belirler. Örnek:

```python
isim = "Ahmet"
soyisim = "Yılmaz"
print(isim, soyisim, sep="-")
# Çıktı: Ahmet-Yılmaz
```

3. `end`: `print()` fonksiyonunun sonunda kullanılacak karakteri belirler. Örnek:

```python
print("Merhaba", end="!")  # Sonunda ünlem işareti yerine yeni satır karakteri kullanıldı
# Çıktı: Merhaba!
```

4\. kaçış dizisi (escape sequence), Python ve birçok programlama dilinde kullanılan özel bir karakter dizisidir. Bu dizgi, metin içinde yeni bir satır başlatmak veya satır sonu yapmak amacıyla kullanılır.  ifadesi, bir karakter olarak algılanmaz, ancak metinde bulunduğunda bir "yeni satır" veya "satır sonu" karakteri gibi davranır.

Örneğin:

```python
print("Merhaba,\ndünya!")
```

Bu kod, iki satırlık bir çıktı üretecektir:

```
Merhaba,
dünya!
```

&#x20;ifadesini kullanarak metni birden fazla satıra bölebilir veya daha düzenli çıktılar oluşturabilirsiniz.

Bu örneklerde `print()` fonksiyonunun farklı parametrelerini ve özelliklerini gösterdim. Bu parametreleri kullanarak çıktıları özelleştirebilir ve çeşitli senaryolara uyarlayabilirsiniz.

\-----------------------------------------------------------------------------------------------------

## <mark style="color:blue;">**İnput Alma**</mark>

Python'da kullanıcıdan girdi almak için `input()` fonksiyonunu kullanabilirsiniz. Bu fonksiyon, kullanıcıdan bir metin girmesini bekler ve girilen metni bir dize olarak döndürür. İşte `input()` fonksiyonunun kullanımı ve bir örnek:

Temel kullanım:

```python
kullanici_girdisi = input("Lütfen bir metin girin: ")
print("Girdiğiniz metin:", kullanici_girdisi)
```

Bu örnekte, kullanıcıya bir metin girmesi istenir ve girilen metin `kullanici_girdisi` değişkenine atanır. Ardından, girilen metin ekrana yazdırılır.

Girdiyi sayıya dönüştürme:

<pre class="language-python"><code class="lang-python">yas = input("Yaşınızı girin: ")
yas_int = int(yas)
<strong>print("İleride", yas_int + 10, "yaşında olacaksınız.")
</strong>
#ikinci yol
yas = int(input("Yaşınızı girin: "))
print("İleride", yas_int + 10, "yaşında olacaksınız.")
</code></pre>

Kullanıcının girdisini aldıktan sonra, metin olarak alınan değeri gerektiğinde sayıya dönüştürmek için `int()` fonksiyonunu kullanabilirsiniz. Bu örnekte kullanıcının yaşını girdikten sonra, 10 yıl sonra kaç yaşında olacağını hesaplayıp yazdırıyoruz.

Girdiyi ondalık sayıya dönüştürme:

```python
boy = input("Boyunuzu metre cinsinden girin: ")
boy_float = float(boy)
print("Boyunuzun 2 katı:", boy_float * 2)
```

Eğer kullanıcının ondalık sayı girmesini bekliyorsanız, girilen metni `float()` fonksiyonuyla ondalık sayıya çevirebilirsiniz.

Kullanıcı girdisini alırken, programınızın beklemesi için kullanılır. Kullanıcı girdiği metni yazdıktan sonra Enter tuşuna basana kadar program bekler. Girdi alındıktan sonra program devam eder.

Kullanıcı girdilerini alırken, girdinin doğru türde olduğundan ve hataları işlemeniz gerektiğinden emin olmalısınız. Kullanıcının beklentiniz dışında bir şey girmesi durumunda programınızın çökmesini veya hatalarla karşılaşmasını engellemek önemlidir.


\-----------------------------------------------------------------------------------------------------
# Python Koşullu İfadeler

## Giriş

Bu rehber, Python programlamaya yeni başlayanlar için temel koşullu ifadeleri anlatmayı amaçlamaktadır. Koşullu ifadeler, programınızın belirli koşullara bağlı olarak farklı yolları takip etmesine olanak tanır.

### Temel Koşullu İfadeler

#### If İfadesi


`if` ifadesi, belirli bir koşulun doğru olduğu durumlarda belirli kod bloklarının çalıştırılmasını sağlar.

```python
x = 10

if x > 5:
    print("x 5'ten büyük")
```

#### If-Else İfadesi

`if-else` ifadesi, bir koşulun doğru olduğu durumda belirli bir kod bloğunu çalıştırır; aksi takdirde başka bir kod bloğunu çalıştırır.

```python
x = 3

if x > 5:
    print("x 5'ten büyük")
else:
    print("x 5'ten küçük veya eşit")
```

#### If-Elif-Else İfadesi

`if-elif-else` ifadesi, bir dizi koşulun sırayla kontrol edildiği ve ilgili kod bloğunun çalıştırıldığı durumlar için kullanılır.

```python
x = 7

if x > 10:
    print("x 10'dan büyük")
elif x > 5:
    print("x 5'ten büyük, ancak 10'dan küçük veya eşit")
else:
    print("x 5'ten küçük veya eşit")
```

### Örnekler

#### Sıcaklık Durumu Kontrolü

```python
temperature = 25

if temperature > 30:
    print("Hava sıcak")
elif temperature > 20:
    print("Hava ılıman")
else:
    print("Hava serin")
```

#### Kullanıcı Yetkilendirme

```python
username = "admin"
password = "12345"

input_username = input("Kullanıcı adını girin: ")
input_password = input("Parolayı girin: ")

if input_username == username and input_password == password:
    print("Giriş başarılı")
else:
    print("Hatalı kullanıcı adı veya parola")
```

Bu örnekler, temel koşullu ifadelerin nasıl kullanılacağını göstermektedir. Daha karmaşık senaryolar için Python belgelerine başvurabilirsiniz.

Bu rehber, GitBook'unuzda temel koşullu ifadeleri anlatan bir bölümün başlangıcı olarak kullanılabilir. Kendi GitBook'unuzu oluşturarak, daha fazla örnek ve açıklama ekleyerek içeriği genişletebilirsiniz.

### iç içe Kosulli ifadeler

#### Örnek 1: Hava Durumu Kontrolü

```python
temperature = 28
humidity = 60

if temperature > 30:
    if humidity > 70:
        print("Hava sıcak ve nemli, serinlemek iyi olabilir.")
    else:
        print("Hava sıcak ama nem düşük, keyifli bir gün!")
else:
    print("Hava ılıman.")
```

Bu örnekte, dıştaki `if` koşulu sıcaklık kontrolünü yaparken, içteki `if` koşulu nem kontrolünü gerçekleştiriyor. Eğer sıcaklık 30 dereceden yüksekse ve nem de 70'ten yüksekse, serinlemek önerilir. Aksi takdirde, sıcaklığın yüksek olmasına rağmen nem düşükse keyifli bir gün geçirilebilir.

#### Örnek 2: Öğrenci Notu Hesaplama

```python
grade = 75

if grade >= 90:
    print("Notunuz A")
elif grade >= 80:
    if grade >= 85:
        print("Notunuz B+")
    else:
        print("Notunuz B")
elif grade >= 70:
    if grade >= 75:
        print("Notunuz C+")
    else:
        print("Notunuz C")
else:
    print("Notunuz F")
```

Bu örnekte, öğrenci notuna göre farklı not aralıklarına karşılık gelen harf notları hesaplanıyor. İç içe geçmiş `if` ve `elif` ifadeleri kullanılarak, belirli sınırlar içindeki not aralıkları belirleniyor.

#### Örnek 3: Kullanıcı Yetkilendirme ve Yetki Kontrolü

```python
username = "admin"
password = "12345"
role = "admin"

input_username = input("Kullanıcı adını girin: ")
input_password = input("Parolayı girin: ")

if input_username == username and input_password == password:
    print("Giriş başarılı.")
    if role == "admin":
        print("Yönetici paneline hoş geldiniz.")
    else:
        print("Standart kullanıcı paneline hoş geldiniz.")
else:
    print("Hatalı kullanıcı adı veya parola.")
```

Bu örnekte, kullanıcı adı ve parola doğruysa ve aynı zamanda kullanıcının rolü "admin" ise, kullanıcı yönetici paneline giriş yapmış olur. Aksi takdirde, standart kullanıcı paneline giriş yapılır.

Bu örnekler, iç içe geçmiş koşullu ifadelerin nasıl kullanılabileceğini basit ve anlaşılır bir şekilde göstermektedir. Daha karmaşık senaryolar için bu temel yapıları genişleterek kullanabilirsiniz.<br>

\-----------------------------------------------------------------------------------------------------
# Sets

### Set Nedir?

Python'da Set, benzersiz ve sırasız (unordered) elemanların koleksiyonunu tutan bir veri yapısıdır. Set'ler matematiksel kümelerin kavramlarına dayanır ve her elemanın yalnızca bir defa bulunabileceği bir yapıya sahiptir. Set'lerde indeksleme veya sıralama gibi kavramlar bulunmaz.

Set'lerin ana özellikleri:

1. **Benzersiz Elemanlar:** Set içinde aynı elemandan yalnızca bir kez bulunabilir. Eğer aynı elemandan birden fazla eklemeye çalışırsanız, sadece bir kopyası set içinde tutulur.
2. **Sırasız:** Set'ler, elemanların sırasız bir şekilde depolandığı veri yapılarıdır. Bu nedenle indeks kullanarak veya sıra numarasına göre erişim yapamazsınız.
3. **Değiştirilebilir:** Set'lerdeki elemanlar değiştirilebilir (mutable) veri tipleri olmalıdır. Yani, liste gibi değiştirilebilir tipleri içerebilirler, ancak set'ler kendileri değiştirilebilirler.
4. **Hızlı Üyelik Kontrolü:** Bir elemanın set içinde olup olmadığını kontrol etmek hızlıdır. Bu özellik, set'lerin büyük veri kümelerinde üyelik kontrolü için tercih edilmesini sağlar.

### Nasıl Set oluşturulur?

Python'da set oluşturmanın farklı yöntemleri bulunmaktadır. Set'ler, `{}` süslü parantezler veya `set()` fonksiyonu kullanılarak oluşturulabilir. İşte bu iki yöntemin kullanımı:

**1. Süslü Parantezler (`{}`) ile Set Oluşturma:**

```python
my_set = {1, 2, 3, 4}
```

Set oluştururken elemanları süslü parantezler içine yazarak virgülle ayırabilirsiniz. Ancak boş bir süslü parantez `{}` kullanırsanız, bu bir boş sözlük (dictionary) oluşturur. Boş bir set oluşturmak için `set()` fonksiyonunu kullanmanız daha güvenlidir.

**2. set() Fonksiyonu ile Set Oluşturma:**

```python
my_set = set([1, 2, 3, 4])
```

`set()` fonksiyonu, bir liste, tuple veya diğer iterable veri yapılarından set oluşturmanızı sağlar.

Ayrıca, string veya liste gibi iterable veri yapılarını doğrudan `set()` fonksiyonuna geçirebilirsiniz:

```python
my_string = "hello"
string_set = set(my_string)
# string_set: {'h', 'e', 'l', 'o'}

my_list = [1, 2, 3, 3, 4, 4, 5]
list_set = set(my_list)
# list_set: {1, 2, 3, 4, 5}
```

Unutmayın ki set'lerde elemanlar benzersiz olmalıdır, bu nedenle aynı elemanın yinelenmesi set içinde sadece bir kez yer alır.

### Bir Set içerisindeki elemana nasıl ulaşırız?

Set'lerde elemanlara indeks numarası veya sıralama ile erişmek mümkün değildir çünkü set'ler sırasız (unordered) veri yapılarıdır. Ancak, bir elemanın set içinde olup olmadığını kontrol etmek veya set içindeki elemanları döngü ile gezinmek mümkündür.

**Elemanın Set İçinde Olup Olmadığını Kontrol Etme:**

Bir elemanın set içinde olup olmadığını `in` operatörü ile kontrol edebilirsiniz:

```python
my_set = {1, 2, 3, 4, 5}
element_to_check = 3

if element_to_check in my_set:
    print(f"{element_to_check} set içinde bulunuyor.")
else:
    print(f"{element_to_check} set içinde bulunmuyor.")
```

**Set İçindeki Elemanları Döngü ile Gezinme:**

Set'lerde elemanlara indeks olmadan erişemeyeceğiniz için elemanları döngü ile gezerek işlem yapabilirsiniz:

```python
my_set = {1, 2, 3, 4, 5}

for element in my_set:
    print(element)
```

Bu örnek, `for` döngüsü kullanarak `my_set` içindeki her bir elemanı gezerek ekrana yazdırır. Set'lerde elemanlar sırasız olduğu için herhangi bir sıralama garantisi yoktur.

### Set Metodları

Python set'leri, içerdikleri elemanları değiştirebilen (mutable) veri yapısıdır. Set'lerde birçok farklı işlem ve metod bulunur. İşte bazı yaygın kullanılan set metodları:

1. **add():** Bir eleman eklemek için kullanılır.

   ```python
   my_set = {1, 2, 3}
   my_set.add(4)
   ```
2. **remove():** Belirtilen bir elemanı set içinden kaldırmak için kullanılır. Eğer eleman set içinde yoksa `KeyError` hatası verir.

   ```python
   my_set = {1, 2, 3, 4}
   my_set.remove(3)
   ```
3. **discard():** Belirtilen bir elemanı set içinden kaldırmak için kullanılır. Eğer eleman set içinde yoksa hata vermez.

   ```python
   my_set = {1, 2, 3, 4}
   my_set.discard(3)
   ```
4. **pop():** Set içinden rastgele bir elemanı çıkarır ve bu elemanı döndürür. Set boşsa `KeyError` hatası verir.

   ```python
   my_set = {1, 2, 3, 4}
   popped_element = my_set.pop()
   ```
5. **clear():** Set'in içindeki tüm elemanları kaldırır ve boş bir set oluşturur.

   <pre class="language-python"><code class="lang-python"><strong>my_set = {1, 2, 3}
   </strong>my_set.clear()
   </code></pre>

<figure><img src="broken-reference" alt=""><figcaption></figcaption></figure>

6. **union():** İki veya daha fazla set'in birleşimini döndürür.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
union_set = set1.union(set2)
```

7. **intersection():** İki veya daha fazla set'in kesişimini döndürür.

```python
set1 = {1, 2, 3}
set2 = {3, 4, 5}
intersection_set = set1.intersection(set2)
```

8. **difference():** Bir set ile diğer setler arasındaki farkı döndürür.

```python
set1 = {1, 2, 3, 4, 5}
set2 = {3, 4, 5}
difference_set = set1.difference(set2)
```

9. **symmetric\_difference():** İki set arasındaki simetrik farkı (her iki sette de bulunmayan elemanlar) döndürür.

```python
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5}
symmetric_difference_set = set1.symmetric_difference(set2)
```

10. **copy():** Bir set'in kopyasını oluşturur.

    ```python
    original_set = {1, 2, 3}
    copy_set = original_set.copy()
    ```
11. **update():** Bir seti başka bir setle günceller veya diğer iterable veri yapılarından gelen elemanlarla günceller.

    ```python
    set1 = {1, 2, 3}
    set2 = {3, 4, 5}
    set1.update(set2)  # set1'i set2 ile günceller
    ```
12. **intersection\_update():** Bir seti, diğer set ile olan kesişimine günceller.

    ```python
    set1 = {1, 2, 3}
    set2 = {3, 4, 5}
    set1.intersection_update(set2)  # set1'i set2 ile kesişime günceller
    ```
13. **difference\_update():** Bir seti, diğer set ile olan farkına günceller.

    ```python
    set1 = {1, 2, 3, 4}
    set2 = {3, 4, 5}
    set1.difference_update(set2)  # set1'i set2 ile farkına günceller
    ```
14. **symmetric\_difference\_update():** Bir seti, diğer set ile olan simetrik farkına günceller.

    ```python
    set1 = {1, 2, 3}
    set2 = {3, 4, 5}
    set1.symmetric_difference_update(set2)  # set1'i set2 ile simetrik farkına günceller
    ```
15. **issubset():** Bir setin başka bir setin alt kümesi olup olmadığını kontrol eder.

    ```python
    set1 = {1, 2}
    set2 = {1, 2, 3, 4}
    is_subset = set1.issubset(set2)  # True
    ```
16. **issuperset():** Bir setin başka bir setin üst kümesi olup olmadığını kontrol eder.

    ```python
    set1 = {1, 2, 3, 4}
    set2 = {1, 2}
    is_superset = set1.issuperset(set2)  # True
    ```
17. **isdisjoint():** İki setin kesişiminin boş olup olmadığını kontrol eder.

    ```python
    set1 = {1, 2, 3}
    set2 = {4, 5, 6}
    is_disjoint = set1.isdisjoint(set2)  # True
    ```

Bu metodlar set'lerin işlemlerini daha fazla kontrol etmenizi ve manipüle etmenizi sağlar. Daha fazla bilgi için Python belgelerini inceleyebilirsiniz.

### Bir elemanın bir Set içerisinde olup olmadığını nasıl sorgularım?

Bir elemanın bir set içinde olup olmadığını sorgulamak için Python'da `in` anahtar kelimesini veya `not in` kelimesini kullanabilirsiniz.  İşte bir elemanın set içinde olup olmadığını sorgulama örneği:

```python
my_set = set("apple")

# Output: True
print('a' in my_set)

# Output: False
print('p' not in my_set)
```

### Bir Set içerisindeki elemanları döngü kullanarak nasıl gezme(Iterating through a Set)

"Iterating Through a Set" ifadesi, bir set içindeki elemanları döngü (iterasyon) kullanarak gezme işlemine işaret eder. Python'da set'ler sırasız (unordered) veri yapıları olduğundan, elemanları indeksleme veya sıralama olmadan gezmek gerekir. Bu nedenle döngüler, set içindeki elemanlara erişmek için sıkça kullanılır.

Set içindeki elemanları döngü ile gezmek için genellikle `for` döngüsü kullanılır. İşte set içindeki elemanları döngü ile gezmek için kullanabileceğiniz örnekler:

```python
my_set = {10, 20, 30, 40, 50}

# For döngüsü kullanarak set içindeki elemanları gezmek
for element in my_set:
    print(element)
```

Bu örnek, `for` döngüsü kullanarak `my_set` adlı set içindeki her bir elemanı `element` adlı değişkende sırayla saklar ve bu elemanları ekrana yazdırır. Unutmayın ki set'ler sırasız olduğundan, elemanların hangi sırayla döngüde gezildiğine dair bir garantisi yoktur.

Set içindeki elemanları döngü ile gezip üzerinde işlem yapmak, set'in içeriğini incelemek veya işlem yapmak için sıkça kullanılan bir yöntemdir.

### Setlerde Built-in fonksiyonları

Python'da set veri yapısı üzerinde kullanabileceğiniz bazı dahili (built-in) fonksiyonlar aşağıda listelenmiştir:

1. **len():** Bir setin eleman sayısını döndürür.

   ```python
   my_set = {1, 2, 3, 4, 5}
   length = len(my_set)
   ```
2. **max():** Bir setin en büyük elemanını döndürür.

   ```python
   my_set = {10, 5, 25, 30}
   max_element = max(my_set)
   ```
3. **min():** Bir setin en küçük elemanını döndürür.

   ```python
   my_set = {10, 5, 25, 30}
   min_element = min(my_set)
   ```
4. **sum():** Bir setin elemanlarının toplamını hesaplar. Sadece sayısal elemanlar içeren setlerde kullanılabilir.

   ```python
   num_set = {1, 2, 3, 4, 5}
   total = sum(num_set)
   ```
5. **sorted():** Bir setin elemanlarını küçükten büyüğe sıralayarak bir liste olarak döndürür.

   ```python
   my_set = {10, 5, 25, 30}
   sorted_list = sorted(my_set)
   ```
6. **any():** Bir setin içindeki elemanlardan en az biri `True` veya `True` değerine çevrilebilecekse `True`, aksi halde `False` döndürür.

   ```python
   bool_set = {False, False, True}
   any_true = any(bool_set)  # True
   ```
7. **all():** Bir setin içindeki elemanların hepsi `True` ise veya `True` değerine çevrilebiliyorsa `True`, aksi halde `False` döndürür.

   ```python
   bool_set = {False, False, True}
   all_true = all(bool_set)  # False
   ```

Bu dahili fonksiyonlar, set veri yapısı üzerinde işlemler yaparken kullanabileceğiniz bazı kullanışlı araçlardır.
# String

String (metin), bilgisayar programlamada kullanılan bir veri tipidir ve karakterlerin dizisini ifade eder. Metinler, kelime, cümle veya herhangi bir karakter dizisini temsil etmek için kullanılır. Metinler, Python ve diğer birçok programlama dilinde önemli bir veri tipidir ve metin işleme, veri analizi, kullanıcı girdisi alma, metin tabanlı dosyaları okuma/yazma gibi birçok alanda kullanılır.

Metinler genellikle çift tırnak (`"..."`) veya tek tırnak (`'...'`) içine alınarak oluşturulur. Örnekler:

```python
isim = "Ahmet"
soyisim = 'Yılmaz'
cumle = "Merhaba, dünya!"
```

Metinlerle çeşitli işlemler yapabilirsiniz, örneğin:

* Metinleri birleştirebilirsiniz (concatenate):

  ```python
  tam_isim = isim + " " + soyisim   # "Ahmet Yılmaz"
  ```
* Metinleri çarparak yinelemeler oluşturabilirsiniz:

  ```python
  tekrarlanan_metin = isim * 3  # "AhmetAhmetAhmet"
  ```
* Metinlerin uzunluğunu ölçebilirsiniz:

  ```python
  uzunluk = len(cumle)  # cumle'nin karakter sayısı
  15
  asdasda
  ```
* Metinlerin içinde belirli karakter veya alt diziyi arayabilirsiniz:

  ```python
  if "dünya" in cumle:
      print("cumle içinde 'dünya' kelimesi var")
  ```
* Metinleri dilimleyebilirsiniz (slicing):

  ```python
  alt_metin = cumle[8:13]  # "dünya"
  ```

Bir metindeki karakterlere erişmek veya metin üzerinde işlem yapmak için indeksleri kullanabilirsiniz. İndeksler, metindeki karakterlerin sırasını belirtir ve sıfırdan başlayarak artar. Pozitif indeksler soldan sağa doğru artar (0'dan başlar), negatif indeksler sağdan sola doğru artar (***-1'den başlar***).

Örneğin, "Merhaba" kelimesini ele alalım:

```css
 M  e  r  h  a  b  a
 0  1  2  3  4  5  6
-7 -6 -5 -4 -3 -2 -1
```

Bu tabloda, her karakterin pozitif ve negatif indeksleri gösterilmiştir.

Metin içindeki belirli bir karaktere veya karakter dizisine erişmek için indeksi kullanabilirsiniz. Örnekler:

```python
metin = "Merhaba"

ilk_karakter = metin[0]  # "M"
ikinci_karakter = metin[1]  # "e"
son_karakter = metin[-1]  # "a"
```

Ayrıca, indeksleri dilimleme (slicing) işlemlerinde de kullanabilirsiniz:

```python
alt_metin = metin[2:5]  # "rha"
```

Bu örnek, `metin` değişkeninin 2. indeksinden başlayarak 5. indeksine kadar olan karakterleri içeren bir alt metni alır.

Python'da indekslerle metin üzerinde birçok işlem yapabilirsiniz. Bu, metinlerin parçalarını almak, alt metinleri manipüle etmek ve metin verileri üzerinde çeşitli işlemler gerçekleştirmek için oldukça kullanışlıdır.

```python

str = Hollanda
print('str = ', str)  # Hollanda

#ilk karakter
print('str[0] = ', str[0])  # H

#son karakter
print('str[-1] = ', str[-1])  # a

#2. ila 5. arasindaki karakterleri dilimleme
print('str[1:5] = ', str[1:5])  # olla


 #6. ila 2. arasindaki son karakteri dilimleme
print('str[5:-2] = ', str[5:-2])  # n 
```

**Not:**  String dilimleme (slicing) işlemi yaparken, dilimlemenin başlangıç ve bitiş indeksleri arasındaki karakterlerden oluşan bir alt metni elde etmek amacıyla kullanılır. ***Dilimleme işlemi sırasında başlangıç indeksi dahil edilirken, bitiş indeksi dahil edilmez.***

Örneğin, "Merhaba" kelimesini ele alalım:

```css
M  e  r  h  a  b  a
0  1  2  3  4  5  6
```

Eğer `metin` değişkeni "Merhaba" ise:

* `metin[1:4]` dilimlemesi, 1. indeksten (e) başlayıp 4. indekse kadar (h) olan karakterleri içerir (dahil değil). Sonuç "erb" olur.
* `metin[2:5]` dilimlemesi, 2. indeksten (r) başlayıp 5. indekse kadar (a) olan karakterleri içerir (dahil değil). Sonuç "rha" olur.

Bu davranışın nedeni, indekslerin genellikle 0'dan başlaması ve indeksler arasındaki karakterlerin sayılmasının, dilimleme sonucunun ne kadar karakter içereceğini belirtmek için kullanılmasıdır. Böylece, dilimlemenin başlangıç indeksi dahil edilirken, bitiş indeksi dahil edilmez.

Eğer sadece başlangıç veya bitiş indeksi belirtilmezse, Python otomatik olarak metnin başından veya sonuna kadar dilimleme yapar. Örneğin:

* `metin[:4]` ifadesi, başlangıç indeksi belirtilmediği için metnin başından 4. indekse kadar (dahil değil) olan karakterleri içerir. Sonuç "Merh" olur.
* `metin[3:]` ifadesi, bitiş indeksi belirtilmediği için 3. indeksten (h) başlayıp metnin sonuna kadar olan karakterleri içerir. Sonuç "haba" olur.
* `metin[:]` ifadesi, başlangıç ve bitiş indeksleri belirtilmediği için tüm metni içerir.

Dilimleme işlemi sırasında, başlangıç indeksi dahil edilirken, bitiş indeksi dahil edilmediği için dikkatli olmak önemlidir.

Bu sadece temel metin işleme örneklerindendir. Metinlerle daha karmaşık işlemler yapmak, dizeleri biçimlendirmek ve metin manipülasyonu yapmak için Python içinde birçok fonksiyon ve yöntem bulunmaktadır.

Python'da metin (string) manipülasyonu için bir dizi string metodu bulunmaktadır. Bu metodlar, metin verilerini işlemek, dönüştürmek ve düzenlemek için kullanılır. İşte yaygın olarak kullanılan bazı Python string metodları:

1. `len()`: Bir dizenin uzunluğunu döndürür.  ***Not: len metodu 1 den baslar indeksten farklidir***

   ```python
   metin = "Merhaba, dünya!"
   uzunluk = len(metin)  #15lower(): Diziyi küçük harfe çevirir.
   ```
2. lower(): Diziyi küçük harfe çevirir.
3. ```python
   metin = "Merhaba, DÜNYA!"
   kucuk_harfli = metin.lower()
   ```
4. `upper()`: Diziyi büyük harfe çevirir.

   ```python
   metin = "Merhaba, dünya!"
   buyuk_harfli = metin.upper()
   ```
5. `capitalize()`: Dizinin ilk harfini büyük yapar, diğerlerini küçük bırakır.

   ```python
   metin = "merhaba, dünya!"
   bas_harf_buyuk = metin.capitalize()
   ```
6. `title()`: Kelimelerin baş harflerini büyük yapar.

   ```python
   metin = "merhaba, dünya!"
   bas_harf_buyuk_kelime = metin.title()
   ```
7. `strip()`: Başındaki ve sonundaki boşlukları temizler.

   ```python
   metin = "   Merhaba, dünya!   "
   temiz_metin = metin.strip()
   ```
8. `split()`: Diziyi belirli bir ayırıcıya göre böler ve bir liste döndürür.

   ```python
   metin = "Merhaba,dünya,nasılsınız?"
   kelimeler = metin.split(",")
   ```
9. `replace()`: Belirli bir alt dizesini başka bir alt dizesiyle değiştirir.

   ```python
   metin = "Merhaba, dünya!"
   yeni_metin = metin.replace("Merhaba", "Selam")
   ```
10. `find()`: Belirli bir alt dizenin dizindeki konumunu döndürür.

    ```python
    metin = "Merhaba, dünya!"
    konum = metin.find("dünya")
    ```
11. `startswith()`: Dizenin belirli bir alt dize ile başlayıp başlamadığını kontrol eder.

    ```python
    metin = "Merhaba, dünya!"
    if metin.startswith("Merhaba"):
        print("Başlıyor!")
    ```
12. `endswith()`: Dizenin belirli bir alt dize ile bitip bitmediğini kontrol eder.

    ```python
    metin = "Merhaba, dünya!"
    if metin.endswith("dünya!"):
        print("Bitiyor!")
    ```

Bu sadece birkaç örnektir ve Python'da birçok farklı string metodu bulunmaktadır. String metotlarını kullanarak metin verilerini işlemek ve düzenlemek oldukça kolaydır. 

\-----------------------------------------------------------------------------------------------------
# Tuples

### Tuple Nedir?

Python'da tuple, değiştirilemez (immutable) bir veri yapısıdır. Yani bir kez oluşturulduktan sonra içeriği değiştirilemez. Tuple, parantez `()` içinde virgülle ayrılmış öğelerden oluşur. Örnek olarak:

```python
my_tuple = (1, 2, 3)
```

Ancak, parantez kullanılmadan da öğeleri virgülle ayırarak tuple oluşturabilirsiniz:

```python
another_tuple = 4, 5, 6
```

Tuple'lar listelerden farklıdır çünkü tuple'lar değiştirilemezdir ve bu nedenle içeriği oluşturulduktan sonra değiştirilemez. Tuple'lar genellikle fonksiyonlardan birden fazla değeri döndürmek veya değiştirilmesini istemediğiniz verileri depolamak için kullanılır.

Tuple'ların özellikleri:

* Değiştirilemez: Bir kez oluşturulduktan sonra, tuple içindeki elemanları değiştiremezsiniz. Bu, verilerin güvenliğini sağlamak için kullanışlı olabilir.
* Heterojen: Bir tuple içinde farklı veri tiplerine sahip öğeler bulunabilir (örneğin, sayılar, metinler, boolean değerler).
* Sıralı: Tuple'lar içindeki öğelerin sırası vardır ve indekslenerek erişilebilirler.
* Hashable: Tuple'lar, dictionary gibi hash tablosu tabanlı veri yapılarında anahtar olarak kullanılabilir.

Örnek:

```python
person = ("John", 30, "New York")
print(person[0])  # "John"
```

Tuple'lar genellikle değiştirilmesi istenmeyen sabit verileri veya birbirine ilişkili verileri gruplamak için kullanılır.

### Nasıl tuple oluşturulur?

Python'da tuple oluşturmak için parantez `()` kullanabilirsiniz. Tuple'ın içindeki öğeleri virgülle ayırarak tanımlarsınız. İşte tuple oluşturma yöntemleri:

1. **Parantez Kullanarak Tuple Oluşturma:**

```python
my_tuple = (1, 2, 3, 4, 5)
```

2. **Parantez Olmadan Tuple Oluşturma:**

```python
another_tuple = 4, 5, 6
```

3. **Bir Değişkeni Tuple'a Dönüştürme:**

```python
my_list = [10, 20, 30]
converted_tuple = tuple(my_list)
```

Tuple oluştururken virgül kullanmak çok önemlidir. Eğer sadece bir elemanlı bir tuple oluşturmak isterseniz, elemanın sonuna virgül koymalısınız. Aksi takdirde Python, bu elemanı bir nesne olarak kabul eder.

```python
single_element_tuple = (10,)  # Bir elemanlı tuple
single_element_tuple_without_comma = (10)  # Bu sadece bir sayıdır, tuple değil
```

Tuple'lar değiştirilemez (immutable) olduğu için oluşturduktan sonra içerisindeki öğeleri değiştiremezsiniz. Eğer içeriği değiştirilmesi gereken bir veri yapısı kullanmanız gerekiyorsa, liste kullanmanız daha uygundur.

### Python'da tuple kullanımına dair bazı örnekler:

**Örnek 1: Kişisel Bilgiler Tuple'ı**

```python
person = ("Alice", 28, "Engineer")
print(person[0])  # Çıktı: "Alice"
print(person[1])  # Çıktı: 28
```

**Örnek 2: Bir Fonksiyonun Birden Fazla Değer Dönmesi**

```python
def divide_and_remainder(a, b):
    quotient = a // b
    remainder = a % b
    return quotient, remainder

result = divide_and_remainder(10, 3)
print(result)  # Çıktı: (3, 1)
```

**Örnek 3: Çeşitli Veri Tiplerini İçeren Tuple**

```python
mixed_tuple = ("apple", 42, True, 3.14)
```

**Örnek 4: Nested Tuple(İç İçe Tuple'lar)**

```python
nested_tuple = ((1, 2, 3), ("a", "b", "c"), (True, False))
```

**Örnek 5: Tuple'ların Listelerle Birleştirilmesi**

```python
tuple1 = (1, 2, 3)
tuple2 = (4, 5, 6)
combined_tuple = tuple1 + tuple2  # (1, 2, 3, 4, 5, 6)
```

**Örnek 6: Tuple'ların Unpacking'i**

```python
coordinates = (10, 20)
x, y = coordinates
print(x)  # Çıktı: 10
print(y)  # Çıktı: 20
```

**Örnek 7: Tuple'ları Dictionary Anahtarları Olarak Kullanma**

```python
location = (40.7128, -74.0060)
locations = {
    "New York": location,
    "Los Angeles": (34.0522, -118.2437)
}
```

**Örnek 8: Tuple'lar ve Looping**

```python
fruits = ("apple", "banana", "orange")
for fruit in fruits:
    print(fruit)
# Çıktı:
# apple
# banana
# orange
```

Bu örnekler, tuple'ların nasıl kullanılabileceği konusunda size bir fikir verebilir. Tuple'lar, özellikle değiştirilmesi istenmeyen veya değişmez verileri saklamak veya bir fonksiyondan birden fazla değer döndürmek için kullanışlıdır.

### Tuple içerisindeki elemanlara nasıl ulaşabilirim?

Tuple'ın elemanlarına indeks kullanarak veya tuple unpacking yöntemiyle erişebilirsiniz.

**1. İndeks Kullanarak Elemanlara Ulaşma:** Tuple'ın elemanlarına indeks numarası ile erişebilirsiniz. İndeksler 0'dan başlar.

```python
my_tuple = (10, 20, 30, 40, 50)
first_element = my_tuple[0]  # İlk eleman (10)
third_element = my_tuple[2]  # Üçüncü eleman (30)
```

**2. Tuple Unpacking ile Elemanlara Ulaşma:** Tuple unpacking, tuple içindeki öğeleri ayrı değişkenlere atama yaparak erişmeyi sağlar.

```python
my_tuple = (10, 20, 30)
x, y, z = my_tuple
print(x)  # 10
print(y)  # 20
print(z)  # 30
```

**3. Negatif İndeksler ile Elemanlara Ulaşma:** Negatif indeksler kullanarak tuple'ın sonundan geriye doğru indeksleme yapabilirsiniz.

```python
my_tuple = (10, 20, 30, 40, 50)
last_element = my_tuple[-1]  # Son eleman (50)
second_last_element = my_tuple[-2]  # Sonuncu eleman (40)
```

**4. Dilimleme (Slicing) ile Belirli Bir Aralıktaki Elemanlara Ulaşma:** Dilimleme kullanarak belirli bir aralıktaki elemanlara ulaşabilirsiniz.

```python
my_tuple = (10, 20, 30, 40, 50)
sub_tuple = my_tuple[1:4]  # 1. indeksten 3. indekse kadar olan elemanlar
# sub_tuple: (20, 30, 40)
```

Tuple'ın elemanlarına bu yöntemlerle erişebilirsiniz. Tuple'lar değiştirilemez olduğu için bir kez oluşturulduktan sonra elemanlarını değiştiremezsiniz.

### Tuple ve Tuple içerisindeki elemanları değiştirebilir miyiz?

Tuple'lar Python'da değiştirilemez (immutable) veri yapılarıdır, bu nedenle bir kez oluşturulduktan sonra içeriğini değiştiremezsiniz. Eğer içeriğini değiştirilmesi gereken bir veri yapısı kullanmanız gerekiyorsa, liste kullanmanız daha uygun olacaktır.

Eğer tuple içeriğini değiştirme ihtiyacınız varsa, tuple'ın elemanlarını kullanarak yeni bir tuple oluşturmanız gerekecektir. Örneğin:

```python
my_tuple = (1, 2, 3)
new_tuple = my_tuple + (4,)  # 4 elemanını eklemek için yeni bir tuple oluşturulur
# new_tuple: (1, 2, 3, 4)
```

Ya da mevcut bir tuple'dan belirli bir dilimleme ile yeni bir tuple oluşturabilirsiniz:

```python
my_tuple = (1, 2, 3, 4, 5)
new_tuple = my_tuple[:3] + (10, 20) + my_tuple[4:]  # 3. elemana kadar, sonra 10 ve 20 eklenir, sonra geri kalan elemanlar eklenir
# new_tuple: (1, 2, 3, 10, 20, 4, 5)
```

Ancak unutmayın ki bu yöntemlerle esasında yeni bir tuple oluşturmuş olursunuz, mevcut tuple'ın içeriği değişmez.

Eğer bir tuple içindeki elemanlar mutable (değiştirilebilir) veri tiplerine sahipse, bu elemanları değiştirebilirsiniz. Ancak tuple'ın kendisi hala immutable (değiştirilemez) olacaktır.

Yani, tuple içindeki elemanlar örneğin liste gibi mutable bir veri tipiyse, bu elemanların içeriğini değiştirebilirsiniz. Ancak, tuple'ın elemanlarını tamamen değiştirme veya eleman eklemek gibi işlemler hala mümkün olmayacaktır.

Örnek:

```python
my_tuple = ([1, 2, 3], [4, 5, 6])
my_tuple[0][1] = 10  # İlk elemanın ikinci öğesini 10 olarak değiştirir
print(my_tuple)  # Çıktı: ([1, 10, 3], [4, 5, 6])
```

Yukarıdaki örnekte, `my_tuple`'ın içindeki elemanlar liste olduğu için, içindeki öğeleri değiştirebiliyoruz. Ancak, `my_tuple`'ı tamamen değiştiremezsiniz.

Tuple'lar Python'da değiştirilemez (immutable) veri yapılarıdır, bu nedenle bir kez oluşturulduktan sonra içeriğini değiştiremezsiniz. Eğer içeriğini değiştirilmesi gereken bir veri yapısı kullanmanız gerekiyorsa, liste kullanmanız daha uygun olacaktır.

Eğer tuple içeriğini değiştirme ihtiyacınız varsa, tuple'ın elemanlarını kullanarak yeni bir tuple oluşturmanız gerekecektir. Örneğin:

```python
my_tuple = (1, 2, 3)
new_tuple = my_tuple + (4,)  # 4 elemanını eklemek için yeni bir tuple oluşturulur
# new_tuple: (1, 2, 3, 4)
```

Ya da mevcut bir tuple'dan belirli bir dilimleme ile yeni bir tuple oluşturabilirsiniz:

```python
my_tuple = (1, 2, 3, 4, 5)
new_tuple = my_tuple[:3] + (10, 20) + my_tuple[4:]  # 3. elemana kadar, sonra 10 ve 20 eklenir, sonra geri kalan elemanlar eklenir
# new_tuple: (1, 2, 3, 10, 20, 4, 5)
```

Ancak unutmayın ki bu yöntemlerle esasında yeni bir tuple oluşturmuş olursunuz, mevcut tuple'ın içeriği değişmez.

Eğer bir tuple içindeki elemanlar mutable (değiştirilebilir) veri tiplerine sahipse, bu elemanları değiştirebilirsiniz. Ancak tuple'ın kendisi hala immutable (değiştirilemez) olacaktır.

Yani, tuple içindeki elemanlar örneğin liste gibi mutable bir veri tipiyse, bu elemanların içeriğini değiştirebilirsiniz. Ancak, tuple'ın elemanlarını tamamen değiştirme veya eleman eklemek gibi işlemler hala mümkün olmayacaktır.

Örnek:

```python
my_tuple = ([1, 2, 3], [4, 5, 6])
my_tuple[0][1] = 10  # İlk elemanın ikinci öğesini 10 olarak değiştirir
print(my_tuple)  # Çıktı: ([1, 10, 3], [4, 5, 6])
```

Yukarıdaki örnekte, `my_tuple`'ın içindeki elemanlar liste olduğu için, içindeki öğeleri değiştirebiliyoruz. Ancak, `my_tuple`'ı tamamen değiştiremezsiniz.

### Tuple Methodları

Tuple'lar değiştirilemez (immutable) veri yapıları olduğu için, listelerde olduğu gibi çok fazla yönteme sahip değillerdir. Ancak yine de bazı temel metodlar ve işlemler tuple'larla kullanılabilir:

1. **count():** Belirli bir değerin tuple içinde kaç kez geçtiğini sayar.

   ```python
   my_tuple = (1, 2, 2, 3, 2, 4)
   count_2 = my_tuple.count(2)
   # count_2: 3
   ```
2. **index():** Belirli bir değerin hangi indekste olduğunu döndürür (ilk bulunanı döndürür).

   ```python
   my_tuple = (10, 20, 30, 20, 40)
   index_20 = my_tuple.index(20)
   # index_20: 1
   ```
3. **len():** Tuple'ın eleman sayısını döndürür.

   ```python
   my_tuple = (1, 2, 3, 4, 5)
   length = len(my_tuple)
   # length: 5
   ```
4. **+ Operatörü:** Tuple'ları birleştirir.

   ```python
   tuple1 = (1, 2, 3)
   tuple2 = (4, 5, 6)
   combined_tuple = tuple1 + tuple2
   # combined_tuple: (1, 2, 3, 4, 5, 6)
   ```
5. **\* Operatörü:** Tuple'ı çoğaltır.

   ```python
   my_tuple = (1, 2, 3)
   multiplied_tuple = my_tuple * 3
   # multiplied_tuple: (1, 2, 3, 1, 2, 3, 1, 2, 3)
   ```
6. **in Operatörü:** Bir değerin tuple içinde olup olmadığını kontrol eder.

   ```python
   my_tuple = (10, 20, 30)
   contains_20 = 20 in my_tuple
   # contains_20: True
   ```
7. **not in Operatörü:** Bir değerin tuple içinde olmadığını kontrol eder.

   ```python
   my_tuple = (10, 20, 30)
   contains_40 = 40 not in my_tuple
   # contains_40: True
   ```

Bu metodlar, tuple'lar üzerinde kullanabileceğiniz temel işlemlerdir. Tuple'ların sınırlı işlem yapma yeteneği, onları değiştirilemez ve güvenilir veri saklama yapısı olarak kullanışlı kılar.

### Bir Tuple nasıl silinir?

\
Python'da `del` anahtarı ile bir tuple'ı silmek mümkündür. Ancak unutmayın ki `del` anahtarı, nesnenin referansını siler ve bellekten kaldırır, ancak verinin kendisini silmez. Bu nedenle, tuple içindeki veriler hâlâ bellekte var olmaya devam edebilir, ancak tuple'a erişim kaybolur.

İşte `del` anahtarıyla bir tuple'ı silme örneği:

```python
my_tuple = ('p', 'r', 'o', 'g', 'r', 'a', 'm', 'i', 'z')

# can't delete items
# TypeError: 'tuple' object doesn't support item deletion
# del my_tuple[3]

# Can delete an entire tuple
del my_tuple

# NameError: name 'my_tuple' is not defined
print(my_tuple)

```

### Tuple içerisinde bir elemanın olup olmadığını nasıl sorgularız?

Bir tuple içinde belirli bir elemanın olup olmadığını sorgulamak için `in` operatörünü kullanabilirsiniz. `in` operatörü, belirli bir değerin bir veri yapısında bulunup bulunmadığını kontrol etmek için kullanılır. İşte bir tuple içinde eleman sorgulama örneği:

```python
# Membership test in tuple
my_tuple = ('a', 'p', 'p', 'l', 'e',)

# In operation
print('a' in my_tuple)
print('b' in my_tuple)

# Not in operation
print('g' not in my_tuple)
```

### Tuple ile nasıl bir döngü(iterating) oluşturabiliriz?

Tuple'ları üzerinde döngü (iterasyon) oluşturmak için `for` döngüsünü kullanabilirsiniz. `for` döngüsü, tuple'ın her bir elemanını tek tek gezmek ve işlem yapmak için kullanılır. İşte tuple'ı iterasyonla gezme örneği:

```python
my_tuple = (10, 20, 30, 40, 50)

for element in my_tuple:
    print(element)
```

Bu örnekte, `for` döngüsü kullanılarak `my_tuple`'ın her bir elemanı `element` adlı değişkende sırayla saklanır ve bu elemanlar ekrana yazdırılır. Sonuç olarak, tuple içindeki her bir elemanı tek tek gezebilirsiniz.

Tuple'lar genellikle sabit verileri veya farklı tipteki değerleri gruplamak için kullanıldığından, döngü kullanarak bu elemanlara erişmek oldukça yaygın bir kullanım senaryosudur.

###
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
# İşleçler (Operatorler)

Python'da işleçler (operators), farklı türde verileri manipüle etmek, hesaplamalar yapmak veya değerleri karşılaştırmak için kullanılan semboller veya özel sözcüklerdir. İşleçler, programlamanın temel taşlarından biridir ve Python'da da geniş bir yelpazede bulunurlar. İşte Python'da yaygın olarak kullanılan bazı temel işleç türleri:

### 1. Aritmetik İşleçler

Aritmetik işleçler matematiksel hesaplamalar yapmak için kullanılır:

* `+`: Toplama
* `-`: Çıkarma
* `*`: Çarpma
* `/`: Bölme
* `%`: Mod (kalanı bulma)
* `**`: Üs alma

Örnek:

```python
x = 10
y = 3

toplam = x + y
fark = x - y
carpim = x * y
bolum = x / y
kalan = x % y
kuvvet = x ** y
```

```python
x = 15
y = 4

# Output: x + y = 19
print('x + y =',x+y)

# Output: x - y = 11
print('x - y =',x-y)

# Output: x * y = 60
print('x * y =',x*y)

# Output: x / y = 3.75
print('x / y =',x/y)

# Output: x // y = 3
print('x // y =',x//y)

# Output: x ** y = 50625
print('x ** y =',x**y)
```

### 2. Karşılaştırma İşleçler

Karşılaştırma işleçleri, değerleri karşılaştırmak ve koşullar oluşturmak için kullanılır:

* `==`: Eşit mi?
* `!=`: Eşit değil mi?
* `<`: Küçük mü?
* `>`: Büyük mü?
* `<=`: Küçük veya eşit mi?
* `>=`: Büyük veya eşit mi?

Örnek:

```python
x = 5
y = 7

esit_mi = x == y
kucuk_mu = x < y
buyuk_mu = x > y
```

```python
x = 10
y = 12

# Output: x > y is False
print('x > y is',x>y)

# Output: x < y is True
print('x < y is',x<y)

# Output: x == y is False
print('x == y is',x==y)

# Output: x != y is True
print('x != y is',x!=y)

# Output: x >= y is False
print('x >= y is',x>=y)

# Output: x <= y is True
print('x <= y is',x<=y)
```

### 3. Mantıksal İşleçler

Mantıksal işleçler, mantıksal değerleri (True veya False) manipüle etmek için kullanılır:

* `and`: Mantıksal VE
* `or`: Mantıksal VEYA
* `not`: Mantıksal DEĞİL

Örnek:

```python
a = True
b = False

sonuc1 = a and b
sonuc2 = a or b
sonuc3 = not a
```

```python
x = True
y = False

print('x and y is',x and y)

print('x or y is',x or y)

print('not x is',not x)
```

```python
x and y is False
x or y is True
not x is False
```

`and` ve `or`, Python'da mantıksal işlemleri gerçekleştiren mantıksal operatörlerdir. Bu operatörler, genellikle koşulların birleştirilmesi veya karşılaştırma ifadelerinin değerlendirilmesi gibi durumlarda kullanılır. İşte `and` ve `or` operatörlerinin farkları:

1. **and Operatörü:** Bu operatör, koşulların her ikisi de doğru (True) olduğunda sonucun doğru (True) olmasını sağlar. Yani, tüm koşulların doğru olması gerekmektedir.

   Örnek:

   ```python
   x = 5
   y = 10
   if x > 0 and y > 0:
       print("Her iki koşul da doğru.")
   ```
2. **or Operatörü:** Bu operatör, en az bir koşulun doğru (True) olduğunda sonucun doğru (True) olmasını sağlar. Yani, en az bir koşulun doğru olması yeterlidir.

   Örnek:

   ```python
   x = 5
   y = -2
   if x > 0 or y > 0:
       print("En az bir koşul doğru.")
   ```

Özetle, `and` operatörü tüm koşulların doğru olması durumunda sonuç doğru olurken, `or` operatörü en az bir koşulun doğru olması durumunda sonucun doğru olmasını sağlar. Bu operatörler, koşullu ifadeleri birleştirmek ve mantıksal kararlar vermek için oldukça kullanışlıdır.

### 4. Atama İşleçleri

Atama işleçleri, değerleri değişkenlere atamak için kullanılır:

* `=`: Değer atama
* `+=`: Toplama ile atama
* `-=`: Çıkarma ile atama
* \`\*=\`\`: Çarpma ile atama
* \`/=\`\`: Bölme ile atama
* `%=`: Mod ile atama
* \`\*\*=\`\`: Üs ile atama

Örnek:

```python
x = 10
y = 3

x += y  # x = x + y
x -= y  # x = x - y
x *= y  # x = x * y
x /= y  # x = x / y
x %= y  # x = x % y
x **= y  # x = x ** y
```

Bu örnekler temel Python işleçlerini göstermektedir. İşleçler, programlamanın temelini oluşturan güçlü bir araçtır ve daha karmaşık işleçler ve ifadelerle daha ileri düzeyde programlar oluşturabilirsiniz.

\-----------------------------------------------------------------------------------------------------
