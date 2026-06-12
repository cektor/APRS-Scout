# Privacy Policy / Gizlilik Politikası

**APRS Tracker Pro** — iOS, iPadOS, macOS & watchOS

**Developer / Geliştirici:** Fatih ÖNDER (TB1TFO) — ALGSoft Inc.
**Contact / İletişim:** info@algsoft.net.tr — https://algsoft.net.tr
**Last updated / Son güncelleme:** June 12, 2026 / 12 Haziran 2026

---

## English

### 1. Overview

APRS Tracker Pro is an amateur (ham) radio application that transmits your position, optional weather data, and short text messages to the **APRS-IS (Automatic Packet Reporting System – Internet Service)** network. It is intended for licensed amateur radio operators.

**We do not collect, store, or sell any personal data on our own servers. We operate no servers, no analytics, no advertising, and no tracking of any kind.** All data described below either stays on your device or is transmitted — only at your explicit request — to the public APRS-IS amateur radio network.

### 2. Important: APRS-IS is a public network

When you press **Send Location**, **Start Tracking**, or send an APRS message, the following information is broadcast to the worldwide, public APRS-IS network:

- Your amateur radio callsign (which you enter yourself)
- Your GPS position (latitude, longitude, altitude), course and speed
- Your optional comment text and selected map symbol
- Optional local weather readings (temperature, humidity, pressure, wind)
- The text of APRS messages you send, including the recipient callsign

APRS-IS data is **publicly visible and permanently archived by independent third-party services** (for example aprs.fi, aprsdirect.com and others). The developer has no control over these archives and **cannot delete data once transmitted**. Do not use this app if you do not want your position to be public. Nothing is ever transmitted automatically — transmission only happens when you start it.

### 3. Permissions the app requests and why

| Permission | Platform | Why it is needed |
|---|---|---|
| **Location — While Using the App** | iOS, macOS, watchOS | To read your GPS coordinates and build APRS position packets, show your Maidenhead grid square, and compute distances to received stations. |
| **Location — Always (background)** | iOS, watchOS | Only needed if you enable continuous tracking, so position beacons can continue at your chosen interval while the app is in the background. iOS shows a visible indicator while this is active. You can use one-shot sending with "While Using" permission only. |
| **Notifications (local)** | iOS | To alert you when an incoming APRS message addressed to your callsign arrives. These are local notifications; no push notification servers are used. |

The app does **not** request access to your camera, microphone, contacts, photos, health data, or any other sensitive data. Dictation on Apple Watch uses the system keyboard/dictation service provided by Apple; the app only receives the final text you accept.

### 4. Data stored on your device

The following settings are stored locally (UserDefaults) and never leave your device except as part of APRS packets you choose to transmit:

- Callsign, APRS passcode (computed locally from your callsign)
- Selected APRS-IS server, port, beacon interval, APRS symbol, comment text
- Optional fixed/static coordinates, weather toggle state
- Message history (kept only in memory during the session)

If you use both iPhone and Apple Watch, these settings are synchronized between your own devices via Apple's WatchConnectivity framework. This sync is device-to-device and does not pass through any developer server.

### 5. Network connections made by the app

| Destination | Purpose | Data sent |
|---|---|---|
| APRS-IS servers (e.g. `euro.aprs2.net`, port 14580) — operated by the amateur radio community | Transmitting your beacons/messages; receiving nearby station activity and messages addressed to you | Callsign, passcode, position packets, messages — only when you initiate |
| Open-Meteo API (`api.open-meteo.com`) | Fetching current weather for your position when the weather option is enabled | Your approximate coordinates (no identifiers, no API key, no account) — see https://open-meteo.com/en/terms |
| Apple App Store (StoreKit) | On-device verification that the app was obtained from the App Store (release builds only) | Handled entirely by Apple's StoreKit framework; no data goes to the developer |

### 6. What we do NOT do

- ❌ No analytics or telemetry SDKs
- ❌ No advertising, no ad identifiers (IDFA)
- ❌ No user accounts, no registration
- ❌ No developer-operated servers storing your data
- ❌ No selling, sharing, or monetizing of personal data
- ❌ No tracking across apps or websites (App Tracking Transparency is not applicable because no tracking occurs)

