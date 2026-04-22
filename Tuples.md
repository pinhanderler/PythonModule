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
