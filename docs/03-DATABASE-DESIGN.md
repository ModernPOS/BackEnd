# 🗄️ ModernPOS Veritabanı Tasarımı
# 🗄️ ModernPOS Ma'lumotlar Bazasi Dizayni

---

## 🌍 Dil / Til
- [🇹🇷 Türkçe](#turkish)
- [🇺🇿 O'zbekcha](#uzbek)

---

<a name="turkish"></a>
# 🇹🇷 TÜRKÇE

## 1️⃣ Veritabanı Genel Bakış

**Veritabanı:** SQL Server 2022  
**ORM:** Entity Framework Core 10  
**Migration:** Code-First Approach

---

## 2️⃣ Ana Tablolar / SQL Şeması

> Her tablo için sadece başlıca alanlar ve örnekler eklenmiştir.

### 👤 Users (Kullanıcılar)
- Id (Guid, PK)
- FirstName
- LastName
- Email (Unique)
- PasswordHash
- Role (int: 0=Admin, 1=Manager, 2=Cashier)
- IsActive (bool)
- CreatedAt / UpdatedAt

### 🏪 Branches (Şubeler)
- Id (Guid, PK)
- Name
- Code (Unique)
- Address
- City
- Country
- IsActive

### 📦 Products (Ürünler)
- Id (Guid, PK)
- Name
- CategoryId (FK)
- Price
- Cost
- Barcode (Unique)
- Unit, MinStock, ImageUrl

### 📂 Categories (Kategoriler)
- Id (Guid, PK)
- Name
- Description
- ParentCategoryId (FK, nullable)

### 📊 Inventory (Stok)
- Id (Guid, PK)
- ProductId (FK)
- BranchId (FK)
- Quantity
- ReservedQuantity
- AvailableQuantity (Computed)

### 💰 Sales (Satışlar)
- Id (Guid, PK)
- SaleNumber (Unique)
- BranchId (FK)
- CustomerId (FK, nullable)
- CashierId (FK)
- SubTotal, TaxAmount, DiscountAmount
- TotalAmount, Status, PaymentStatus
- CreatedAt

### 📝 SaleItems (Satış Kalemleri)
- Id (Guid, PK)
- SaleId (FK)
- ProductId (FK)
- ProductName
- Quantity, UnitPrice, TaxRate, Discount, TotalAmount

### 💳 Payments (Ödemeler)
- Id (Guid, PK)
- SaleId (FK)
- PaymentMethod (int: 0=Cash,1=Card,2=QR,...)
- Amount

### 👥 Customers (Müşteriler)
- Id (Guid, PK)
- FirstName, LastName
- Email, PhoneNumber
- Address, City
- LoyaltyPoints, TotalPurchases

### 💼 Cashiers (Kasalar)
- Id (Guid, PK)
- Name
- Code (Unique)
- BranchId (FK)

---

## 3️⃣ İlişki Şeması (ERD)

```
Branches ──▶ Cashiers
Branches ──▶ Inventory
Products ──▶ Inventory
Products ──▶ SaleItems
Categories ──▶ Products
Sales ──▶ SaleItems
Sales ──▶ Payments
Sales ──▶ Customers
Sales ──▶ Cashiers
```

---

## 4️⃣ Seed Data (Başlangıç Verisi)

Örnek olarak:
- Admin kullanıcı
- Ana şube
- Birkaç demo ürün/kategori

---

<a name="uzbek"></a>
# 🇺🇿 O'ZBEKCHA

## 1️⃣ Ma'lumotlar Bazasi Umumiy Ko'rinishi

**Ma'lumotlar Bazasi:** SQL Server 2022  
**ORM:** Entity Framework Core 10  
**Migration:** Code-First yondashuv

## 2️⃣ Database Schema (Jadval tuzilmasi)

Yuqoridagi Türkçe tablolarning O'zbekcha karşılığında bir fark yoktur.  
Tuzilma bir xil, faqat field/column isimlari o'zbekcha bo'lishi mumkin.

---

**⭐ Yulduzcha bering!**
