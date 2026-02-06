# 🔌 ModernPOS API Dokümantasyonu
# 🔌 ModernPOS API Hujjati

---

## 🌍 Dil / Til
- [🇹🇷 Türkçe](#turkish)
- [🇺🇿 O'zbekcha](#uzbek)

---

<a name="turkish"></a>
# 🇹🇷 TÜRKÇE

## 1️⃣ Genel API Bilgileri

- **Base URL:** `http://localhost:5000/api/`
- **Format:** RESTful
- **Authentication:** JWT Bearer Token
- **Version:** v1

---

## 2️⃣ Authentication Endpoint’leri

| Method | Endpoint            | Açıklama                |
|--------|---------------------|-------------------------|
| POST   | /auth/register      | Kullanıcı kayıt         |
| POST   | /auth/login         | Kullanıcı girişi        |
| POST   | /auth/refresh       | Token yenileme          |

**Örnek login:**
```json
POST /auth/login

{
  "email": "admin@modernpos.com",
  "password": "Admin@123"
}
```

---

## 3️⃣ Kullanıcı Yönetimi

| Method | Endpoint            | Açıklama              |
|--------|---------------------|-----------------------|
| GET    | /users              | Kullanıcı listesi     |
| GET    | /users/{id}         | Kullanıcı bilgisi     |
| POST   | /users              | Kullanıcı oluştur     |
| PUT    | /users/{id}         | Kullanıcı güncelle    |
| DELETE | /users/{id}         | Kullanıcı sil         |

---

## 4️⃣ Ürün/Kategori

| Method | Endpoint            | Açıklama              |
|--------|---------------------|-----------------------|
| GET    | /products           | Ürün listesi          |
| GET    | /products/{id}      | Ürün bilgisi          |
| POST   | /products           | Ürün oluştur          |
| PUT    | /products/{id}      | Ürün güncelle         |
| DELETE | /products/{id}      | Ürün sil              |

| Method | Endpoint            | Açıklama              |
|--------|---------------------|-----------------------|
| GET    | /categories         | Kategori listesi      |
| GET    | /categories/{id}    | Kategori bilgisi      |
| POST   | /categories         | Kategori oluştur      |
| PUT    | /categories/{id}    | Kategori güncelle     |
| DELETE | /categories/{id}    | Kategori sil          |

---

## 5️⃣ Satış & Kasa

| Method | Endpoint            | Açıklama                        |
|--------|---------------------|---------------------------------|
| GET    | /sales              | Satış listesi                   |
| GET    | /sales/{id}         | Satış bilgisi                   |
| POST   | /sales              | Satış oluştur                   |
| GET    | /saleitems/{id}     | Satış kalem bilgisi             |
| GET    | /cashiers           | Kasa listesi                    |
| GET    | /cashiers/{id}      | Kasa bilgisi                    |

---

## 6️⃣ Raporlama

| Method | Endpoint                   | Açıklama                    |
|--------|----------------------------|-----------------------------|
| GET    | /reports/daily-sales       | Günlük satış raporu         |
| GET    | /reports/product-sales     | Ürün bazlı satış raporu     |
| GET    | /reports/cashier-sales     | Kasiyer satış raporu        |
| GET    | /reports/inventory         | Stok raporu                 |

---

## 7️⃣ Örnek Response

```json
GET /products

[
  {
    "id": "e1a56...",
    "name": "Kola 1L",
    "categoryId": "c59f...",
    "price": 22.50,
    "barcode": "869xxxxxx",
    "stock": 125
  },
  {
    "id": "bc9d6...",
    "name": "Sandviç",
    "categoryId": "c59f...",
    "price": 35.00,
    "barcode": "869yyyyyy",
    "stock": 12
  }
]
```

---

<a name="uzbek"></a>
# 🇺🇿 O'ZBEKCHA

## 1️⃣ API Umumiy Ko’rinishi

**Base URL:** `http://localhost:5000/api/`  
**Format:** RESTful  
**Authentication:** JWT Bearer Token  
**Version:** v1

**Endpointlar Türkçe kısmındaki bilan aynidir.**

---

**⭐ Agar loyihani yoqtirsangiz, yulduzcha bering!**
