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
