TeamPCP — Temel Bulgular

Flare araştırmacıları tarafından ilk kez Aralık 2025'te belgelenen TeamPCP, unauthenticated cloud control plane'leri exploit ederek standardize payload'lar dağıtan, cloud-native bir siber suç platformu olarak tanımlanmaktadır.

Kampanyanın özeti: 

TeamPCP, güvenlik açığı tarayıcısı Trivy ve ilgili GitHub Actions'ı compromise ettikten sonra Checkmarx araçlarına, KICS GitHub Action'ına ve OpenVSX extension'larına yayıldı. Tüm bu vakalarda credential çalımı üzerinden kompromi gerçekleşti. 

Neden benzersizdir: 

Kampanya üç temel özelliğiyle öne çıkıyor: self-propagating worm kabiliyeti, blockchain tabanlı C2 (ICP canister'ı C2 olarak kullanan ilk belgelenmiş tehdit aktörü) ve güvenlik araçlarının saldırı yüzeyi olarak kullanılması en titiz organizasyonlar en yüksek riske maruz kaldı.

Detection yaklaşımı: Static analiz ve dependency scanning başarısız oldu; runtime detection başarılı oldu. 
Saldırgan, nihayetinde credential çalmak ve exfil yapmak için sistem çağrıları kullanmak zorundadır  bu çağrılar, saldırganın koda nasıl eriştiğinden bağımsız olarak gözlemlenebilir.

Makalede şunlar bulunuyor:

# Tam operasyonel kronoloji (Temmuz 2025 → Mart 2026)
# 9 adımlı cascade kill chain diyagramı
# 13 MITRE ATT&CK tekniği mapping
# Falco, Splunk SPL ve Wazuh detection rule'ları
# Aktif IOC listesi (C2 IP, malicious paket versiyonları)
# 10 madde önleyici kontrol önerisi

