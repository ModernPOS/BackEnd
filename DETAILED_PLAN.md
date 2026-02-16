# Detailed Development Plan: WPF + .NET 10 POS

## 🌍 Languages / Diller / Tillar
- [English](#english-step-by-step)
- [Türkçe](#türkçe-adım-adım)
- [O'zbek](#ozbek-qadam-ba-qadam)

---

## English Step-by-Step

### 1. Backend Foundation (.NET 10)
- **Step 1.1: Solution & Projects**: Create `POS.Domain`, `POS.Application`, `POS.Infrastructure`, and `POS.WebAPI`.
- **Step 1.2: Domain Models**: Define core entities (Product, Sale, User, Terminal).
- **Step 1.3: Application Logic**: Setup MediatR for Command/Query separation (CQRS).
- **Step 1.4: Persistence**: Setup EF Core with PostgreSQL and initialize migrations.
- **Step 1.5: Identity**: Implement JWT-based secure authentication.

### 2. Desktop Development (WPF + DevExpress)
- **Step 2.1: UI Scaffolding**: Setup WPF project using DevExpress templates (Modern UI/Office style).
- **Step 2.2: MVVM Setup**: Implementation of `BaseViewModel` and Service abstractions for API calls.
- **Step 2.3: Sales Screen**: Design a high-performance, touch-friendly POS grid and numeric pad.
- **Step 2.4: Hardware Service**: Port Atol/Mercury drivers into specialized hardware services.
- **Step 2.5: Sync Logic**: Offline-first capability and real-time API syncing.

---

## Türkçe Adım Adım

### 1. Backend Temeli (.NET 10)
- **Adım 1.1: Solution ve Projeler**: `POS.Domain`, `POS.Application`, `POS.Infrastructure` ve `POS.WebAPI` katmanlarının oluşturulması.
- **Adım 1.2: Domain Modelleri**: Temel varlıkların (Ürün, Satış, Kullanıcı, Terminal) tanımlanması.
- **Adım 1.3: Uygulama Mantığı**: CQRS için MediatR altyapısının kurulması.
- **Adım 1.4: Veritabanı**: EF Core ve PostgreSQL kurulumu, ilk migration'ların oluşturulması.
- **Adım 1.5: Güvenlik**: JWT tabanlı Identity sisteminin entegrasyonu.

### 2. Masaüstü Geliştirme (WPF + DevExpress)
- **Adım 2.1: Arayüz İskeleti**: DevExpress şablonları kullanılarak WPF projesinin başlatılması.
- **Adım 2.2: MVVM Kurulumu**: `BaseViewModel` ve API servis soyutlamalarının yapılması.
- **Adım 2.3: Satış Ekranı**: Performanslı, dokunmatik uyumlu POS ekranı ve sayısal tuş takımı tasarımı.
- **Adım 2.4: Donanım Servisleri**: Atol/Mercury sürücülerinin WPF hizmetlerine dönüştürülmesi.
- **Adım 2.5: Senkronizasyon**: Çevrimdışı çalışma (Offline-first) ve anlık veri senkronizasyonu.

---

## O'zbek Qadam-ba-qadam

### 1-bosqich: Backend Asosi (.NET 10)
- **1.1-qadam: Solution va Loyihalar**: `POS.Domain`, `POS.Application`, `POS.Infrastructure` va `POS.WebAPI` qatlamlarini yaratish.
- **1.2-qadam: Domain Modellar**: Asosiy obyektlarni (Mahsulot, Sotuv, Foydalanuvchi) aniqlash.
- **1.3-qadam: Biznes Mantiq**: CQRS va MediatR tizimini sozlash.
- **1.4-qadam: Ma'lumotlar Bazasi**: EF Core va PostgreSQL integratsiyasi.
- **1.5-qadam: Xavfsizlik**: JWT asosida avtorizatsiya tizimi.

### 2-bosqich: Desktop Dasturi (WPF + DevExpress)
- **2.1-qadam: UI Skeleti**: DevExpress shablonlari yordamida WPF loyihasini boshlash.
- **2.2-qadam: MVVM Sozlash**: `BaseViewModel` va API servislarini loyihalash.
- **2.3-qadam: Sotuv Ekranining Dizayni**: Sensorli ekranlarga moslashtirilgan POS interfeysi.
- **2.4-qadam: Qurilmalar Servisi**: Atol/Mercury drayverlarini xizmat ko'rinishiga o'tkazish.
- **2.5-qadam: Sinxronizatsiya**: Offline rejimda ishlash va real-vaqtdagi ma'lumotlar almashinuvi.
