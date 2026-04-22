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
