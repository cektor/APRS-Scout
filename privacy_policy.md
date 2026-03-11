# Privacy Policy / Gizlilik Politikası

**Last Updated / Son Güncelleme:** January 2025

---

## English Version

### Introduction

This Privacy Policy describes how APRS Gönder ("we", "our", or "the app") handles information when you use our mobile application. We are committed to protecting your privacy and being transparent about our data practices.

### Information We Collect

#### Location Data
- **What we collect:** The app accesses your device's GPS location (latitude, longitude, altitude) when you use the APRS tracking features.
- **How we use it:** Location data is used solely to transmit your position to APRS-IS (APRS Internet Service) servers according to your configured settings. This is the core functionality of amateur radio APRS tracking.
- **Storage:** Location data is NOT stored on our servers. It is only temporarily processed on your device and transmitted directly to third-party APRS-IS servers that you select.
- **Control:** You have complete control over when location data is shared. The app only accesses location when you explicitly start tracking or send a position report.

#### User-Provided Information
- **Callsign:** Your amateur radio callsign is required to use APRS services. This is stored locally on your device.
- **APRS Configuration:** Server settings, update intervals, comments, and symbol preferences are stored locally on your device.
- **Messages:** APRS messages you send and receive are temporarily stored locally on your device for display purposes only.

#### Weather Data
- **Source:** When enabled, the app fetches weather data from Open-Meteo API (a free, public weather service) based on your current location.
- **Usage:** Weather data is used to enhance your APRS position reports with meteorological information.
- **No Personal Data:** Weather requests only include geographic coordinates, no personal identifiers.

### Information We Do NOT Collect

- ❌ We do NOT collect, store, or transmit any personal information to our own servers
- ❌ We do NOT track your usage patterns or behavior
- ❌ We do NOT collect device identifiers (IMEI, MAC address, etc.)
- ❌ We do NOT access your contacts, photos, or other personal files
- ❌ We do NOT use analytics or tracking services
- ❌ We do NOT display advertisements or use advertising networks
- ❌ We do NOT sell, rent, or share any data with third parties for marketing purposes

### Third-Party Services

The app connects to external services that are essential for APRS functionality:

#### APRS-IS Servers
- **Purpose:** To transmit and receive APRS packets (position reports, messages, status updates)
- **Data Shared:** Your callsign, location coordinates, altitude, comments, and messages you choose to send
- **Privacy:** APRS-IS is a public amateur radio network. All data transmitted to APRS-IS becomes publicly accessible to other amateur radio operators. This is the intended design of the APRS system.
- **Servers Used:** You can select from multiple APRS-IS servers (e.g., rotate.aprs2.net, euro.aprs2.net, etc.)

#### Open-Meteo Weather API
- **Purpose:** To retrieve current weather conditions for your location
- **Data Shared:** Only geographic coordinates (latitude/longitude)
- **Privacy Policy:** https://open-meteo.com/en/terms

#### APRS.fi Map Service
- **Purpose:** To display APRS stations and activity on an interactive map
- **Data Shared:** When you view the map, your browser loads content from aprs.fi
- **Privacy Policy:** https://aprs.fi/page/privacy

### Data Storage and Security

- **Local Storage Only:** All user preferences, callsigns, and message history are stored exclusively on your device using Android's SharedPreferences and local memory.
- **No Cloud Backup:** We do not back up your data to any cloud service.
- **Data Deletion:** Uninstalling the app will remove all locally stored data from your device.
- **Transmission Security:** Connections to APRS-IS servers use standard TCP/IP protocols. Note that APRS is not an encrypted protocol by design.

### Permissions Explained

The app requests the following Android permissions:

| Permission | Purpose | Required |
|------------|---------|----------|
| `ACCESS_FINE_LOCATION` | To obtain precise GPS coordinates for APRS position reports | Yes |
| `ACCESS_COARSE_LOCATION` | Fallback for approximate location | Yes |
| `ACCESS_BACKGROUND_LOCATION` | To continue tracking when app is in background | Optional* |
| `INTERNET` | To connect to APRS-IS servers and weather API | Yes |
| `FOREGROUND_SERVICE` | To maintain tracking service while app is minimized | Yes |
| `FOREGROUND_SERVICE_LOCATION` | Required for location-based foreground service | Yes |
| `POST_NOTIFICATIONS` | To notify you of incoming APRS messages | Optional |
| `WAKE_LOCK` | To keep device awake during active tracking | Yes |

