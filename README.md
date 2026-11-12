# FreshLine Dentist — Modern Ağız ve Diş Sağlığı Polikliniği

Modern, hızlı ve mobil uyumlu dental klinik tanıtım ve online randevu talep web uygulaması.

---

## 🌟 Proje Hakkında

**FreshLine Dentist**, diş poliklinikleri ve hekimler için tasarlanmış; hasta odaklı, modern, kurumsal standartlara ve sağlık mevzuatına tam uyumlu bir web sitesi çözümüdür. Harici ağır kütüphanelere (framework) bağımlı olmadan saf HTML5, modern CSS3 ve optimize JavaScript mimarisiyle sıfır gecikmeli yüksek performans sunar.

---

## ✨ Temel Özellikler

- **📱 %100 Mobil ve Masaüstü Uyumlu (Responsive):** Tüm ekran boyutlarına (telefon, tablet, masaüstü) duyarlı modern arayüz tasarımı.
- **⚡ Ultra Hızlı & Bağımsız:** Framework veya harici kütüphane gerektirmez (Vanilla JS + CSS).
- **⏱️ Canlı Çalışma Durumu Göstergesi:** Ziyaret saati ve gününe göre otomatik *"Şu an açığız"* veya bir sonraki açılış vaktini belirten *"Şu an kapalıyız"* rozeti.
- **🦷 İnteraktif Tedavi Kataloğu:** Listelenen diş tedavilerinden *"Randevu talebi"* butonuna tıklandığında randevu formuna otomatik tedavi seçimi ve yumuşak kaydırma.
- **💬 Akıllı WhatsApp Randevu Sistemi:**
  - Form üzerinden ad, telefon, tedavi türü, tercih edilen gün ve saat aralığı alınır.
  - Pazar günü gibi kapalı günlerin seçimi otomatik engellenir.
  - Bilgileri önceden biçimlendirilmiş profesyonel bir mesaj taslağı halinde kliniğin WhatsApp hattına iletir.
- **📞 Kapsamlı & Alternatif İletişim Kanalları:**
  - Sabit telefon santrali, alternatif mobil / WhatsApp destek hattı, resmi kurumsal e-posta adresi.
  - Kolay yol tarifi için interaktif OpenStreetMap harita entegrasyonu.
  - Hızlı mesajlaşma için sağ alt sabit WhatsApp iletişim butonu.
- **👨‍⚕️ Uzman Hekim Kadrosu & Klinik Galerisi:** Uzmanlık alanları, tedavi üniteleri ve sterilizasyon standartlarının tanıtımı.
- **❓ Akordeon Sıkça Sorulan Sorular (SSS):** Tedavi planlaması, ücretlendirme, çocuk diş hekimliği ve otopark bilgileri.
- **🔒 KVKK / Aydınlatma Metni:** Hasta veri güvenliği için açılır modal penceresi ve randevu onay kutusu.
- **🚀 Arama Motoru Optimizasyonu (SEO):** OpenGraph etiketleri, semantik HTML5 başlık hiyerarşisi ve Google zengin sonuçları için Schema.org `Dentist` JSON-LD yapılandırılmış verisi.

---

## 🏢 Kurumsal İletişim Bilgileri

| Alan | Bilgi |
| --- | --- |
| **Marka / Klinik Adı** | FreshLine Dentist (Ağız ve Diş Sağlığı Polikliniği) |
| **Adres** | Büyükdere Caddesi No: 168/4, Levent, Beşiktaş / İstanbul |
| **Santral / Ana Hat** | [0 (212) 284 10 20](tel:+902122841020) |
| **Alternatif & WhatsApp Destek** | [0 (533) 810 40 20](tel:+905338104020) |
| **E-posta** | [info@freshlinedentist.com](mailto:info@freshlinedentist.com) |
| **Konum & Ulaşım** | Levent metro istasyonuna 3 dakika yürüme mesafesi |
| **Çalışma Saatleri** | Hafta içi: 09:00 – 19:00<br>Cumartesi: 09:00 – 15:00<br>Pazar: Kapalı |

