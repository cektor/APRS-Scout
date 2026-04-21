# Privacy Policy for APRS Tracker

**App Name:** APRS Tracker
**Package Name:** com.qrv73.aprssend
**Developer:** Algsoft
**Last Updated:** April 21, 2026
**Effective Date:** April 21, 2026
**Version:** 3.0

---

## English Version

### 1. Introduction

This Privacy Policy describes how APRS Tracker ("we", "us", "our", or "the app"), developed by Algsoft, collects, uses, shares, and protects information when you use our Android mobile application. This application is designed for licensed amateur radio operators to transmit their position and messages via the APRS (Automatic Packet Reporting System) network.

We are committed to protecting your privacy and being transparent about our data practices. This policy is provided in both English and Turkish to serve our international user base.

APRS Tracker supports the following interface languages: **English** (default), **Turkish**, **German**, **French**, and **Spanish**. The app automatically adapts to the system language of your device.

**Developer Contact:**
- **Company:** Algsoft
- **Email:** info@algsoft.net.tr
- **Website:** https://algsoft.net.tr
- **Project Website:** https://qrv73.com

---

### 2. Location Data — Collection, Use, Sharing, and Retention

**This section provides a detailed explanation of how our app accesses and processes Location Data, as required by Google Play's User Data Policy.**

#### 2.1 What Location Data We Collect

Our app collects the following location data from your device:

- **Precise (GPS) Location (Latitude and Longitude):** Collected using the device's GPS sensor and Google Play Services Fused Location Provider to determine your exact geographic coordinates.
- **Altitude:** Collected from the device's GPS sensor to determine your elevation above sea level.
- **Approximate (Coarse) Location:** Used as a fallback when precise GPS signal is unavailable.

#### 2.2 How Location Data Is Collected

- Location data is collected through the Android `FusedLocationProviderClient` API provided by Google Play Services.
- The app requests `ACCESS_FINE_LOCATION` permission for precise GPS coordinates.
- The app requests `ACCESS_COARSE_LOCATION` permission as a fallback for approximate coordinates.
- The app optionally requests `ACCESS_BACKGROUND_LOCATION` permission only when continuous tracking mode is activated, allowing location updates while the app runs in the background via a foreground service.

#### 2.3 When Location Data Is Collected

- **Manual Send:** Location data is collected once when you press the "Send Location" button.
- **Continuous Tracking:** When you start tracking mode ("Start Tracking"), location data is collected at regular intervals (configurable by the user, default: 120 seconds) as long as tracking is active.
- **No Passive Collection:** The app does **NOT** collect location data when it is closed or when tracking is not active. Location is collected **only** when you explicitly initiate a send or start tracking.

#### 2.4 How Location Data Is Used

Location data is used for the following purposes:

1. **APRS Position Reporting (Primary Purpose):** Your GPS coordinates (latitude, longitude, altitude) are formatted into an APRS-standard position packet and transmitted to APRS-IS (APRS Internet Service) servers. This is the core and primary functionality of the app — enabling amateur radio operators to share their position on the public APRS network.

2. **Grid Square Calculation:** Your coordinates are converted to a Maidenhead grid locator (grid square) for display within the app. This calculation is performed locally on your device.

3. **Weather Data Retrieval (Optional):** If you enable the weather feature, your latitude and longitude are sent to the Open-Meteo weather API to retrieve current weather conditions for your location. Only geographic coordinates are sent — no personal identifiers.

#### 2.5 How Location Data Is Shared

Location data is shared with the following third-party services:

| Recipient | Data Shared | Purpose | Public? |
|-----------|------------|---------|---------|
| **APRS-IS Servers** (e.g., rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net) | Latitude, longitude, altitude, callsign, timestamp, comment | Transmitting APRS position packets to the amateur radio network | **Yes — APRS is a public network. All transmitted data is publicly visible to anyone.** |
| **Open-Meteo API** (api.open-meteo.com) | Latitude, longitude only | Fetching weather data for your location (optional feature) | No |