*Background location is only requested when you start continuous tracking mode.

### Children's Privacy

This app is designed for licensed amateur radio operators. We do not knowingly collect information from children under 13. If you are under 13, please do not use this app without parental supervision.

### Your Rights and Choices

- **Location Control:** You can enable/disable location access at any time through Android settings
- **Data Deletion:** Clear app data or uninstall to remove all local information
- **Tracking Control:** You have full control to start/stop APRS tracking at any time
- **Message Privacy:** You control what messages you send; received messages can be cleared manually

### Changes to This Policy

We may update this Privacy Policy from time to time. Any changes will be posted within the app and on our GitHub repository. Continued use of the app after changes constitutes acceptance of the updated policy.

### Open Source

This app is open source. You can review the complete source code to verify our privacy practices at: [GitHub Repository URL]

### Contact Information

For questions or concerns about this Privacy Policy, please contact:

- **Developer:** Algsoft
- **Email:** info@algsoft.net.tr
- **Website:** https://algsoft.net.tr
- **Project Website:** https://qrv73.com

### Legal Compliance

This app complies with:
- Google Play Store Data Safety requirements
- Android privacy best practices
- Amateur radio regulations regarding APRS usage

---

## Türkçe Versiyon

### Giriş

Bu Gizlilik Politikası, APRS Gönder ("biz", "bizim" veya "uygulama") mobil uygulamamızı kullandığınızda bilgilerin nasıl işlendiğini açıklar. Gizliliğinizi korumaya ve veri uygulamalarımız konusunda şeffaf olmaya kararlıyız.

### Topladığımız Bilgiler

#### Konum Verileri
- **Ne topluyoruz:** Uygulama, APRS takip özelliklerini kullandığınızda cihazınızın GPS konumuna (enlem, boylam, yükseklik) erişir.
- **Nasıl kullanıyoruz:** Konum verileri yalnızca yapılandırdığınız ayarlara göre konumunuzu APRS-IS (APRS İnternet Servisi) sunucularına iletmek için kullanılır. Bu, amatör telsiz APRS takibinin temel işlevidir.
- **Depolama:** Konum verileri sunucularımızda SAKLANMAZ. Yalnızca cihazınızda geçici olarak işlenir ve seçtiğiniz üçüncü taraf APRS-IS sunucularına doğrudan iletilir.
- **Kontrol:** Konum verilerinin ne zaman paylaşılacağı konusunda tam kontrole sahipsiniz. Uygulama, yalnızca takibi açıkça başlattığınızda veya bir konum raporu gönderdiğinizde konuma erişir.

#### Kullanıcı Tarafından Sağlanan Bilgiler
- **Çağrı İşareti:** APRS hizmetlerini kullanmak için amatör telsiz çağrı işaretiniz gereklidir. Bu, cihazınızda yerel olarak saklanır.
- **APRS Yapılandırması:** Sunucu ayarları, güncelleme aralıkları, yorumlar ve sembol tercihleri cihazınızda yerel olarak saklanır.
- **Mesajlar:** Gönderdiğiniz ve aldığınız APRS mesajları yalnızca görüntüleme amacıyla cihazınızda geçici olarak saklanır.

#### Hava Durumu Verileri
- **Kaynak:** Etkinleştirildiğinde, uygulama mevcut konumunuza göre Open-Meteo API'den (ücretsiz, halka açık bir hava durumu servisi) hava durumu verilerini alır.
- **Kullanım:** Hava durumu verileri, APRS konum raporlarınızı meteorolojik bilgilerle zenginleştirmek için kullanılır.
- **Kişisel Veri Yok:** Hava durumu istekleri yalnızca coğrafi koordinatları içerir, kişisel tanımlayıcı içermez.

### TOPLAMADĞIMIZ Bilgiler

- ❌ Kendi sunucularımıza herhangi bir kişisel bilgi toplamıyor, saklamıyor veya iletmiyoruz
- ❌ Kullanım kalıplarınızı veya davranışlarınızı takip etmiyoruz
- ❌ Cihaz tanımlayıcıları (IMEI, MAC adresi, vb.) toplamıyoruz
- ❌ Kişilerinize, fotoğraflarınıza veya diğer kişisel dosyalarınıza erişmiyoruz
- ❌ Analitik veya takip hizmetleri kullanmıyoruz
- ❌ Reklam göstermiyoruz veya reklam ağları kullanmıyoruz
- ❌ Pazarlama amacıyla herhangi bir veriyi üçüncü taraflarla satmıyor, kiralamıyor veya paylaşmıyoruz

