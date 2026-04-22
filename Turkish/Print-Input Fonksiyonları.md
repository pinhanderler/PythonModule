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