**Important Notice:** APRS-IS is a publicly accessible amateur radio network. When you transmit your position via this app, your callsign and location become publicly visible on websites such as aprs.fi, aprs.direct, and other APRS tracking platforms. This is the intended and standard behavior of the APRS system.

#### 2.6 Location Data Storage and Retention

- **No Server Storage:** We (Algsoft) do **NOT** store your location data on any server we own or operate.
- **No Cloud Backup:** Location data is **NOT** backed up to any cloud service.
- **Device Memory Only:** Location data is held temporarily in your device's RAM (volatile memory) only while the app is running and actively transmitting.
- **No Persistent Local Storage:** Location data is **NOT** written to a local database or file on your device.
- **Automatic Deletion:** Location data in device memory is cleared when the app is closed or when tracking is stopped.
- **Third-Party Retention:** Once transmitted to APRS-IS servers, the data is subject to the data retention policies of the APRS-IS network and any services that archive APRS data (such as aprs.fi). We have no control over third-party data retention.

#### 2.7 User Control Over Location Data

- **Start/Stop Control:** You have full control to start and stop location sharing at any time using the app's interface buttons.
- **Permission Management:** You can revoke location permissions at any time through your device's Android Settings > Apps > APRS Tracker > Permissions.
- **Background Location:** Background location access is only requested when you start continuous tracking. You can deny this permission and still use the manual single-send feature.
- **Interval Configuration:** When using continuous tracking, you can configure the transmission interval to control how frequently your location is shared.

---

### 3. Other Data We Collect

#### 3.1 User-Provided Configuration Data

The following data is provided by you and stored **locally on your device only** using Android SharedPreferences:

- **Amateur Radio Callsign:** Required for APRS authentication and identification on the network.
- **APRS Server Settings:** Server address, port number, and connection preferences.
- **Transmission Settings:** Update interval, status comment text, symbol table, and symbol code.
- **Weather Feature Toggle:** Whether the optional weather feature is enabled or disabled.

This configuration data is **never** transmitted to Algsoft servers. It is used only to configure how the app connects to APRS-IS and formats your APRS packets.

#### 3.2 APRS Messages

- APRS messages you send to and receive from other amateur radio operators are temporarily stored in your device's memory (RAM) for display within the app.
- Sent messages are transmitted to APRS-IS servers and become publicly visible on the APRS network.
- Message history is **not** persisted to disk and is cleared when the app is closed.

#### 3.3 APRS Log Data

- The app can display a real-time log of APRS packets received from the APRS-IS network (Stream tab).
- This log data is held temporarily in memory for display purposes and is cleared when the app is closed or the log view is cleared.

#### 3.4 App Announcements

- The app fetches announcement content from `https://algsoft.net.tr/uygulama-duyurulari/` to display developer announcements and updates.
- This request does not transmit any personal data or location data. Only a standard HTTPS request is made to retrieve the webpage content.

---

### 4. Data We Do NOT Collect

We want to be completely transparent. The following data types are **NOT** collected, accessed, stored, or transmitted by this app:

- Personal information (name, email address, physical address, phone number)
- Financial or payment information
- Health and fitness data
- Photos, videos, or audio files
- Files and documents
- Calendar events or contacts
- Call logs or SMS messages
- Device identifiers (IMEI, Android ID, MAC address, advertising ID)
- App usage analytics or behavioral data
- Web browsing history
- Crash reports or performance diagnostics (no analytics SDK is integrated)

---

### 5. Third-Party Services

Our app connects to the following external services:

#### 5.1 APRS-IS (APRS Internet Service) Servers

- **Purpose:** Core app functionality — transmitting and receiving APRS packets.
- **Data Transmitted:** Callsign, GPS coordinates (latitude, longitude, altitude), timestamp, status comments, and APRS messages.
- **Connection Type:** Unencrypted TCP/IP (standard APRS protocol — APRS is not an encrypted protocol by design, as it is an amateur radio standard).
- **Default Port:** 14580
- **Available Servers:** rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net, soam.aprs2.net, aunz.aprs2.net, aprs1.hamnet.cloud, aprs2.hamnet.cloud, aprs3.hamnet.cloud, aprs.hc.r1.ampr.org, and user-configurable custom servers.
- **Privacy Note:** All data transmitted to APRS-IS is publicly accessible. This is inherent to the APRS system design.
- **More Information:** http://www.aprs-is.net/

