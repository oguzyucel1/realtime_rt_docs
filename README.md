# 📄 LiveDocs – Realtime Collaborative Editor

<p align="center">
  Google Docs alternatifi gerçek zamanlı belge düzenleme uygulaması – Next.js, Clerk, Liveblocks ve Tailwind ile inşa edildi.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-13+-black?style=for-the-badge&logo=next.js" />
  <img src="https://img.shields.io/badge/TailwindCSS-3.x-blue?style=for-the-badge&logo=tailwindcss" />
  <img src="https://img.shields.io/badge/Clerk-Auth-success?style=for-the-badge&logo=clerk" />
  <img src="https://img.shields.io/badge/Liveblocks-Realtime-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Sentry-Monitoring-critical?style=for-the-badge&logo=sentry" />
  <img src="https://img.shields.io/badge/TypeScript-Strict-blue?style=for-the-badge&logo=typescript" />
</p>

---

## 🚀 Proje Özeti

**LiveDocs**, Next.js 13 App Router mimarisiyle geliştirilmiş, Google Docs benzeri bir **gerçek zamanlı işbirliği uygulamasıdır**.  
Kullanıcılar belgeler oluşturabilir, düzenleyebilir, paylaşabilir ve aynı anda birden fazla kullanıcıyla canlı olarak çalışabilir.

---

## ✨ Özellikler

- 🧾 **Markdown destekli Lexical editör**
- 🧑‍🤝‍🧑 **Canlı işbirliği** (Live cursors, aktif kullanıcı avatarları)
- 💬 **Gerçek zamanlı yorumlar, emoji ve etiketleme**
- 🔔 **Anlık bildirimler**
- 📤 **Belgeleri oluşturma, silme, paylaşma**
- 🔐 **Clerk ile kullanıcı oturumu ve kimlik doğrulama**
- 📈 **Sentry ile uygulama hata takibi**
- 🎨 **Figma tabanlı pixel-perfect responsive UI**
- ⚡ **Dark mode destekli modern tasarım**

---

## 🧱 Teknolojiler

| Teknoloji     | Açıklama                                    |
|---------------|---------------------------------------------|
| **Next.js 13**| App Router + Server Components              |
| **Tailwind CSS**| Modern responsive UI framework           |
| **Clerk**     | OAuth + JWT + kullanıcı yönetimi           |
| **Liveblocks**| Realtime işbirliği / socket temelli         |
| **Sentry**    | Uygulama izleme, performans ve hata loglama |
| **Lexical**   | Meta tarafından geliştirilen rich text editor |
| **TypeScript**| Tip güvenliği ve modüler mimari             |

---

## 🔐 Kimlik Doğrulama

Clerk entegrasyonu ile:
- Google ile tek tıkla giriş
- Kullanıcı avatarı, e-posta, IP bilgileri
- Kullanıcı başına erişim yetkilendirme
- Özel giriş/çıkış sayfaları (`/sign-in`, `/sign-up`)

---

## 🧩 Gerçek Zamanlı Altyapı (Liveblocks)

- Belge başına benzersiz "room ID"
- Aktif kullanıcı avatarları canlı izlenebilir
- Canlı düzenleme (cursors, selection)
- Sunucu tarafında kullanıcıya özel yetkilendirme ve kimlik doğrulama (`/api/liveblocks/auth`)
- Belgeler için otomatik oluşturulan collaborative “room” yapısı

---

## 📁 Klasör Yapısı

```text
realtime-docs/
├── app/                 # Next.js route yapısı
│   └── documents/       # Belge görüntüleme, dinamik ID ile
│   └── (auth)/          # Clerk giriş/çıkış sayfaları
├── components/          # Reusable UI bileşenleri
├── lib/                 # Yardımcı fonksiyonlar, server actions
├── styles/              # Tailwind + global stiller
├── public/              # Statik ikonlar ve görseller
├── types/               # Tip tanımları
├── middleware.ts        # Clerk korumalı route middleware
└── liveblocks.config.ts # Liveblocks yapılandırma
```
---

## 📊 Monitoring

- ✅ **Sentry kurulumu** yapılmıştır  
- 📊 **Sunucu + istemci taraflı performans takibi** sağlanır  
- 🌍 **Üretim ortamı izlenebilir**

---

## 🔒 Yetkilendirme & Paylaşım

- 🔐 Her belge, **sahibine özel** olarak oluşturulur  
- 🔗 Belgeler **paylaşılabilir** veya **yetkiler kaldırılabilir**  
- 👥 **Görüntüleyici / Düzenleyici** rolleri atanabilir

---

## 🧑‍💻 Geliştirici

| Bilgi        | Detay                                                        |
|--------------|--------------------------------------------------------------|
| 👨‍💻 Geliştirici | [@oguzyucel1](https://github.com/oguzyucel1)               |
| 📧 İletişim   | GitHub üzerinden **issue** açabilir veya **PR** gönderebilirsin |

---

## 🪪 Lisans

MIT Lisansı – detaylar için [LICENSE](./LICENSE) dosyasını inceleyiniz.

---

<p align="center">
  <b>Gerçek zamanlı yazmak, geleceğin standardıdır. <br/> LiveDocs ile bunu başlat.</b>
</p>
