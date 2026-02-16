# POS Architecture Guide (Clean Architecture)

## 🌍 Languages / Diller / Tillar
- [English](#english-guide)
- [Türkçe](#türkçe-rehber)
- [O'zbek](#ozbek-qollanma)

---

## English Guide
### 1. Domain Layer
Contains Entities, Value Objects, and Domain Logic. No external dependencies.
### 2. Application Layer
Handles business orchestration. Uses MediatR for CQRS.
### 3. Infrastructure Layer
Implementation of database, file systems, and identity servers.
### 4. Hardware Layer
Abstraction for fiscal printers, scanners, and terminals.

---

## Technical Recommendations (Advice)
- **Backend**: **.NET 10 (C#)** is the best choice. It provides top-tier performance and excellent libraries for hardware integration (Serial/USB).
- **Desktop**: **WPF + DevExpress** is recommended over WinForms. WPF's MVVM pattern aligns perfectly with Clean Architecture, and it provides a far more "premium" and modern UI/UX with smooth animations and better scaling on high-resolution monitors.

---

## Türkçe Rehber
### 1. Domain Katmanı
Varlıklar (Entities), Değer Nesneleri ve İş Mantığını içerir. Dış bağımlılığı yoktur.
### 2. Application Katmanı
İş akışlarını yönetir. CQRS yapısı için MediatR kullanır.
### 3. Infrastructure Katmanı
Veritabanı, dosya sistemi ve kimlik doğrulama servislerinin implementasyonu.
### 4. Donanım Katmanı
Fiskal yazıcılar, barkod okuyucular ve terminaller için soyutlama katmanı.

---

## Teknik Öneriler (.NET 10 & Desktop)
- **Backend**: **.NET 10 (C#)** kesinlikle en mantıklı tercih. Donanım entegrasyonu (Serial/USB) için en güçlü kütüphanelere ve en yüksek performansa sahiptir.
- **Masaüstü (Desktop)**: **WPF + DevExpress**, WinForms'a göre çok daha mantıklıdır. WPF'in MVVM deseni "Clean Architecture" ile tam uyumludur. Ayrıca yüksek çözünürlüklü ekranlarda (4K) çok daha iyi ölçeklenir ve çok daha "premium" (wow factor) bir arayüz sunar.

---

## O'zbek Qollanma
### 1. Domain Qatlami
Entitilar, Value Objectlar va Biznes qoidalari. Tashqi kutubxonalarga bog'lanmagan.
### 2. Application Qatlami
Biznes jarayonlarini boshqarish. CQRS uchun MediatR ishlatiladi.
### 3. Infrastructure Qatlami
Ma'lumotlar bazasi, fayl tizimi va xavfsizlik (identity) tizimlari.
### 4. Qurilmalar Qatlami (Hardware)
Fiskal printerlar, skanerlar va terminallar uchun umumiy interfeys.

---

## Texnik Tavsiyalar (.NET 10 va Desktop)
- **Backend**: **.NET 10 (C#)** eng to'g'ri tanlov. Qurilmalar bilan ishlash (Serial/USB) va yuqori unumdorlik (performance) uchun juda mos.
- **Desktop**: **WPF + DevExpress** WinForms'ga qaraganda ancha afzal. WPF'dagi MVVM pattern "Clean Architecture" bilan mukammal integratsiya bo'ladi va dizayn jihatidan ancha premium ko'rinish beradi.