### Üçüncü Taraf Hizmetler

Uygulama, APRS işlevselliği için gerekli olan harici hizmetlere bağlanır:

#### APRS-IS Sunucuları
- **Amaç:** APRS paketlerini (konum raporları, mesajlar, durum güncellemeleri) iletmek ve almak
- **Paylaşılan Veriler:** Çağrı işaretiniz, konum koordinatları, yükseklik, yorumlar ve göndermeyi seçtiğiniz mesajlar
- **Gizlilik:** APRS-IS halka açık bir amatör telsiz ağıdır. APRS-IS'e iletilen tüm veriler diğer amatör telsiz operatörleri tarafından halka açık olarak erişilebilir hale gelir. Bu, APRS sisteminin amaçlanan tasarımıdır.
- **Kullanılan Sunucular:** Birden fazla APRS-IS sunucusu arasından seçim yapabilirsiniz (örn. rotate.aprs2.net, euro.aprs2.net, vb.)

#### Open-Meteo Hava Durumu API
- **Amaç:** Konumunuz için güncel hava durumu koşullarını almak
- **Paylaşılan Veriler:** Yalnızca coğrafi koordinatlar (enlem/boylam)
- **Gizlilik Politikası:** https://open-meteo.com/en/terms

#### APRS.fi Harita Servisi
- **Amaç:** APRS istasyonlarını ve etkinliği etkileşimli bir harita üzerinde görüntülemek
- **Paylaşılan Veriler:** Haritayı görüntülediğinizde, tarayıcınız aprs.fi'den içerik yükler
- **Gizlilik Politikası:** https://aprs.fi/page/privacy

### Veri Depolama ve Güvenlik

- **Yalnızca Yerel Depolama:** Tüm kullanıcı tercihleri, çağrı işaretleri ve mesaj geçmişi yalnızca cihazınızda Android'in SharedPreferences ve yerel bellek kullanılarak saklanır.
- **Bulut Yedekleme Yok:** Verilerinizi herhangi bir bulut hizmetine yedeklemiyoruz.
- **Veri Silme:** Uygulamayı kaldırmak, cihazınızdan yerel olarak saklanan tüm verileri kaldıracaktır.
- **İletim Güvenliği:** APRS-IS sunucularına bağlantılar standart TCP/IP protokollerini kullanır. APRS'nin tasarım gereği şifreli bir protokol olmadığını unutmayın.

### İzinler Açıklaması

Uygulama aşağıdaki Android izinlerini talep eder:

| İzin | Amaç | Gerekli |
|------|------|---------|
| `ACCESS_FINE_LOCATION` | APRS konum raporları için hassas GPS koordinatları almak | Evet |
| `ACCESS_COARSE_LOCATION` | Yaklaşık konum için yedek | Evet |
| `ACCESS_BACKGROUND_LOCATION` | Uygulama arka plandayken takibe devam etmek | İsteğe Bağlı* |
| `INTERNET` | APRS-IS sunucularına ve hava durumu API'sine bağlanmak | Evet |
| `FOREGROUND_SERVICE` | Uygulama simge durumuna küçültülürken takip servisini sürdürmek | Evet |
| `FOREGROUND_SERVICE_LOCATION` | Konum tabanlı ön plan servisi için gerekli | Evet |
| `POST_NOTIFICATIONS` | Gelen APRS mesajları hakkında sizi bilgilendirmek | İsteğe Bağlı |
| `WAKE_LOCK` | Aktif takip sırasında cihazı uyanık tutmak | Evet |

*Arka plan konumu yalnızca sürekli takip modunu başlattığınızda istenir.

### Çocukların Gizliliği

Bu uygulama lisanslı amatör telsiz operatörleri için tasarlanmıştır. 13 yaşın altındaki çocuklardan bilerek bilgi toplamıyoruz. 13 yaşın altındaysanız, lütfen bu uygulamayı ebeveyn gözetimi olmadan kullanmayın.

### Haklarınız ve Seçimleriniz

- **Konum Kontrolü:** Android ayarları üzerinden istediğiniz zaman konum erişimini etkinleştirebilir/devre dışı bırakabilirsiniz
- **Veri Silme:** Tüm yerel bilgileri kaldırmak için uygulama verilerini temizleyin veya uygulamayı kaldırın
- **Takip Kontrolü:** APRS takibini istediğiniz zaman başlatma/durdurma konusunda tam kontrole sahipsiniz
- **Mesaj Gizliliği:** Hangi mesajları göndereceğinizi siz kontrol edersiniz; alınan mesajlar manuel olarak temizlenebilir

