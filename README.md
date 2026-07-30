# Cem Vural Yılmaz

**Flutter / Mobile Developer** · İstanbul, Türkiye

App Store ve Google Play'de yayında olan uygulamaları tek başıma geliştirip yayına alıyorum.
Sunucu tarafında doğrulanan satın alma akışları, Firestore güvenlik kuralları ve
transaction tabanlı uygulama içi ekonomi üzerine çalışıyorum.

Yazılım Mühendisliği, Kırklareli Üniversitesi (2026).

---

## Yayındaki uygulamalar

### 🎮 [ikiliya](https://ikiliya.com) — çok oyunculu Türkçe kelime ve bulmaca platformu
İki kişilik gerçek zamanlı oyunlar: Kelimelik, XOX, Hafıza, Dörtlük. Sezonluk içerik,
ELO sıralaması ve uygulama içi ekonomi.

[App Store](https://apps.apple.com/tr/app/id6765803594) · [Google Play](https://play.google.com/store/apps/details?id=com.ikiliya.app) · [ikiliya.com](https://ikiliya.com)

- Sunucu tarafında doğrulanan uygulama içi satın alma: Apple App Store Server Notifications + Google RTDN, sandbox/prod ayrımı, idempotent grant kuyruğu
- Firestore güvenlik kuralları ve transaction tabanlı coin/ödül ekonomisi — istemciden self-grant saldırısına kapalı
- Firebase App Check (App Attest) ile callable fonksiyonların korunması
- 80+ Cloud Functions · 669 birim/widget testi · GitHub Actions + Codemagic ile TestFlight'a otomatik dağıtım

`Flutter` `Dart` `Firebase` `Firestore` `Cloud Functions` `Provider` `MVVM` `TypeScript`

---

### 🥬 [freshIt](https://freshit.app) — market fişinden gıda israfı takibi
Market fişini fotoğraflayıp ürünleri ve son kullanma tarihlerini takip eden uygulama.
Kırklareli Üniversitesi GADOM stajı kapsamında dört haftada geliştirildi.

[App Store](https://apps.apple.com/tr/app/id6788709155) · [freshit.app](https://freshit.app)

- Fiş görüntüsünden yapılandırılmış veri çıkarımı (LLM vision) ve maliyet odaklı model kademelendirmesi
- Riverpod + Freezed ile feature-first Clean Architecture
- Sunucu tarafı premium doğrulama · 171 test

`Flutter` `Firebase` `Riverpod` `Freezed` `Clean Architecture` `Claude Vision API`

---

### 🧩 [Bulmaca Köşesi](https://bulmacakosesi.com) — günlük Türkçe bulmaca
Günlük bulmaca uygulaması; abonelik öncelikli reklamsızlık modeli ve premium oyun arşivi.
*App Store incelemesinde.*

[bulmacakosesi.com](https://bulmacakosesi.com)

- RevenueCat ile abonelik altyapısı (aylık + yıllık, ücretsiz deneme), reklam/abonelik geçiş mantığı
- iOS ATT izin akışının doğru zamanlanması ile App Store 2.1 uyumu
- 844 birim/widget testi

`Flutter` `Dart` `Firebase` `Riverpod` `RevenueCat` `AdMob`

---

## Açık kaynak

### 📦 [turkish_word_keyboard](https://github.com/cemvuralyilmaz/turkish_word_keyboard)
Türkçe kelime oyunları için ekran klavyesi — ikiliya'nın Kelimelik oyunundan çıkarıldı.

Türkçe'de `'istanbul'.toUpperCase()` yanlış sonuç verir (`ISTANBUL`), `['dut','çilek','cam'].sort()`
yanlış sıralar. Paket bunları çözer; klavye dizilimi de iOS Türkçe (Q) klavyesiyle birebir aynıdır.

`Flutter` `Dart` · 38 test · MIT

### 📦 [utf16_safe_text](https://github.com/cemvuralyilmaz/utf16_safe_text)
UTF-16 güvenli string kırpma — ikiliya'dan çıkarıldı.

Emoji, Dart'ta iki kod biriminden oluşur. Ham `substring` bu çiftin ortasından bölerse geriye
eşsiz bir surrogate kalır ve Flutter'ın metin motoru `string is not well-formed UTF-16` ile çöker —
adında emoji olan tek bir kullanıcı, o adı kırpan her ekranı düşürür. Paket kırpmayı güvenli hale
getirir, bozuk gelen string'i onarır ve render öncesi doğrulama sağlar.

`Dart` · bağımlılık yok · 31 test · MIT

---

## Teknolojiler

| | |
|---|---|
| **Mobil** | Flutter · Dart · iOS · Android · Riverpod · Provider/MVVM · Freezed · Clean Architecture |
| **Backend & Bulut** | Firebase (Firestore, Auth, Cloud Functions, App Check, Remote Config) · TypeScript/Node · REST API |
| **Yayın & Araçlar** | RevenueCat · AdMob · CI/CD (GitHub Actions, Codemagic) · Git · Unit/Widget test |
| **Geçmiş** | Java · Spring Boot · PostgreSQL · React.js · Next.js |

---

## İletişim

[LinkedIn](https://www.linkedin.com/in/cemvuralyilmaz) · yilmazcemvural35@gmail.com

<sub>Yayındaki uygulamaların kaynak kodu, uygulama içi satın alma ve kullanıcı verisi içerdiği için özel repo'larda tutuluyor.</sub>