#### 5.2 Open-Meteo Weather API

- **Purpose:** Retrieving current weather conditions (optional feature).
- **Data Transmitted:** Geographic coordinates (latitude, longitude) only.
- **Data Received:** Temperature, humidity, atmospheric pressure, wind speed, wind direction, and wind gusts.
- **Connection Type:** HTTPS (encrypted).
- **Privacy Policy:** https://open-meteo.com/en/terms
- **No Personal Data:** No personal identifiers, device information, or account data is sent.

#### 5.3 APRS.fi Map Service

- **Purpose:** Displaying APRS stations on an interactive map within the app (Map tab, loaded via WebView).
- **Data Shared:** Standard web request data (IP address, user agent) when loading the map page.
- **Connection Type:** HTTPS (encrypted).
- **Privacy Policy:** https://aprs.fi/page/privacy

#### 5.4 Algsoft Announcement Service

- **Purpose:** Displaying developer announcements and app update notifications.
- **URL:** https://algsoft.net.tr/uygulama-duyurulari/
- **Data Transmitted:** No personal or location data — only a standard HTTPS page request.
- **Data Received:** HTML content containing announcement text.

---

### 6. Android Permissions

The app requests the following Android permissions. Each permission is explained below:

| Permission | Purpose | Required? |
|------------|---------|-----------|
| `ACCESS_FINE_LOCATION` | To obtain precise GPS coordinates (latitude, longitude) for APRS position reports. This is the core functionality of the app. | **Yes** |
| `ACCESS_COARSE_LOCATION` | To obtain approximate location as a fallback when GPS is unavailable. | **Yes** |
| `ACCESS_BACKGROUND_LOCATION` | To continue collecting and transmitting location data when the app is in the background during continuous tracking mode. Only requested when you start tracking. | **Optional** |
| `INTERNET` | To connect to APRS-IS servers for transmitting/receiving APRS packets, to fetch weather data from Open-Meteo API, to load APRS.fi maps, and to fetch announcements. | **Yes** |
| `FOREGROUND_SERVICE` | To run a foreground service with a persistent notification during continuous tracking, ensuring the operating system does not terminate the tracking process. | **Yes** |
| `FOREGROUND_SERVICE_LOCATION` | Required by Android for foreground services that access location data. | **Yes** |
| `POST_NOTIFICATIONS` | To display notifications for incoming APRS messages and tracking status. | **Optional** |
| `WAKE_LOCK` | To prevent the device from sleeping during active tracking, ensuring position reports are sent at the configured intervals. | **Yes** |

---

### 7. Data Storage and Security

- **Local Storage Only:** All user configuration (callsign, server settings, preferences) is stored exclusively on your device using Android's SharedPreferences.
- **No Remote Database:** We do not operate any server or database that stores user data.
- **No Cloud Sync:** Your data is not synchronized to any cloud service.
- **Data Deletion:** Uninstalling the app removes all locally stored configuration data from your device. You can also clear app data from Android Settings at any time.
- **Transmission Security:** Connections to Open-Meteo API, APRS.fi, and Algsoft website use HTTPS (encrypted). Connections to APRS-IS servers use unencrypted TCP/IP as per the APRS protocol standard.

---

### 8. Children's Privacy

This app is designed exclusively for licensed amateur radio operators. It is not intended for use by children. We do not knowingly collect any information from children under the age of 13 (or under the age of 16 in the European Economic Area). If you believe a child has used this app, please contact us at info@algsoft.net.tr.

---

### 9. Your Rights and Choices

You have the following rights regarding your data:

