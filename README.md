# 🏪 ModernPOS - Modern Satış Noktası Sistemi
# 🏪 ModernPOS - Zamonaviy Savdo Nuqtasi Tizimi

[![.NET](https://img.shields.io/badge/.NET-8.0-512BD4?logo=dotnet)](https://dotnet.microsoft.com/)
[![SQL Server](https://img.shields.io/badge/SQL%20Server-2022-CC2927?logo=microsoft-sql-server)](https://www.microsoft.com/sql-server)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## 🌍 Dil / Til | Language
- [🇹🇷 Türkçe](#turkish)
- [🇺🇿 O'zbekcha](#uzbek)

---

<a name="turkish"></a>
# 🇹🇷 TÜRKÇE

## 📋 Proje Hakkında

**ModernPOS**, modern teknolojilerle geliştirilmiş, kapsamlı bir **Satış Noktası (Point of Sale)** sistemidir. Perakende mağazalar, marketler, cafe ve restoranlar için tasarlanmıştır.

### 🎯 Hedefler

- ✅ **Cross-platform:** Web, Desktop, Mobile, Tablet desteği
- ✅ **Cloud-ready:** On-premise veya Cloud ortamda çalışabilir
- ✅ **Microservices:** Modüler ve ölçeklenebilir mimari
- ✅ **Real-time:** Anlık senkronizasyon ve bildirimler
- ✅ **Modern UI/UX:** Kullanıcı dostu arayüz
- ✅ **API-first:** Entegrasyon odaklı tasarım

### 🛠️ Teknoloji Stack

**Backend:**
- .NET 8 (C# 12)
- ASP.NET Core Web API
- Entity Framework Core 8
- SQL Server 2022
- Redis (Distributed Cache)
- RabbitMQ (Message Queue)
- SignalR (Real-time)
- Clean Architecture + DDD + CQRS

**Frontend:**
- Angular 19 (Web)
- WPF + DevExpress (Desktop)
- Flutter 3.x (Mobile)

**DevOps:**
- Docker & Docker Compose
- Kubernetes
- GitHub Actions (CI/CD)
- Azure / AWS

## 📁 Proje Yapısı

- **docs/** - Dokümantasyon
  - 01-PROJECT-PLAN.md - Master plan
  - 02-ARCHITECTURE.md - Mimari tasarım
  - 03-DATABASE-DESIGN.md - Veritabanı şeması
  - 04-API-DOCUMENTATION.md - API dökümanları

- **tasks/** - Görev yönetimi
  - PHASE-1-TASKS.md - Faz 1 görevleri
  - BACKLOG.md - Yapılacaklar

- **src/** (yakında) - Kaynak kod
  - ModernPOS.Domain/
  - ModernPOS.Application/
  - ModernPOS.Infrastructure/
  - ModernPOS.API/

- **docker-compose.yml** - Docker yapılandırması
- **.gitignore** - Git ignore
- **README.md** - Bu dosya
