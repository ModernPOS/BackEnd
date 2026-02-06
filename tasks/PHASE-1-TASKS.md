# 🗒️ ModernPOS Faz 1 Görev Listesi
# 🗒️ ModernPOS 1-Faza Vazifa Ro’yxati

---

## 🌍 Dil / Til
- [🇹🇷 Türkçe](#turkish)
- [🇺🇿 O'zbekcha](#uzbek)

---

<a name="turkish"></a>
# 🇹🇷 TÜRKÇE

## 🔥 Faz 1 – Altyapı ve Temel İşlevler

### 1. Proje Kurulumu & Clean Architecture
- [ ] .NET 8 çözüm ve src klasörü oluştur
- [ ] Domain, Application, Infrastructure, API katmanları kur (boş)
- [ ] Docker Compose dosyası ile SQL Server, Redis, RabbitMQ kur

### 2. Authentication – Kullanıcı Yönetimi
- [ ] Entity: User, Role, PasswordHash
- [ ] JWT Token Authentication
- [ ] Register, Login, Refresh endpointleri
- [ ] E2E testler: register, login

### 3. Ürün & Kategori CRUD
- [ ] Entity: Product, Category
- [ ] API endpointleri: /products, /categories
- [ ] Validation (FluentValidation)
- [ ] Birim testler

### 4. Satış, Kasa, Stok
- [ ] Entity: Sale, SaleItem, Cashier, Inventory
- [ ] Satış işlemleri: /sales, /saleitems endpointleri
- [ ] Kasa işlemleri: /cashiers endpointi
- [ ] Stok işlemleri: /inventory endpointi

### 5. Temel Raporlama
- [ ] Günlük satış raporu /reports/daily-sales
- [ ] Ürün bazlı satış raporu /reports/product-sales
- [ ] Kasiyer satış raporu /reports/cashier-sales

### 6. Test & CI/CD
- [ ] Test altyapısı, test cases
- [ ] GitHub Actions ile .NET build & test workflow

---

## 🤝 Faz 1 Tamamlandığında:
- [ ] Temel authentication ve CRUD işlevleri çalışan API
- [ ] Docker ortamında test edilebilen
- [ ] Temel raporlama endpointleri mevcut
- [ ] Kodun %60+ test coverage

---

<a name="uzbek"></a>
# 🇺🇿 O'ZBEKCHA

## 🔥 1-Faza – Asosiy infratuzilma va funksiyalar

### 1. Loyihani yaratish & Clean Architecture
- [ ] .NET 8, src katlamlari (Domain, Application, Infrastructure, API)
- [ ] Docker Compose: SQL Server, Redis, RabbitMQ

### 2. Autentifikatsiya – Foydalanuvchi boshqaruvi
- [ ] User, Role, PasswordHash entity
- [ ] JWT Token Authentication
- [ ] Register, Login, Refresh endpointlar
- [ ] E2E testlar

### 3. Mahsulot va Kategoriya CRUD
- [ ] Product, Category entity
- [ ] API endpointlar
- [ ] Validation
- [ ] Unit testlar

### 4. Savdo, Kassa, Ombor
- [ ] Sale, SaleItem, Cashier, Inventory entity
- [ ] Savdo endpointlar
- [ ] Kassa endpointlar
- [ ] Ombor endpointlar

### 5. Asosiy hisobotlar
- [ ] Kunlik savdo hisobotlari
- [ ] Mahsulot savdo hisobotlari
- [ ] Kassa hisobotlari

### 6. Test & CI/CD
- [ ] Test infratuzilmasi
- [ ] GitHub Actions build & test workflow

---

**⭐ Agar loyihani yoqtirsangiz, yulduzcha bering!**
