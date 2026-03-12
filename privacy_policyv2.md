# Privacy Policy for APRS Gönder (APRS İzci)

**App Name:** APRS Gönder (APRS İzci)
**Package Name:** com.qrv73.aprsgonder
**Developer:** Algsoft
**Last Updated:** March 12, 2026
**Effective Date:** March 12, 2026
**Version:** 2.0

---

## English Version

### 1. Introduction

This Privacy Policy describes how APRS Gönder (also known as "APRS İzci") ("we", "us", "our", or "the app"), developed by Algsoft, collects, uses, shares, and protects information when you use our Android mobile application. This application is designed for licensed amateur radio operators to transmit their position and messages via the APRS (Automatic Packet Reporting System) network.

We are committed to protecting your privacy and being transparent about our data practices. This policy is provided in both English and Turkish to serve our international user base.

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

- **Manual Send:** Location data is collected once when you press the "Konum Gönder" (Send Location) button.
- **Continuous Tracking:** When you start tracking mode ("Takibi Başlat"), location data is collected at regular intervals (configurable by the user, default: 120 seconds) as long as tracking is active.
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
- **Permission Management:** You can revoke location permissions at any time through your device's Android Settings > Apps > APRS Gönder > Permissions.
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

- The app can display a real-time log of APRS packets received from the APRS-IS network.
- This log data is held temporarily in memory for display purposes and is cleared when the app is closed or the log view is cleared.

#### 3.4 App Announcements

- The app fetches announcement content from `https://algsoft.net.tr/uygulama-duyurulari/` to display developer announcements and updates.
- This request does not transmit any personal data or location data. Only a standard HTTP request is made to retrieve the webpage content.

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
- **Available Servers:** rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net, and user-configurable custom servers.
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

- **Purpose:** Displaying APRS stations on an interactive map within the app (loaded via WebView).
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

This app is available globally. Regardless of your location:

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

Bu Gizlilik Politikası, Algsoft tarafından geliştirilen APRS Gönder (diğer adıyla "APRS İzci") ("biz", "bizim" veya "uygulama") Android mobil uygulamamızı kullandığınızda bilgilerin nasıl toplandığını, kullanıldığını, paylaşıldığını ve korunduğunu açıklar. Bu uygulama, lisanslı amatör telsiz operatörlerinin APRS (Automatic Packet Reporting System — Otomatik Paket Raporlama Sistemi) ağı üzerinden konum ve mesaj iletmesi için tasarlanmıştır.

Gizliliğinizi korumaya ve veri uygulamalarımız konusunda şeffaf olmaya kararlıyız. Bu politika, uluslararası kullanıcı tabanımıza hizmet etmek amacıyla hem İngilizce hem de Türkçe olarak sunulmaktadır.

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
- Uygulama, yalnızca sürekli takip modu etkinleştirildiğinde isteğe bağlı olarak `ACCESS_BACKGROUND_LOCATION` izni talep eder; bu izin, uygulamanın ön plan servisi aracılığıyla arka planda çalışırken konum güncellemeleri almasını sağlar.

#### 2.3 Konum Verileri Ne Zaman Toplanır

- **Manuel Gönderim:** "Konum Gönder" düğmesine bastığınızda konum verileri bir kez toplanır.
- **Sürekli Takip:** Takip modunu başlattığınızda ("Takibi Başlat"), takip aktif olduğu sürece konum verileri düzenli aralıklarla (kullanıcı tarafından yapılandırılabilir, varsayılan: 120 saniye) toplanır.
- **Pasif Toplama Yok:** Uygulama kapalıyken veya takip aktif değilken konum verileri **TOPLANMAZ**. Konum, yalnızca siz açıkça bir gönderim başlattığınızda veya takibi başlattığınızda toplanır.

#### 2.4 Konum Verileri Nasıl Kullanılır

Konum verileri aşağıdaki amaçlarla kullanılır:

1. **APRS Konum Raporlama (Ana Amaç):** GPS koordinatlarınız (enlem, boylam, yükseklik) APRS standart konum paketine dönüştürülür ve APRS-IS (APRS İnternet Servisi) sunucularına iletilir. Bu, uygulamanın temel ve birincil işlevidir — amatör telsiz operatörlerinin konumlarını halka açık APRS ağında paylaşmalarını sağlar.

2. **Grid Square Hesaplama:** Koordinatlarınız, uygulama içinde görüntülenmek üzere Maidenhead grid lokator (grid square) formatına dönüştürülür. Bu hesaplama tamamen cihazınızda yerel olarak yapılır.

