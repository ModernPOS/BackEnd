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

## O'zbek Qollanma
### 1. Domain Qatlami
Entitilar, Value Objectlar va Biznes qoidalari. Tashqi kutubxonalarga bog'lanmagan.
### 2. Application Qatlami
Biznes jarayonlarini boshqarish. CQRS uchun MediatR ishlatiladi.
### 3. Infrastructure Qatlami
Ma'lumotlar bazasi, fayl tizimi va xavfsizlik (identity) tizimlari.
### 4. Qurilmalar Qatlami (Hardware)
Fiskal printerlar, skanerlar va terminallar uchun umumiy interfeys.