- **Access and Control:** You can view all stored configuration data within the app's settings.
- **Location Permission:** You can grant or revoke location permission at any time via Android Settings.
- **Stop Sharing:** You can stop all data transmission by stopping tracking and closing the app.
- **Data Deletion:** You can delete all locally stored data by clearing app data in Android Settings or by uninstalling the app.
- **Background Location:** You can deny background location permission and still use the app for manual single position sends.

---

### 10. International Users

This app is available globally and supports English, Turkish, German, French, and Spanish interface languages. The app automatically adapts to your device's system language. Regardless of your location:

- No personal data is transferred to or stored on Algsoft servers.
- Location data is transmitted only to APRS-IS servers (which operate globally) and optionally to Open-Meteo API.
- You maintain full control over when and whether your location data is shared.

For users in the European Union / European Economic Area: You have additional rights under GDPR including the right to access, rectification, erasure, restriction of processing, data portability, and the right to object. Since we do not store any personal data on our servers, most of these rights are automatically fulfilled. For any GDPR-related inquiries, contact us at info@algsoft.net.tr.

For users in Turkey: This app complies with the Turkish Personal Data Protection Law (KVKK, Law No. 6698). No personal data is processed on our servers. For KVKK-related inquiries, contact us at info@algsoft.net.tr.

---

### 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. When we do:

- The "Last Updated" date at the top will be revised.
- Significant changes will be communicated through in-app announcements.
- The updated policy will be available at our project website and GitHub repository.
- Continued use of the app after changes constitutes acceptance of the updated policy.

---

### 12. Open Source

This app is open source. You can review the complete source code to independently verify our privacy practices. Transparency is a core value of our development process.

---

### 13. Contact Information

For any questions, concerns, or requests related to this Privacy Policy or your data:

- **Developer:** Algsoft
- **Email:** info@algsoft.net.tr
- **Website:** https://algsoft.net.tr
- **Project Website:** https://qrv73.com

---

### 14. Legal Compliance

This app and this Privacy Policy comply with:

- Google Play Developer Program Policies (including User Data Policy)
- Google Play Data Safety requirements
- European Union General Data Protection Regulation (GDPR)
- Turkish Personal Data Protection Law (KVKK, Law No. 6698)
- Android privacy and permission best practices
- Amateur radio regulations regarding APRS usage

---
---

## Türkçe Versiyon

### 1. Giriş

Bu Gizlilik Politikası, Algsoft tarafından geliştirilen APRS Tracker ("biz", "bizim" veya "uygulama") Android mobil uygulamamızı kullandığınızda bilgilerin nasıl toplandığını, kullanıldığını, paylaşıldığını ve korunduğunu açıklar. Bu uygulama, lisanslı amatör telsiz operatörlerinin APRS (Automatic Packet Reporting System — Otomatik Paket Raporlama Sistemi) ağı üzerinden konum ve mesaj iletmesi için tasarlanmıştır.

Gizliliğinizi korumaya ve veri uygulamalarımız konusunda şeffaf olmaya kararlıyız.

APRS Tracker şu arayüz dillerini destekler: **İngilizce** (varsayılan), **Türkçe**, **Almanca**, **Fransızca** ve **İspanyolca**. Uygulama, cihazınızın sistem diline otomatik olarak uyum sağlar.

**Geliştirici İletişim Bilgileri:**
- **Şirket:** Algsoft
- **E-posta:** info@algsoft.net.tr
- **Web Sitesi:** https://algsoft.net.tr
- **Proje Web Sitesi:** https://qrv73.com

---

### 2. Konum Verileri — Toplama, Kullanım, Paylaşım ve Saklama

**Bu bölüm, Google Play Kullanıcı Verileri Politikası gereğince, uygulamamızın Konum Verilerine nasıl eriştiğini ve işlediğini ayrıntılı olarak açıklamaktadır.**

#### 2.1 Hangi Konum Verilerini Topluyoruz

Uygulamamız cihazınızdan aşağıdaki konum verilerini toplar:

