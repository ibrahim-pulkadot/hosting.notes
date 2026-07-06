# 🧩 Panel ve Operasyon

## 🖥️ Panel Seçimi

**WiseCP**'yi Türk bir ürün olması ve uygun fiyatı yüzünden tercih ettik. Normalde **WHMCS** alırdık ama bizim için çok pahalıydı.

WiseCP kullanmak kolay olmadı:

- Sistem sürekli donuyor/kasıyordu.
- **PayTR** entegrasyonu sürekli bozuktu.
- **İyzico** sanal POS'ta sürekli hatalar alıyorduk.
- Neredeyse her hafta sistemde yeni bir açık buluyorduk. Biz raporlamaktan bıktık, onlar düzeltmekten bıkmadı 😅

## 🔧 Kendi Panelimiz

Bu sorunlar yüzünden WHMCS API'si ile kendi panelimizi (Next.js tabanlı) yazdık. Geliştirirken tek zorlandığımız kısım fiziksel cihazlara (ESXi sunucularına) bağlanma tarafıydı, onun dışında ciddi bir sorun yaşamadık.

## 🛒 Sipariş & Provisioning Akışı

Müşteri tarafındaki akış şöyleydi:

1. Hesap oluştur — TC kimlik no, isim-soyisim, telefon, adres gibi bilgiler girilir.
2. Satın alım yapılır.
3. Hizmet otomatik kurulur ve teslim edilir.

## 🎫 Destek Sistemleri

Destek talepleri aynı anda 4 farklı kanaldan yönetiliyordu:

- Kendi yazılımımız (panel içi destek)
- WiseCP
- WhatsApp
- Discord ticket sistemi

## 💳 Faturalama & Yenileme

Abonelik yenilemeleri otomatikti, ek olarak hatırlatma ve uyarı sistemleri de vardı. Ödeme **3 gün** geciktiğinde sunucu otomatik olarak siliniyordu — silme işlemi tamamen otomatikti.

## 🔐 Güvenlik & Yedekleme

- Her gün sabah **06:00**'da tüm sunucuların yedeği alınıyordu.
- Panel güvenliği için **2FA**, **rate limit**, giriş logları ve IP adresi tespiti kullanıyorduk.
- Ekstra bir önlem olarak: yönetici cihazlarının anakart bilgilerini detaylıca kaydedip şifreliyorduk. Panel, bu donanım bilgisi birebir eşleşmediği sürece erişime izin vermiyordu — yani panele sadece belirli, kayıtlı cihazlardan girilebiliyordu.