3. **Hava Durumu Verisi Alma (İsteğe Bağlı):** Hava durumu özelliğini etkinleştirirseniz, konumunuz için güncel hava durumu koşullarını almak amacıyla enlem ve boylamınız Open-Meteo hava durumu API'sine gönderilir. Yalnızca coğrafi koordinatlar gönderilir — kişisel tanımlayıcı bilgi gönderilmez.

#### 2.5 Konum Verileri Nasıl Paylaşılır

Konum verileri aşağıdaki üçüncü taraf hizmetlerle paylaşılır:

| Alıcı | Paylaşılan Veri | Amaç | Halka Açık mı? |
|--------|----------------|------|----------------|
| **APRS-IS Sunucuları** (örn. rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net) | Enlem, boylam, yükseklik, çağrı işareti, zaman damgası, yorum | APRS konum paketlerinin amatör telsiz ağına iletilmesi | **Evet — APRS halka açık bir ağdır. İletilen tüm veriler herkes tarafından görülebilir.** |
| **Open-Meteo API** (api.open-meteo.com) | Yalnızca enlem ve boylam | Konumunuz için hava durumu verisi alma (isteğe bağlı özellik) | Hayır |

**Önemli Uyarı:** APRS-IS, halka açık bir amatör telsiz ağıdır. Bu uygulama aracılığıyla konumunuzu ilettiğinizde, çağrı işaretiniz ve konumunuz aprs.fi, aprs.direct ve diğer APRS takip platformlarında herkese açık olarak görünür hale gelir. Bu, APRS sisteminin amaçlanan ve standart davranışıdır.

#### 2.6 Konum Verisi Saklama ve Tutma

- **Sunucu Depolaması Yok:** Biz (Algsoft) konum verilerinizi sahip olduğumuz veya işlettiğimiz herhangi bir sunucuda **SAKLAMIYORUZ**.
- **Bulut Yedekleme Yok:** Konum verileri herhangi bir bulut hizmetine **YEDEKLENMİYOR**.
- **Yalnızca Cihaz Belleği:** Konum verileri, yalnızca uygulama çalışırken ve aktif olarak iletim yaparken cihazınızın RAM'inde (geçici bellek) geçici olarak tutulur.
- **Kalıcı Yerel Depolama Yok:** Konum verileri cihazınızda yerel bir veritabanına veya dosyaya **YAZILMAZ**.
- **Otomatik Silme:** Cihaz belleğindeki konum verileri, uygulama kapatıldığında veya takip durdurulduğunda silinir.
- **Üçüncü Taraf Saklama:** APRS-IS sunucularına iletildikten sonra veriler, APRS-IS ağının ve APRS verilerini arşivleyen hizmetlerin (aprs.fi gibi) veri saklama politikalarına tabidir. Üçüncü taraf veri saklama üzerinde kontrolümüz yoktur.

#### 2.7 Konum Verileri Üzerinde Kullanıcı Kontrolü

- **Başlatma/Durdurma Kontrolü:** Uygulamanın arayüz düğmelerini kullanarak konum paylaşımını istediğiniz zaman başlatabilir ve durdurabilirsiniz.
- **İzin Yönetimi:** Android Ayarları > Uygulamalar > APRS Gönder > İzinler üzerinden konum izinlerini istediğiniz zaman iptal edebilirsiniz.
- **Arka Plan Konumu:** Arka plan konum erişimi yalnızca sürekli takibi başlattığınızda istenir. Bu izni reddedebilir ve yine de manuel tekli gönderim özelliğini kullanabilirsiniz.
- **Aralık Yapılandırma:** Sürekli takip kullanırken, konumunuzun ne sıklıkla paylaşılacağını kontrol etmek için iletim aralığını yapılandırabilirsiniz.

---

### 3. Topladığımız Diğer Veriler

#### 3.1 Kullanıcı Tarafından Sağlanan Yapılandırma Verileri

Aşağıdaki veriler sizin tarafınızdan sağlanır ve Android SharedPreferences kullanılarak **yalnızca cihazınızda yerel olarak** saklanır:

- **Amatör Telsiz Çağrı İşareti:** APRS kimlik doğrulama ve ağdaki tanımlama için gereklidir.
- **APRS Sunucu Ayarları:** Sunucu adresi, port numarası ve bağlantı tercihleri.
- **İletim Ayarları:** Güncelleme aralığı, durum yorum metni, sembol tablosu ve sembol kodu.
- **Hava Durumu Özelliği:** İsteğe bağlı hava durumu özelliğinin etkin veya devre dışı olup olmadığı.

