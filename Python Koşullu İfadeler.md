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
