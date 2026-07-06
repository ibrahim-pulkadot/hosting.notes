# 🏗️ Altyapı Kurulumu

## 📍 Lokasyon / Datacenter

Sunucularımız **Kuzey Data Center**'da barındırılıyordu — **Tier III** bir tesis. Datacenter'ın kendisiyle hiçbir sorunumuz olmadı, yaşadığımız sıkıntılar tamamen üçüncü şahıs olan aracı hosting firmasıyla ilgiliydi (bu firmayı isim olarak vermek istemiyorum, [şirket açılışı](../01-sirket-acilisi/README.md) bölümünde de bahsettiğim gibi).

Fiziksel sunucuları rack olarak bu üçüncü şahıs hosting firmasından kiraladık.

## 🌐 Network

Kendi adımıza bir **IP class** anons ettirmiştik — toplamda **256 IP adresi** (254'ü kullanılabilir).

## 🛡️ DDoS Koruması

DDoS koruması **Juniper MX480** cihazı üzerinden sağlanıyordu, buna ek olarak **Mikrotik + firewall** kombinasyonuyla toplamda **8+ Tbps** DDoS koruma kapasitemiz vardı.

## 🔑 Erişim & Sanallaştırma

Sunuculara **KVM** üzerinden erişiyorduk. **ESXi** kurulumunu kendimiz yaptık, kurulum sırasında herhangi bir sorun yaşamadık.

## 📈 Ölçekleme: 1'den 5 Sunucuya

1 sunucudan 5 sunucuya çıkış sürecinde beklenmedik bir sorunla karşılaştık: müşteriler hizmet almayı bıraksa bile bazı yazılım sorunları yüzünden cihazlar (VDS'ler) düzgün silinmiyordu, bu da sunucularda RAM'in dolu görünmesine yol açıyordu. Bu görünüşteki doluluk yüzünden yeni makineler aldık — üstelik o dönem çok fazla sponsorluğumuz vardı ve talep gerçekten yüksekti.

Daha sonra sponsorluk anlaşmalarının çoğunu feshedince cihazlarda biraz boşluk oluştu, ama iş işten geçmişti — zaten gereğinden fazla donanım almıştık 😞

## ✅ Arıza Durumu

Bütün bu süreç boyunca hiçbir donanım arızası yaşamadık.

## 👀 İzleme

Sunucu ve servis takibi için **Uptime Kuma** kullandık.