Bu yapılandırma verileri **hiçbir zaman** Algsoft sunucularına iletilmez. Yalnızca uygulamanın APRS-IS'e nasıl bağlanacağını ve APRS paketlerinizi nasıl biçimlendireceğini yapılandırmak için kullanılır.

#### 3.2 APRS Mesajları

- Diğer amatör telsiz operatörlerine gönderdiğiniz ve onlardan aldığınız APRS mesajları, uygulama içinde görüntülenmek üzere cihazınızın belleğinde (RAM) geçici olarak saklanır.
- Gönderilen mesajlar APRS-IS sunucularına iletilir ve APRS ağında herkese açık olarak görünür hale gelir.
- Mesaj geçmişi diske **kaydedilmez** ve uygulama kapatıldığında silinir.

#### 3.3 APRS Log Verileri

- Uygulama, APRS-IS ağından alınan APRS paketlerinin gerçek zamanlı günlüğünü görüntüleyebilir.
- Bu günlük verileri görüntüleme amacıyla geçici olarak bellekte tutulur ve uygulama kapatıldığında veya günlük görünümü temizlendiğinde silinir.

#### 3.4 Uygulama Duyuruları

- Uygulama, geliştirici duyurularını ve güncellemelerini görüntülemek için `https://algsoft.net.tr/uygulama-duyurulari/` adresinden duyuru içeriği çeker.
- Bu istek herhangi bir kişisel veri veya konum verisi iletmez. Yalnızca web sayfası içeriğini almak için standart bir HTTPS isteği yapılır.

---

### 4. TOPLAMADĞIMIZ Veriler

Tamamen şeffaf olmak istiyoruz. Aşağıdaki veri türleri bu uygulama tarafından **TOPLANMAZ, ERİŞİLMEZ, SAKLANMAZ veya İLETİLMEZ:**

- Kişisel bilgiler (ad, e-posta adresi, fiziksel adres, telefon numarası)
- Finansal veya ödeme bilgileri
- Sağlık ve fitness verileri
- Fotoğraflar, videolar veya ses dosyaları
- Dosyalar ve belgeler
- Takvim etkinlikleri veya kişiler
- Arama kayıtları veya SMS mesajları
- Cihaz tanımlayıcıları (IMEI, Android ID, MAC adresi, reklam kimliği)
- Uygulama kullanım analitiği veya davranışsal veriler
- Web tarama geçmişi
- Çökme raporları veya performans tanılama (hiçbir analitik SDK entegre edilmemiştir)

---

### 5. Üçüncü Taraf Hizmetler

Uygulamamız aşağıdaki harici hizmetlere bağlanır:

#### 5.1 APRS-IS (APRS İnternet Servisi) Sunucuları

- **Amaç:** Temel uygulama işlevselliği — APRS paketlerinin iletilmesi ve alınması.
- **İletilen Veriler:** Çağrı işareti, GPS koordinatları (enlem, boylam, yükseklik), zaman damgası, durum yorumları ve APRS mesajları.
- **Bağlantı Türü:** Şifrelenmemiş TCP/IP (standart APRS protokolü — APRS, bir amatör telsiz standardı olarak tasarım gereği şifreli bir protokol değildir).
- **Varsayılan Port:** 14580
- **Mevcut Sunucular:** rotate.aprs2.net, euro.aprs2.net, asia.aprs2.net, noam.aprs2.net ve kullanıcı tarafından yapılandırılabilir özel sunucular.
- **Gizlilik Notu:** APRS-IS'e iletilen tüm veriler herkese açık olarak erişilebilir. Bu, APRS sistem tasarımının doğasında vardır.
- **Daha Fazla Bilgi:** http://www.aprs-is.net/

#### 5.2 Open-Meteo Hava Durumu API

- **Amaç:** Güncel hava durumu koşullarını alma (isteğe bağlı özellik).
- **İletilen Veriler:** Yalnızca coğrafi koordinatlar (enlem, boylam).
- **Alınan Veriler:** Sıcaklık, nem, atmosfer basıncı, rüzgar hızı, rüzgar yönü ve rüzgar hamleleri.
- **Bağlantı Türü:** HTTPS (şifreli).
- **Gizlilik Politikası:** https://open-meteo.com/en/terms
- **Kişisel Veri Yok:** Kişisel tanımlayıcı, cihaz bilgisi veya hesap verisi gönderilmez.