### 7. Data retention and deletion

The developer retains nothing, so there is nothing for us to delete. Locally stored settings are removed when you delete the app. Data already broadcast to APRS-IS is archived by independent third parties under their own policies and cannot be recalled — this is an inherent property of the amateur radio APRS network that every licensed operator should understand.

### 8. Children's privacy

This app is intended for licensed amateur radio operators and is not directed at children under 13. We do not knowingly collect any data from children; in fact, we collect no data at all.

### 9. Your rights (GDPR / KVKK / CCPA)

Since the developer processes no personal data on any server, there is no developer-held data to access, correct, or erase. For data already on the public APRS-IS network, archival services (e.g. aprs.fi) have their own data controllers and removal procedures. For any privacy question, contact us at the e-mail address above and we will respond as soon as possible.

### 10. Changes to this policy

Updates to this policy will be published at this URL with a new "Last updated" date. Material changes will be noted in the App Store release notes.

---

## Türkçe

### 1. Genel Bakış

APRS Tracker Pro; konumunuzu, isteğe bağlı hava durumu verilerini ve kısa metin mesajlarını **APRS-IS (Automatic Packet Reporting System – Internet Service)** ağına ileten bir amatör telsiz uygulamasıdır. Lisanslı amatör telsiz operatörleri için tasarlanmıştır.

**Hiçbir kişisel verinizi kendi sunucularımızda toplamıyor, saklamıyor ve satmıyoruz. Sunucumuz, analitik aracımız, reklamımız ve hiçbir türde izleme sistemimiz yoktur.** Aşağıda açıklanan tüm veriler ya cihazınızda kalır ya da yalnızca sizin açık isteğinizle herkese açık APRS-IS amatör telsiz ağına iletilir.

### 2. Önemli: APRS-IS herkese açık bir ağdır

**Konum Gönder**, **Takibi Başlat** veya mesaj gönder dediğinizde şu bilgiler dünya çapındaki herkese açık APRS-IS ağına yayınlanır:

- Çağrı işaretiniz (kendi girdiğiniz)
- GPS konumunuz (enlem, boylam, irtifa), yön ve hız
- İsteğe bağlı yorum metniniz ve seçtiğiniz harita sembolü
- İsteğe bağlı yerel hava durumu değerleri (sıcaklık, nem, basınç, rüzgar)
- Gönderdiğiniz APRS mesajlarının içeriği ve alıcı çağrı işareti

APRS-IS verileri **herkes tarafından görülebilir ve bağımsız üçüncü taraf hizmetlerce (örn. aprs.fi) kalıcı olarak arşivlenir.** Geliştiricinin bu arşivler üzerinde denetimi yoktur ve **bir kez iletilen veri silinemez.** Konumunuzun herkese açık olmasını istemiyorsanız bu uygulamayı kullanmayın. Hiçbir veri otomatik gönderilmez — iletim yalnızca siz başlattığınızda gerçekleşir.

### 3. İstenen izinler ve nedenleri

| İzin | Platform | Neden gerekli |
|---|---|---|
| **Konum — Uygulamayı Kullanırken** | iOS, macOS, watchOS | GPS koordinatlarınızı okuyup APRS konum paketleri oluşturmak, Maidenhead grid karenizi göstermek ve alınan istasyonlara uzaklık hesaplamak için. |
| **Konum — Her Zaman (arka plan)** | iOS, watchOS | Yalnızca sürekli takibi etkinleştirirseniz gerekir; uygulama arka plandayken seçtiğiniz aralıkta konum vericisinin sürmesi içindir. Bu etkinken iOS görünür bir gösterge sunar. Tek seferlik gönderim için "Kullanırken" izni yeterlidir. |
| **Bildirimler (yerel)** | iOS | Çağrı işaretinize gelen APRS mesajlarında sizi uyarmak için. Bunlar yerel bildirimdir; push (anlık bildirim) sunucusu kullanılmaz. |

