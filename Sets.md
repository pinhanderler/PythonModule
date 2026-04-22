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
