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