### Bu Politikadaki Değişiklikler

Bu Gizlilik Politikasını zaman zaman güncelleyebiliriz. Herhangi bir değişiklik uygulama içinde ve GitHub depomuzda yayınlanacaktır. Değişikliklerden sonra uygulamayı kullanmaya devam etmek, güncellenmiş politikanın kabulü anlamına gelir.

### Açık Kaynak

Bu uygulama açık kaynaklıdır. Gizlilik uygulamalarımızı doğrulamak için kaynak kodun tamamını inceleyebilirsiniz: [GitHub Depo URL'si]

### İletişim Bilgileri

Bu Gizlilik Politikası hakkında sorularınız veya endişeleriniz için lütfen iletişime geçin:

- **Geliştirici:** Algsoft
- **E-posta:** info@algsoft.net.tr
- **Web Sitesi:** https://algsoft.net.tr
- **Proje Web Sitesi:** https://qrv73.com

### Yasal Uyumluluk

Bu uygulama şunlara uygundur:
- Google Play Store Veri Güvenliği gereksinimleri
- Android gizlilik en iyi uygulamaları
- APRS kullanımına ilişkin amatör telsiz düzenlemeleri

---

## Data Safety Declaration for Google Play Console

### Data Collection Summary

**Does your app collect or share any of the required user data types?**
- **NO** - This app does not collect or share any user data with third parties for advertising, analytics, or marketing purposes.

### Location Data Details

**Location (Approximate and Precise)**
- **Collected:** Yes
- **Shared:** Yes (with APRS-IS servers only)
- **Ephemeral:** Yes (not stored permanently)
- **Required:** Yes (core functionality)
- **Purpose:** App functionality (APRS position reporting)
- **User Control:** Users can start/stop sharing at any time

### Data Not Collected

The following data types are NOT collected:
- Personal information (name, email, address, phone, etc.)
- Financial information
- Health and fitness data
- Photos and videos
- Audio files
- Files and documents
- Calendar events
- Contacts
- App activity
- Web browsing history
- App info and performance
- Device or other identifiers

### Security Practices

- Data is encrypted in transit using standard protocols
- Users can request data deletion by uninstalling the app
- No data is stored on developer servers
- Open source - code is publicly auditable

---

## Google Play Console Veri Güvenliği Beyanı

### Veri Toplama Özeti

**Uygulamanız gerekli kullanıcı veri türlerinden herhangi birini topluyor veya paylaşıyor mu?**
- **HAYIR** - Bu uygulama, reklam, analitik veya pazarlama amacıyla üçüncü taraflarla herhangi bir kullanıcı verisi toplamaz veya paylaşmaz.

### Konum Verisi Detayları

**Konum (Yaklaşık ve Hassas)**
- **Toplanan:** Evet
- **Paylaşılan:** Evet (yalnızca APRS-IS sunucularıyla)
- **Geçici:** Evet (kalıcı olarak saklanmaz)
- **Gerekli:** Evet (temel işlevsellik)
- **Amaç:** Uygulama işlevselliği (APRS konum raporlama)
- **Kullanıcı Kontrolü:** Kullanıcılar istediği zaman paylaşımı başlatabilir/durdurabilir

### Toplanmayan Veriler

Aşağıdaki veri türleri toplanmaz:
- Kişisel bilgiler (ad, e-posta, adres, telefon, vb.)
- Finansal bilgiler
- Sağlık ve fitness verileri
- Fotoğraflar ve videolar
- Ses dosyaları
- Dosyalar ve belgeler
- Takvim etkinlikleri
- Kişiler
- Uygulama etkinliği
- Web tarama geçmişi
- Uygulama bilgisi ve performansı
- Cihaz veya diğer tanımlayıcılar

### Güvenlik Uygulamaları

- Veriler standart protokoller kullanılarak aktarım sırasında şifrelenir
- Kullanıcılar uygulamayı kaldırarak veri silme talebinde bulunabilir
- Geliştirici sunucularında veri saklanmaz
- Açık kaynak - kod herkese açık olarak denetlenebilir

---

**Version / Versiyon:** 1.0  
**Effective Date / Yürürlük Tarihi:** January 2025  
**App Package Name / Uygulama Paket Adı:** com.qrv73.aprsgonder