---

## 📁 Proje Dizin Yapısı

```text
FreshLine-Dentist/
├── index.html       # Web sitesinin semantik iskeleti, içerik bölümleri ve SEO/JSON-LD kodları
├── style.css        # Renk paleti, tipografi, modern CSS değişkenleri ve responsive kuralları
├── script.js        # WhatsApp yönlendirmesi, canlı çalışma saati kontrolü ve dinamik kartlar
├── README.md        # Proje dokümantasyonu ve kullanım kılavuzu
└── img/             # Klinik, tedavi odaları ve hekim fotoğrafları
    ├── hero.jpg            # Ana karşılama görseli
    ├── dr-1.jpg            # Protetik diş tedavisi uzmanı
    ├── dr-2.jpg            # Diş hekimi
    ├── dr-3.jpg            # Çocuk diş hekimliği uzmanı
    ├── resepsiyon.jpg      # Bekleme ve karşılama alanı
    ├── tedavi-odasi.jpg    # Tedavi ünitesi
    └── sterilizasyon.jpg   # Sterilizasyon ve hijyen odası
```

---

## ⚙️ Yapılandırma ve Özelleştirme

Web sitesinin temel ayarları `script.js` dosyasının ilk satırlarından kolayca yönetilebilir:

```javascript
// script.js

// 1. WhatsApp Randevu & Destek Numarası (başında + olmadan, ülke koduyla)
const WHATSAPP_NO = "905338104020";

// 2. Çalışma Saatleri (0: Pazar, 1: Pazartesi ... 6: Cumartesi)
// [açılış saati, kapanış saati] veya kapalı günler için null
const SAATLER = {
  0: null,
  1: [9, 19],
  2: [9, 19],
  3: [9, 19],
  4: [9, 19],
  5: [9, 19],
  6: [9, 15],
};

// 3. Tedavi Hizmetleri Listesi
const TEDAVILER = [
  { ad: "İmplant Tedavisi", acik: "Eksik dişlerin yerine..." },
  { ad: "Ortodonti & Şeffaf Plak", acik: "Çapraşık dişlerin düzenlenmesi..." },
  // İhtiyaca göre yeni tedaviler eklenebilir
];
```

---

## 🚀 Yerel Olarak Çalıştırma

Projeyi çalıştırmak için herhangi bir kurulum ya da derleme (build) adımına ihtiyaç yoktur:

### Seçenek 1: Doğrudan Tarayıcıda Açma
`index.html` dosyasını çift tıklayarak varsayılan internet tarayıcınızda açabilirsiniz.

### Seçenek 2: Yerel Statik Sunucu ile Çalıştırma
Tavsiye edilen yöntem bir yerel sunucu başlatmaktır:

```bash
# Python ile:
python -m http.server 8000

# veya Node.js npx ile:
npx serve .
```
Ardından tarayıcınızdan `http://localhost:8000` adresine gidebilirsiniz.

---

## 🌐 Yayına Alma (Deployment)

Proje statik dosyalardan (HTML/CSS/JS) oluştuğu için aşağıdaki servislerde sıfır maliyetle saniyeler içinde yayına alınabilir:
- **GitHub Pages**
- **Vercel**
- **Netlify**
- **Cloudflare Pages**
- CPanel veya herhangi bir Linux/Windows web sunucusu

---

## ⚖️ Yasal ve Mevzuat Uyumluluğu

- Sağlık Bakanlığı sağlık hizmetleri tanıtım ve bilgilendirme esaslarına uygun olarak yanıltıcı kampanya ifadeleri, fiyat listeleri veya hasta öncesi/sonrası manipülatif görselleri barındırmaz.
- Footer alanında mesul müdür bilgisi ve tıbbi tavsiye yerine geçmediğine dair aydınlatma yer alır.
- 6698 sayılı KVKK kapsamında randevu talebi oluşturan ziyaretçilerin rızası alınır.

---

© FreshLine Dentist. Tüm hakları saklıdır.
