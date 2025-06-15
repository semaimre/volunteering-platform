# Gönüllülük ve Yradımlaşma Platformu

Gönüllü Yönetim Sistemi, **PHP, MySQL ve Bootstrap** tabanlı, gönüllüleri ve gönüllü ilanlarını kolayca **yönetmeyi**, **takip etmeyi** ve **organize etmeyi** hedefleyen basit ve etkili bir **web uygulamasıdır**.

---

## 🚀 Özellikler

- 🔐 **Kullanıcı Girişi ve Oturum Yönetimi**
- 👥 **Profil Güncelleme:** Ad, yaş, şehir ve yetenekleri düzenlenebilir.
- 📝 **Gönüllü İlanları oluşturabilir ve düzenleyebilir**
- 🙏 **Gönüllüler:** İlanlara gönüllü olarak **başvurabilir**
- 📁 **Başvurular:** İlan oluşturucusu, kaç kişinin **başvurduğunu** ve **detayları** görebilir
- 🌍 **Şehir ve Kategori:** İlanlar ve gönüllüler şehir ve ilgi alanlarına göre sınıflandırılabilir

---

## 🛠 Teknoloji Stack

- **PHP 7+**
- **MySQL**
- **HTML, CSS (Bootstrap)**
- **Javascript (opsiyonel fonksiyonalite)**
- **PDO** (Veritabanı ile güvenli bağlantı)

---

## 📁 Proje Dizini

```
.
├── aboutyou.php    // Ana profil ve gönüllü ekranı
├── config.php      // PDO ile MySQL bağlantısını oluşturur
├── login.php       // Giriş ekranı
├── logout.php      // Oturum kapatma
├── welcome.php     // Ana sayfa
├── events/        // Gönüllü ilanları ilə ilgili fonksiyonlar
├── css/
├── images/
├── README.md
```

---

## ⚙ Kurulum

1️⃣ Bu projeyi bilgisayarınıza klonlayın:

```bash
git clone https://github.com/kullanici/gonullu-yonetim.git
```

2️⃣ `config.php` içinde **MySQL** bilgilerinizi düzenleyin:

```php
$dsn = 'mysql:host=localhost;dbname=veritabani_adi;charset=utf8';
$username = 'db_kullanici';
$password = 'db_sifre';

$pdo = new PDO($dsn, $username, $password);
$pdo->setAttribute(PDO::ATTR_DEFAULT_FETCH_MODE, PDO::FETCH_ASSOC);
```

3️⃣ Apache ya da Nginx içinde oluşturduğunuz directory’ye taşıyın.

4️⃣ Tarayıcınızı açın:

```
http://localhost/gonullu-yonetim/
```

---

## 📝 Veritabanı

**volunteers** (kullanıcılar) 
- `id`
- `user_id`
- `fullname`
- `age`
- `city`
- `skills`

**events** (gönüllü ilanları) 
- `id`
- `user_id`
- `title`
- `category`
- `city`
- `created_at`

**applications** (başvurular) 
- `id`
- `event_id`
- `user_id`
- `applied_at`

---

## 👥 Katkıda Bulun

1️⃣ Forklayın
2️⃣ `feature/{yenilik}` dalında çalışmalarınızı yapın
3️⃣ Pull isteği oluşturun
4️⃣ Geri bildirime göre düzenleyin

---

## 📝 Lisans

MIT

---

🚀 İyi çalışmalar!  
Proje ile ilgili sorularınızı **Issue** oluşturarak belirtebilirsiniz.