Uygulama kameranıza, mikrofonunuza, kişilerinize, fotoğraflarınıza, sağlık verilerinize veya başka hiçbir hassas veriye erişim istemez. Apple Watch'taki dikte, Apple'ın sistem dikte hizmetini kullanır; uygulamaya yalnızca onayladığınız nihai metin iletilir.

### 4. Cihazınızda saklanan veriler

Şu ayarlar yerel olarak (UserDefaults) saklanır ve iletmeyi seçtiğiniz APRS paketleri dışında cihazınızdan asla çıkmaz:

- Çağrı işareti, APRS passcode (çağrı işaretinizden cihazda hesaplanır)
- Seçili APRS-IS sunucusu, port, gönderim aralığı, APRS sembolü, yorum metni
- İsteğe bağlı sabit konum koordinatları, hava durumu seçeneği
- Mesaj geçmişi (yalnızca oturum süresince bellekte tutulur)

iPhone ve Apple Watch'u birlikte kullanıyorsanız bu ayarlar Apple'ın WatchConnectivity çerçevesiyle yalnızca kendi cihazlarınız arasında eşitlenir; hiçbir geliştirici sunucusundan geçmez.

### 5. Uygulamanın kurduğu ağ bağlantıları

| Hedef | Amaç | Gönderilen veri |
|---|---|---|
| APRS-IS sunucuları (örn. `euro.aprs2.net`, port 14580) — amatör telsiz topluluğunca işletilir | Verici/mesaj iletimi; çevredeki istasyon etkinliğinin ve size gelen mesajların alınması | Çağrı işareti, passcode, konum paketleri, mesajlar — yalnızca siz başlattığınızda |
| Open-Meteo API (`api.open-meteo.com`) | Hava durumu seçeneği açıkken konumunuzun güncel hava verisini almak | Yaklaşık koordinatlarınız (kimlik bilgisi, API anahtarı, hesap yok) — bkz. https://open-meteo.com/en/terms |
| Apple App Store (StoreKit) | Uygulamanın App Store'dan edinildiğinin cihaz üzerinde doğrulanması (yalnızca yayın sürümleri) | Tamamen Apple StoreKit çerçevesince yürütülür; geliştiriciye veri gitmez |

### 6. Yapmadıklarımız

- ❌ Analitik veya telemetri SDK'sı yok
- ❌ Reklam ve reklam tanımlayıcısı (IDFA) yok
- ❌ Kullanıcı hesabı, kayıt yok
- ❌ Verinizi saklayan geliştirici sunucusu yok
- ❌ Kişisel veri satışı, paylaşımı, ticarileştirmesi yok
- ❌ Uygulamalar/web siteleri arası izleme yok (izleme olmadığından App Tracking Transparency kapsamı dışındadır)

### 7. Veri saklama ve silme

Geliştirici hiçbir veri tutmadığından silinecek bir veri de yoktur. Yerel ayarlar uygulamayı sildiğinizde kaldırılır. APRS-IS'e yayınlanmış veriler bağımsız üçüncü taraflarca kendi politikaları uyarınca arşivlenir ve geri çağrılamaz — bu, her lisanslı operatörün bildiği üzere APRS ağının doğasında vardır.

### 8. Çocukların gizliliği

Bu uygulama lisanslı amatör telsiz operatörlerine yöneliktir; 13 yaş altı çocuklara yönelik değildir. Çocuklardan bilerek veri toplamayız; esasen hiç veri toplamayız.

### 9. Haklarınız (KVKK / GDPR / CCPA)

Geliştirici hiçbir sunucuda kişisel veri işlemediğinden erişilecek, düzeltilecek veya silinecek geliştirici elindeki bir veri yoktur. Herkese açık APRS-IS ağındaki veriler için arşiv hizmetlerinin (örn. aprs.fi) kendi veri sorumluları ve kaldırma süreçleri vardır. Gizlilikle ilgili her soru için yukarıdaki e-posta adresinden bize ulaşabilirsiniz; en kısa sürede yanıtlarız.

### 10. Politika değişiklikleri

Bu politikadaki güncellemeler yeni "Son güncelleme" tarihiyle bu adreste yayımlanır. Önemli değişiklikler App Store sürüm notlarında belirtilir.
