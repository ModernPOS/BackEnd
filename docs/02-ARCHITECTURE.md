# 🏗️ ModernPOS Mimari Dokümantasyonu
# 🏗️ ModernPOS Arxitektura Hujjati

---

## 🌍 Dil / Til
- [🇹🇷 Türkçe](#turkish)
- [🇺🇿 O'zbekcha](#uzbek)

---

<a name="turkish"></a>
# 🇹🇷 TÜRKÇE

## 1️⃣ Mimari Genel Bakış

ModernPOS, **Clean Architecture** prensiplerine göre tasarlanmış, modern bir .NET 10 uygulamasıdır.

### 🎯 Mimari Hedefler
- ✅ Bağımsızlık: Framework, UI, Database’den bağımsız
- ✅ Test Edilebilirlik: Kolayca test edilebilir
- ✅ Sürdürülebilirlik: Kolay bakım ve geliştirme
- ✅ Ölçeklenebilirlik: Yatay ve dikey ölçeklendirme
- ✅ Modülerlik: Bağımsız modüller

---

## 2️⃣ Clean Architecture Katmanları

```
Presentation Layer (API)    | Controllers, Middlewares
           ↓
Application Layer           | Use Cases, CQRS, DTOs, Validators
           ↓
Domain Layer (Core)         | Entities, Value Objects, Interfaces
           ↑
Infrastructure Layer        | Data Access, External Services, Repositories
```

---

### 📦 Domain Layer (ModernPOS.Domain)
- **İş kuralları, entity, value object tanımları, domain event ve repository interface’leri**
- Hiçbir katmana bağımlı değil

---

### 📦 Application Layer (ModernPOS.Application)
- **Use case’ler, CQRS (commands & queries), business logic orchestration, mapping, validation**
- Domain layer’a bağımlı

---

### 📦 Infrastructure Layer (ModernPOS.Infrastructure)
- **Data access (EF Core), external services, file/email/sms system, caching**
- Domain ve application’a bağımlı

---

### 📦 Presentation Layer (ModernPOS.API)
- **REST API endpoints, authentication/authorization, middleware, Swagger**
- Application ve infrastructure’a bağımlı

---

## 3️⃣ CQRS Pattern
- Komutlar (commands) veri değiştirir, sorgular (queries) veri okur.
- Separation of concerns, ölçeklenebilirlik ve read/write optimizasyonu sağlar.

---

## 4️⃣ Repository & Dependency Injection
- Generic repository ile veri erişimi soyutlanır.
- Dependency Injection (.NET built-in) ile servisler yönetilir.

---

## 5️⃣ Global Exception Middleware
- Hatalar merkezi olarak yakalanır.

---

## 6️⃣ JWT Authentication
- Kullanıcı Rollerine göre yetki.

---

## 7️⃣ Redis Caching
- Performans arttırma için.

---

<a name="uzbek"></a>
# 🇺🇿 O'ZBEKCHA

## 1️⃣ Arxitektura Umumiy Ko’rinishi

ModernPOS, **Clean Architecture** prinsipiga muvofiq ishlab chiqilgan zamonaviy .NET 8 ilovasidir.

### 🎯 Arxitektura Maqsadlari
- ✅ Mustaqillik: Framework, UI, Database’dan mustaqil
- ✅ Test qilish mumkinligi: Osonlik bilan test qilinadi
- ✅ Davomiylik: Oson parvarish va rivojlantirish
- ✅ Kengaytirilish: Gorizontal, vertikal kengaytirish
- ✅ Modullik: Mustaqil modullar

---

## 2️⃣ Clean Architecture Qatlamlari

Yuqoridagi Türkçe kısmındaki ile ayni tuzilma.

---

**⭐ Agar loyihani yoqtirsangiz, yulduzcha bering!**
