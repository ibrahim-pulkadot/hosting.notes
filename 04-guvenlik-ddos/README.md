# 🛡️ Güvenlik ve DDoS

## 💥 Saldırı Deneyimleri

Karşılaştığımız en büyük saldırı hem **L7** hem **volumetrik** tarzda, yaklaşık **4.5 Tbps** boyutundaydı. Buna rağmen hiçbir şey olmadı — hizmetlerimizde herhangi bir aksama yaşanmadı.

Saldırıların kaynağı genelde ya **rakip firmalar** ya da **kişisel husumetlerden** kaynaklanıyordu.

## 🔒 Koruma Önlemleri

[Altyapı](../02-altyapi-kurulumu/README.md) bölümünde bahsettiğim Juniper MX480 + Mikrotik ile sağlanan 8+ Tbps'lik DDoS korumasına ek olarak:

- **WAF** (Web Application Firewall)
- **Rate limiting**

katmanları da vardı. Bu sayede hiçbir saldırı sırasında hizmetlerimizde aksama yaşamadık.

## 🕵️ Sızma / İhlal Durumu

Faaliyetimiz boyunca hiçbir şekilde bir sızma ya da güvenlik ihlali yaşanmadı.

## 🔐 Müşteri Verilerinin Güvenliği

Müşteri verileri (fatura sistemi için gerekli TC no, isim, adres vb.) bize normalde şifrelenmeden geliyordu. Biz bu veriyi kendi sistemimizde/donanımımızda **şifreleme** ve ek olarak **hashleme + salt round** ile koruma altına alıyorduk.

## 👷 Ekip & Müdahale Süreci

Bir saldırı ya da güvenlik olayında ilk müdahaleyi kendimiz yapıyorduk. Eğer konu bizim bilgimizin yetersiz kaldığı bir noktaya gelirse, bir **networkçü** ile görüşüp destek alıyorduk.