#### 5.3 APRS.fi Harita Servisi

- **Amaç:** APRS istasyonlarını uygulama içinde etkileşimli bir harita üzerinde görüntüleme (WebView aracılığıyla yüklenir).
- **Paylaşılan Veriler:** Harita sayfası yüklenirken standart web istek verileri (IP adresi, kullanıcı aracısı).
- **Bağlantı Türü:** HTTPS (şifreli).
- **Gizlilik Politikası:** https://aprs.fi/page/privacy

#### 5.4 Algsoft Duyuru Servisi

- **Amaç:** Geliştirici duyurularını ve uygulama güncelleme bildirimlerini görüntüleme.
- **URL:** https://algsoft.net.tr/uygulama-duyurulari/
- **İletilen Veriler:** Kişisel veya konum verisi iletilmez — yalnızca standart bir HTTPS sayfa isteği yapılır.
- **Alınan Veriler:** Duyuru metni içeren HTML içerik.

---

### 6. Android İzinleri

Uygulama aşağıdaki Android izinlerini talep eder. Her izin aşağıda açıklanmıştır:

| İzin | Amaç | Gerekli mi? |
|------|------|-------------|
| `ACCESS_FINE_LOCATION` | APRS konum raporları için hassas GPS koordinatları (enlem, boylam) almak. Bu, uygulamanın temel işlevidir. | **Evet** |
| `ACCESS_COARSE_LOCATION` | GPS mevcut olmadığında yaklaşık konum almak için yedek. | **Evet** |
| `ACCESS_BACKGROUND_LOCATION` | Sürekli takip modu sırasında uygulama arka plandayken konum verisi toplamaya ve iletmeye devam etmek. Yalnızca takibi başlattığınızda istenir. | **İsteğe Bağlı** |
| `INTERNET` | APRS paketlerinin iletimi/alımı için APRS-IS sunucularına, hava durumu verisi için Open-Meteo API'sine, APRS.fi haritalarına ve duyurulara bağlanmak. | **Evet** |
| `FOREGROUND_SERVICE` | Sürekli takip sırasında kalıcı bildirimle bir ön plan servisi çalıştırmak, işletim sisteminin takip sürecini sonlandırmamasını sağlamak. | **Evet** |
| `FOREGROUND_SERVICE_LOCATION` | Konum verilerine erişen ön plan servisleri için Android tarafından zorunlu kılınır. | **Evet** |
| `POST_NOTIFICATIONS` | Gelen APRS mesajları ve takip durumu için bildirim görüntülemek. | **İsteğe Bağlı** |
| `WAKE_LOCK` | Aktif takip sırasında cihazın uyumasını önlemek, konum raporlarının yapılandırılan aralıklarla gönderilmesini sağlamak. | **Evet** |

---

### 7. Veri Depolama ve Güvenlik

- **Yalnızca Yerel Depolama:** Tüm kullanıcı yapılandırması (çağrı işareti, sunucu ayarları, tercihler) yalnızca cihazınızda Android SharedPreferences kullanılarak saklanır.
- **Uzak Veritabanı Yok:** Kullanıcı verilerini saklayan herhangi bir sunucu veya veritabanı işletmiyoruz.
- **Bulut Senkronizasyon Yok:** Verileriniz herhangi bir bulut hizmetine senkronize edilmez.
- **Veri Silme:** Uygulamayı kaldırmak, yerel olarak saklanan tüm yapılandırma verilerini cihazınızdan kaldırır. Ayrıca Android Ayarları'ndan istediğiniz zaman uygulama verilerini temizleyebilirsiniz.
- **İletim Güvenliği:** Open-Meteo API, APRS.fi ve Algsoft web sitesine bağlantılar HTTPS (şifreli) kullanır. APRS-IS sunucularına bağlantılar, APRS protokol standardı gereği şifrelenmemiş TCP/IP kullanır.

---

### 8. Çocukların Gizliliği