- **Hassas (GPS) Konum (Enlem ve Boylam):** Tam coğrafi koordinatlarınızı belirlemek için cihazınızın GPS sensörü ve Google Play Services Fused Location Provider kullanılarak toplanır.
- **Yükseklik (Altitude):** Deniz seviyesinden yüksekliğinizi belirlemek için cihazınızın GPS sensöründen toplanır.
- **Yaklaşık (Kaba) Konum:** Hassas GPS sinyali mevcut olmadığında yedek olarak kullanılır.

#### 2.2 Konum Verileri Nasıl Toplanır

- Konum verileri, Google Play Services tarafından sağlanan Android `FusedLocationProviderClient` API'si aracılığıyla toplanır.
- Uygulama, hassas GPS koordinatları için `ACCESS_FINE_LOCATION` izni talep eder.
- Uygulama, yaklaşık koordinatlar için yedek olarak `ACCESS_COARSE_LOCATION` izni talep eder.
- Uygulama, yalnızca sürekli takip modu etkinleştirildiğinde isteğe bağlı olarak `ACCESS_BACKGROUND_LOCATION` izni talep eder.

#### 2.3 Konum Verileri Ne Zaman Toplanır

- **Manuel Gönderim:** "Send Location" (Konum Gönder) düğmesine bastığınızda konum verileri bir kez toplanır.
- **Sürekli Takip:** Takip modunu başlattığınızda ("Start Tracking"), takip aktif olduğu sürece konum verileri düzenli aralıklarla (kullanıcı tarafından yapılandırılabilir, varsayılan: 120 saniye) toplanır.
- **Pasif Toplama Yok:** Uygulama kapalıyken veya takip aktif değilken konum verileri **TOPLANMAZ**.

#### 2.4 Konum Verileri Nasıl Kullanılır

1. **APRS Konum Raporlama (Ana Amaç):** GPS koordinatlarınız APRS standart konum paketine dönüştürülür ve APRS-IS sunucularına iletilir.
2. **Grid Square Hesaplama:** Koordinatlarınız Maidenhead grid lokator formatına dönüştürülür. Bu hesaplama tamamen cihazınızda yerel olarak yapılır.
3. **Hava Durumu Verisi Alma (İsteğe Bağlı):** Hava durumu özelliğini etkinleştirirseniz enlem ve boylamınız Open-Meteo API'sine gönderilir.

#### 2.5 Konum Verileri Nasıl Paylaşılır

| Alıcı | Paylaşılan Veri | Amaç | Halka Açık mı? |
|--------|----------------|------|----------------|
| **APRS-IS Sunucuları** | Enlem, boylam, yükseklik, çağrı işareti, zaman damgası, yorum | APRS konum paketlerinin iletilmesi | **Evet — APRS halka açık bir ağdır.** |
| **Open-Meteo API** | Yalnızca enlem ve boylam | Hava durumu verisi alma (isteğe bağlı) | Hayır |

**Önemli Uyarı:** APRS-IS halka açık bir ağdır. İlettiğiniz konum ve çağrı işareti aprs.fi gibi platformlarda herkese görünür olur.

#### 2.6 Konum Verisi Saklama ve Tutma

- **Sunucu Depolaması Yok:** Konum verilerinizi sunucularımızda **SAKLAMIYORUZ**.
- **Bulut Yedekleme Yok:** Konum verileri herhangi bir bulut hizmetine **YEDEKLENMİYOR**.
- **Yalnızca Cihaz Belleği:** Veriler yalnızca uygulama çalışırken RAM'de geçici olarak tutulur.
- **Otomatik Silme:** Uygulama kapatıldığında veya takip durdurulduğunda silinir.

#### 2.7 Konum Verileri Üzerinde Kullanıcı Kontrolü

- **Başlatma/Durdurma Kontrolü:** Konum paylaşımını istediğiniz zaman başlatabilir ve durdurabilirsiniz.
- **İzin Yönetimi:** Android Ayarları > Uygulamalar > APRS Tracker > İzinler üzerinden konum izinlerini istediğiniz zaman iptal edebilirsiniz.
- **Arka Plan Konumu:** Yalnızca sürekli takibi başlattığınızda istenir.
- **Aralık Yapılandırma:** İletim aralığını yapılandırabilirsiniz.

