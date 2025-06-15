# 🌟 Gönüllülük ve Yardımlaşma Platformu

**Gönüllü Yönetim Sistemi**, PHP, MySQL ve Bootstrap kullanılarak geliştirilmiş bir web uygulamasıdır. Amacı, gönüllüleri ve gönüllü ilanlarını kolayca **yönetmek**, **takip etmek** ve **organize etmek** için sade ve etkili bir çözüm sunmaktır.

---

## 🚀 Temel Özellikler

- 🔐 **Kullanıcı Girişi & Oturum Yönetimi**  
- 👤 **Profil Güncelleme:** Ad, yaş, şehir ve yetenek düzenleme  
- 📝 **Gönüllü İlanları:** Oluşturma, düzenleme ve listeleme  
- 🙋‍♂️ **Gönüllü Başvurusu:** Kullanıcıların ilanlara başvurabilmesi  
- 📋 **Başvuru Takibi:** İlan sahiplerinin başvuranları görmesi  
- 🌍 **Şehir & Kategori Bazlı Filtreleme**

---

## 📌 Sayfa Detayları

### 🔑 Kullanıcı Girişi  
Kayıtlı kullanıcılar, `login.php` sayfasından sisteme giriş yapabilir.  
![Giriş Sayfası](images/login.png)

### 👤 Profil Sayfası  
Kullanıcılar burada:  
- Bilgilerini (Ad, yaş, şehir, yetenekler) güncelleyebilir.  
- Başvurduğun ilanlar listelenir 
- Açtığı gönüllü ilanlarını ve bu ilanlara yapılan başvuruları görüntüleyebilir.    

![Açtığı İlanlar](images/ilan.png)  





![Başvurduğu İlanlar](images/application.png)

### 🙏 Gönüllü Ol Sayfası  
- Şehir ve kategori bazında filtreleme yaparak uygun ilanları bulabilirsiniz.  
- Tüm açık gönüllü ilanları listelenir.  
![Gönüllü Olma - Filtre](images/gonulluol1.png)






---

## 🛠 Kullanılan Teknolojiler

- PHP 7+  
- MySQL  
- HTML & CSS (Bootstrap)  
- JavaScript (İsteğe bağlı)  
- PDO (Güvenli veritabanı işlemleri)

---

## 📁 Proje Dizini
```
proje/
├── aboutyou.php         
├── config.php            
├── index.php             
├── login.php              
├── logout.php            
├── register.php          
├── search.php             
├── update_profile.php    
├── volunteer.php         
├── volunteer_submit.php   
├── welcome.php                    
---

## ⚙ Kurulum Adımları

1️⃣ Bu projeyi bilgisayarınıza klonlayın:

```bash
git clone https://github.com/kullanici/gonullu-yonetim.git
```

2️⃣ `config.php` dosyasında veritabanı bilgilerinizi düzenleyin:

```php
$dsn = 'mysql:host=localhost;dbname=veritabani_adi;charset=utf8';
$username = 'db_kullanici';
$password = 'db_sifre';

$pdo = new PDO($dsn, $username, $password);
$pdo->setAttribute(PDO::ATTR_DEFAULT_FETCH_MODE, PDO::FETCH_ASSOC);
```

3️⃣ Projeyi Apache ya da Nginx'in ilgili dizinine taşıyın.

4️⃣ Tarayıcınızı açın ve aşağıdaki URL'ye gidin:

```
http://localhost/proje
```

## 📝 Linkler
- Web Sitesi:[Tıklayınız](http://95.130.171.20/~st23360859020)
- Tanıtım Videosu Linki:[Tıklayınız]()


---


