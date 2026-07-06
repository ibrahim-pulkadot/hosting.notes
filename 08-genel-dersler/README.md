# 🎓 Genel Dersler ve Tavsiyeler

Bu, serinin son bölümü. Yedi bölüm boyunca anlattığım her şeyden sonra, bu işe girmeyi düşünen birine söyleyeceklerim:

## ⚠️ Göze Almanız Gerekenler

- **Güçlü ve güvenilir bir destek ekibiniz yoksa**, dışarıdayken bile rahatsız edilebilirsiniz. Bu işle 7/24 ilgilenmeniz gerekiyor.
- **Paranız yoksa bu işe girmeyin.** Bu, sermayesi olmadan girilebilecek bir iş değil.
- Kazanmak istiyorsanız **kurumsal müşterilere** satış yapmalısınız. Sadece oyun sunucusu müşterileriyle uğraşırsanız, parayı uzun vadede kazanırsınız.
- Bu işi oturtmak yaklaşık **1 yıl** sürer. 1 yıl sonra net kâra geçersiniz.

## 💼 İki Farklı Yaklaşım

**Az sermayeyle (kendiniz yönetecekseniz):** Bu iş, "param olsun, bana gelir getirsin" diye düşünenler için de uygun bir iş modeli — ama bunun için parası olan birinin bu işe girmesi gerekiyor.

**Çok sermayeyle (birine yönettirecekseniz):** Fiziksel sunucu satın alıp işin başına bu işi bilen birini koyabilirsiniz, o kişi her şeyi detaylıca yönetir. (Bizim de bu konuda sunduğumuz bir hizmetimiz var, [hizmetlerimiz.md](../hizmetlerimiz.md) dosyasına bakabilirsiniz.)

Başlangıçta bir yazılımcıyla çalışmak mantıksız olabilir — **VMware ESXi 8 + DiyoVM + WiseCP** entegrasyonu başlangıç için yeterli ve iyidir.

## 💸 Örnek Bütçe Dağılımı: 50.000₺

Bu işe 50.000₺ ile başlayacak olsam:

- **25.000₺** → iyi bir donanım/cihaz
- **Kalan tutar** → pazarlama
- **1.000-2.000₺** → ekip

## 💰 Örnek Bütçe Dağılımı: 1.000.000₺ (Yönetilen Senaryo)

Biri bana 1 milyon TL verip bu işi yönetmemi istese:

1. **500.000₺** → çok kaliteli 5 fiziksel sunucu (toplamda ~1.5 TB RAM)
2. Her ay sabit **15.000₺** → pazarlama ekibine (fiyatlandırma toplantıları + Instagram yönetimi). İlk 3 ay toplam **45.000₺**. 3 aydan sonra pazarlama ekibiyle çalışmayı bırakıp reklamları kendimiz yönetiriz — çünkü marka 3 ayda tanınır hale gelmiş olur.
3. Kalan **~455.000₺**'den lisanslara ve veri merkeziyle anlaşmaya ödeme yapılır, elde **~440.000₺** kalır.
4. İlk 3 ayı atlattıktan sonra bu parayla yeni donanım alıp bütçeyi tekrar 500.000₺'ye tamamlarız → **5 sunucu daha** eklenir.

Sonuç: **10 fiziksel sunucu**, toplamda **3 TB (3.072 GB) RAM** kapasitesi.

### Örnek Gelir Tablosu (3.072 GB kapasiteyle, teorik maksimum doluluk)

| Paket | Fiyat (+KDV) | Maksimum Paket Sayısı | Aylık Potansiyel Gelir |
|---|---|---|---|
| 2 GB RAM | 200₺ | 1.536 | 307.200₺ |
| 8 GB RAM | 330₺ | 384 | 126.720₺ |

*(Kurumsal müşterilere satılmadığı, sadece bireysel paket satışı yapıldığı varsayılmıştır. Gerçek doluluk oranı bu rakamların altında kalır.)*

### Kurumsal Satış Senaryosu (SLA Seviye 3)

Aynı 10 sunucu / 3.072 GB kapasiteyi bu sefer **kurumsal müşterilere, SLA Seviye 3** garantisiyle sattığımızı varsayalım. SLA Seviye 3 — yüksek uptime garantisi, öncelikli destek ve ihlal durumunda tazminat maddeleri içerir — bu yüzden bireysel paket fiyatının üzerine **~%60 kurumsal/SLA primi** ekledim:

| Paket | Bireysel Fiyat | Kurumsal SLA-3 Fiyatı (+KDV) | Maksimum Paket Sayısı | Aylık Potansiyel Gelir |
|---|---|---|---|---|
| 6 GB RAM | ~250₺ | **400₺** | 512 | 204.800₺ |
| 8 GB RAM | 330₺ | **530₺** | 384 | 203.520₺ |

*(Bu tablodaki %60 prim oranı örnek bir varsayımdır — gerçek kurumsal fiyatlandırmanız farklıysa bana gerçek rakamı ver, tabloyu ona göre güncelleyeyim. Burada da teorik maksimum doluluk varsayılmıştır, kurumsal satışta gerçek doluluk oranı genelde bireysele göre daha düşük ama müşteri başına daha istikrarlı olur.)*

## 🎯 Son Söz

> "Risk almadan hiçbir şekilde başarılı iş yapamazsın."

Hosting sektörüne yeniden girecek olsam, **kendi yazılımımla, kendi donanımımla** girerdim ve **pazarlamayı asla küçümsemez**, ona da yeterli bütçe ayırırdım.