Bu uygulama yalnızca lisanslı amatör telsiz operatörleri için tasarlanmıştır. Çocuklar tarafından kullanılması amaçlanmamıştır. 13 yaşın altındaki (Avrupa Ekonomik Alanı'nda 16 yaşın altındaki) çocuklardan bilerek herhangi bir bilgi toplamıyoruz. Bir çocuğun bu uygulamayı kullandığını düşünüyorsanız, lütfen info@algsoft.net.tr adresinden bizimle iletişime geçin.

---

### 9. Haklarınız ve Seçimleriniz

Verilerinizle ilgili aşağıdaki haklara sahipsiniz:

- **Erişim ve Kontrol:** Saklanan tüm yapılandırma verilerini uygulamanın ayarları içinde görüntüleyebilirsiniz.
- **Konum İzni:** Android Ayarları üzerinden konum iznini istediğiniz zaman verebilir veya iptal edebilirsiniz.
- **Paylaşımı Durdurma:** Takibi durdurarak ve uygulamayı kapatarak tüm veri iletimini durdurabilirsiniz.
- **Veri Silme:** Android Ayarları'nda uygulama verilerini temizleyerek veya uygulamayı kaldırarak yerel olarak saklanan tüm verileri silebilirsiniz.
- **Arka Plan Konumu:** Arka plan konum iznini reddedebilir ve yine de uygulamayı manuel tekli konum gönderimleri için kullanabilirsiniz.

---

### 10. Uluslararası Kullanıcılar

Bu uygulama dünya genelinde kullanılabilir. Konumunuzdan bağımsız olarak:

- Algsoft sunucularına hiçbir kişisel veri aktarılmaz veya saklanmaz.
- Konum verileri yalnızca APRS-IS sunucularına (küresel olarak çalışan) ve isteğe bağlı olarak Open-Meteo API'sine iletilir.
- Konum verilerinizin ne zaman ve paylaşılıp paylaşılmayacağı konusunda tam kontrol sizde kalır.

Avrupa Birliği / Avrupa Ekonomik Alanı'ndaki kullanıcılar için: GDPR kapsamında erişim, düzeltme, silme, işleme kısıtlama, veri taşınabilirliği ve itiraz etme haklarınız bulunmaktadır. Sunucularımızda herhangi bir kişisel veri saklamadığımız için bu hakların çoğu otomatik olarak karşılanmaktadır. GDPR ile ilgili sorularınız için info@algsoft.net.tr adresinden bize ulaşabilirsiniz.

Türkiye'deki kullanıcılar için: Bu uygulama Kişisel Verilerin Korunması Kanunu'na (KVKK, 6698 sayılı Kanun) uygundur. Sunucularımızda hiçbir kişisel veri işlenmemektedir. KVKK ile ilgili sorularınız için info@algsoft.net.tr adresinden bize ulaşabilirsiniz.

---

### 11. Bu Politikadaki Değişiklikler

Bu Gizlilik Politikasını zaman zaman güncelleyebiliriz. Güncellediğimizde:

- Üstteki "Son Güncelleme" tarihi revize edilecektir.
- Önemli değişiklikler uygulama içi duyurularla bildirilecektir.
- Güncellenmiş politika proje web sitemizde ve GitHub depomuzda yayınlanacaktır.
- Değişikliklerden sonra uygulamayı kullanmaya devam etmek, güncellenmiş politikanın kabulü anlamına gelir.

---

### 12. Açık Kaynak

Bu uygulama açık kaynaklıdır. Gizlilik uygulamalarımızı bağımsız olarak doğrulamak için kaynak kodun tamamını inceleyebilirsiniz. Şeffaflık, geliştirme sürecimizin temel değeridir.

---

### 13. İletişim Bilgileri

Bu Gizlilik Politikası veya verilerinizle ilgili herhangi bir soru, endişe veya talep için:

- **Geliştirici:** Algsoft
- **E-posta:** info@algsoft.net.tr
- **Web Sitesi:** https://algsoft.net.tr
- **Proje Web Sitesi:** https://qrv73.com

---

### 14. Yasal Uyumluluk

Bu uygulama ve bu Gizlilik Politikası aşağıdakilere uygundur:

- Google Play Geliştirici Program Politikaları (Kullanıcı Verileri Politikası dahil)
- Google Play Veri Güvenliği gereksinimleri
- Avrupa Birliği Genel Veri Koruma Tüzüğü (GDPR)
- Türkiye Kişisel Verilerin Korunması Kanunu (KVKK, 6698 sayılı Kanun)
- Android gizlilik ve izin en iyi uygulamaları
- APRS kullanımına ilişkin amatör telsiz düzenlemeleri

---

**Version / Versiyon:** 2.0
**Effective Date / Yürürlük Tarihi:** March 12, 2026
**App Package Name / Uygulama Paket Adı:** com.qrv73.aprsgonder
**Developer / Geliştirici:** Algsoft
**Contact / İletişim:** info@algsoft.net.tr