---

### 3. Topladığımız Diğer Veriler

#### 3.1 Kullanıcı Tarafından Sağlanan Yapılandırma Verileri

Android SharedPreferences kullanılarak **yalnızca cihazınızda yerel olarak** saklanır:

- Amatör Telsiz Çağrı İşareti
- APRS Sunucu Ayarları (sunucu adresi, port numarası)
- İletim Ayarları (aralık, yorum, sembol)
- Hava Durumu Özelliği tercihi

Bu veriler **hiçbir zaman** Algsoft sunucularına iletilmez.

#### 3.2 APRS Mesajları

- Gönderip aldığınız mesajlar RAM'de geçici olarak saklanır.
- Gönderilen mesajlar APRS-IS'te herkese açık olur.
- Mesaj geçmişi diske kaydedilmez, uygulama kapatılınca silinir.

#### 3.3 APRS Log Verileri

- Akış sekmesinde görüntülenen gerçek zamanlı paket günlüğü geçici bellekte tutulur.
- Uygulama kapatıldığında veya günlük temizlendiğinde silinir.

#### 3.4 Uygulama Duyuruları

- `https://algsoft.net.tr/uygulama-duyurulari/` adresinden duyuru içeriği çekilir.
- Hiçbir kişisel veri veya konum verisi iletilmez.

---

### 4. Toplamadığımız Veriler

Aşağıdaki veriler bu uygulama tarafından **TOPLANMAZ, ERİŞİLMEZ, SAKLANMAZ veya İLETİLMEZ:**

- Kişisel bilgiler (ad, e-posta, adres, telefon)
- Finansal veya ödeme bilgileri
- Sağlık ve fitness verileri
- Fotoğraf, video veya ses dosyaları
- Takvim etkinlikleri veya kişiler
- Cihaz tanımlayıcıları (IMEI, Android ID, MAC adresi)
- Uygulama kullanım analitiği
- Çökme raporları (hiçbir analitik SDK entegre edilmemiştir)

---

### 5. Üçüncü Taraf Hizmetler

#### 5.1 APRS-IS Sunucuları

- **Amaç:** APRS paketlerinin iletilmesi ve alınması.
- **İletilen Veriler:** Çağrı işareti, GPS koordinatları, zaman damgası, yorumlar ve mesajlar.
- **Bağlantı:** Şifrelenmemiş TCP/IP (APRS protokolü standardı), port 14580.
- **Sunucular:** rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net, soam.aprs2.net, aunz.aprs2.net, aprs1.hamnet.cloud, aprs2.hamnet.cloud, aprs3.hamnet.cloud, aprs.hc.r1.ampr.org

#### 5.2 Open-Meteo Hava Durumu API

- **Amaç:** Güncel hava durumu (isteğe bağlı).
- **İletilen:** Yalnızca coğrafi koordinatlar.
- **Bağlantı:** HTTPS (şifreli).

#### 5.3 APRS.fi Harita Servisi

- **Amaç:** Harita sekmesinde APRS istasyonlarını WebView üzerinden görüntüleme.
- **Bağlantı:** HTTPS (şifreli).

#### 5.4 Algsoft Duyuru Servisi

- **Amaç:** Geliştirici duyuruları.
- **URL:** https://algsoft.net.tr/uygulama-duyurulari/
- **İletilen:** Kişisel veya konum verisi yok.

---

### 6. Android İzinleri

| İzin | Amaç | Gerekli mi? |
|------|------|-------------|
| `ACCESS_FINE_LOCATION` | Hassas GPS koordinatları almak. | **Evet** |
| `ACCESS_COARSE_LOCATION` | GPS yokken yaklaşık konum yedek. | **Evet** |
| `ACCESS_BACKGROUND_LOCATION` | Arka planda sürekli takip. Yalnızca takip başlatıldığında istenir. | **İsteğe Bağlı** |
| `INTERNET` | APRS-IS, Open-Meteo, APRS.fi ve duyuru bağlantıları. | **Evet** |
| `FOREGROUND_SERVICE` | Sürekli takip için ön plan servisi. | **Evet** |
| `FOREGROUND_SERVICE_LOCATION` | Konum erişen ön plan servisleri için Android zorunluluğu. | **Evet** |
| `POST_NOTIFICATIONS` | Mesaj ve takip bildirimleri. | **İsteğe Bağlı** |
| `WAKE_LOCK` | Aktif takipte cihazın uyumasını önlemek. | **Evet** |

