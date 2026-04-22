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
