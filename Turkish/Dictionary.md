# Dictionaries

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