---

### 7. Veri Depolama ve Güvenlik

- Tüm kullanıcı yapılandırması yalnızca cihazda Android SharedPreferences ile saklanır.
- Kullanıcı verilerini saklayan sunucu veya veritabanı işletmiyoruz.
- Uygulamayı kaldırmak tüm yerel yapılandırma verilerini siler.
- Open-Meteo, APRS.fi ve Algsoft bağlantıları HTTPS kullanır; APRS-IS bağlantıları APRS protokolü gereği şifrelenmemiş TCP/IP kullanır.

---

### 8. Çocukların Gizliliği

Bu uygulama yalnızca lisanslı amatör telsiz operatörleri için tasarlanmıştır. 13 yaşın altındaki çocuklardan bilerek bilgi toplamıyoruz.

---

### 9. Haklarınız ve Seçimleriniz

- Konum iznini Android Ayarları üzerinden istediğiniz zaman iptal edebilirsiniz.
- Takibi durdurarak tüm veri iletimini durdurabilirsiniz.
- Uygulama verilerini Android Ayarları'ndan temizleyerek veya uygulamayı kaldırarak tüm yerel verileri silebilirsiniz.

---

### 10. Uluslararası Kullanıcılar

APRS Tracker dünya genelinde kullanılabilir ve **İngilizce (varsayılan), Türkçe, Almanca, Fransızca ve İspanyolca** arayüz dillerini destekler. Uygulama, cihazın sistem diline otomatik uyum sağlar.

- Algsoft sunucularında hiçbir kişisel veri saklanmaz.
- Konum verileri yalnızca APRS-IS ve isteğe bağlı Open-Meteo'ya iletilir.

**AB / AEA kullanıcıları:** GDPR kapsamında erişim, düzeltme, silme ve veri taşınabilirliği haklarınız bulunmaktadır. Sunucularımızda kişisel veri saklamadığımızdan bu hakların büyük çoğunluğu otomatik olarak karşılanmaktadır. Sorularınız için: info@algsoft.net.tr

**Türkiye kullanıcıları:** Uygulama KVKK (6698 sayılı Kanun) uyumludur. Sorularınız için: info@algsoft.net.tr

---

### 11. Bu Politikadaki Değişiklikler

- "Son Güncelleme" tarihi revize edilecektir.
- Önemli değişiklikler uygulama içi duyurularla bildirilecektir.
- Güncellenmiş politika proje web sitesinde yayınlanacaktır.

---

### 12. Açık Kaynak

Bu uygulama açık kaynaklıdır. Gizlilik uygulamalarımızı bağımsız olarak doğrulamak için kaynak kodun tamamını inceleyebilirsiniz.

---

### 13. İletişim Bilgileri

- **Geliştirici:** Algsoft
- **E-posta:** info@algsoft.net.tr
- **Web Sitesi:** https://algsoft.net.tr
- **Proje Web Sitesi:** https://qrv73.com

---

### 14. Yasal Uyumluluk

- Google Play Geliştirici Program Politikaları
- Google Play Veri Güvenliği gereksinimleri
- Avrupa Birliği GDPR
- Türkiye KVKK (6698 sayılı Kanun)
- Android gizlilik ve izin en iyi uygulamaları
- APRS kullanımına ilişkin amatör telsiz düzenlemeleri

---

**Version / Versiyon:** 3.0
**Effective Date / Yürürlük Tarihi:** April 21, 2026
**App Package Name / Uygulama Paket Adı:** com.qrv73.aprssend
**Developer / Geliştirici:** Algsoft
**Contact / İletişim:** info@algsoft.net.tr
