# QR Menü ve Adisyon Programı Seçim Rehberi

Restoran, kafe, bar, pastane ve fast-food işletmeleri için **QR menü** ve **adisyon programı
(restoran POS sistemi)** seçerken bakılması gereken başlıkların sade bir dökümü. Amaç, teklif
almadan önce "ne soracağımı biliyorum" noktasına gelmek.

> **Uyarı:** Bu belge bilgilendirme amaçlıdır, hukuki veya mali tavsiye değildir. Mevzuat
> değişir, tutarlar her yıl güncellenir. Yasal yükümlülükleri uygulamadan önce resmî
> kaynaktan (aşağıdaki Kaynaklar bölümü) teyit edin.

---

## İçindekiler

1. [Terimler sözlüğü](#1-terimler-sözlüğü)
2. [QR menü nedir, ne değildir](#2-qr-menü-nedir-ne-değildir)
3. [Adisyon programı / restoran POS: modül haritası](#3-adisyon-programı--restoran-pos-modül-haritası)
4. [Bulut ile yerel kurulum farkı](#4-bulut-ile-yerel-kurulum-farkı)
5. [Yazarkasa (ÖKC) ve mali mevzuat](#5-yazarkasa-ökc-ve-mali-mevzuat)
6. [Menüde bulunması gereken bilgiler](#6-menüde-bulunması-gereken-bilgiler)
7. [Fiyat modelleri ve gizli maliyetler](#7-fiyat-modelleri-ve-gizli-maliyetler)
8. [İşletme tipine göre öncelikler](#8-i̇şletme-tipine-göre-öncelikler)
9. [Değerlendirme kontrol listesi (22 madde)](#9-değerlendirme-kontrol-listesi-22-madde)
10. [Kurulum ve geçiş planı](#10-kurulum-ve-geçiş-planı)
11. [Sık yapılan hatalar](#11-sık-yapılan-hatalar)
12. [Kaynaklar](#kaynaklar)

---

## 1. Terimler sözlüğü

| Terim | Anlamı |
|---|---|
| **Adisyon** | Bir masaya ait açık hesap. Sipariş eklendikçe büyür, ödeme alınınca kapanır. |
| **Adisyon programı** | Masa, sipariş, mutfak, kasa ve raporlamayı yöneten yazılım. Türkiye'de yerleşmiş ad. |
| **POS** | Point of Sale — satış noktası. "Restoran POS sistemi" adisyon programının uluslararası karşılığıdır. |
| **KDS** | Kitchen Display System — mutfak ekranı. Kâğıt fişin yerini alan, siparişin anlık düştüğü ekran. |
| **QR menü / karekod menü** | Masadaki kodun okutulmasıyla telefonda açılan dijital menü. |
| **ÖKC** | Ödeme Kaydedici Cihaz — yazarkasa. "Yeni nesil ÖKC" mali belgeyi elektronik üreten cihaz sınıfıdır. |
| **Reçete** | Bir ürünün hangi malzemeden ne kadar içerdiğinin tanımı. Maliyet ve otomatik stok düşümünün temeli. |
| **Fire / zayiat** | Bozulma, dökülme, iade gibi nedenlerle satılamadan eksilen stok. |
| **Cari / veresiye** | Müşteri adına açılan hesap; borç ve tahsilat hareketleriyle takip edilir. |
| **Kat planı** | Salon, teras, bahçe gibi alanların ve masaların ekrandaki yerleşimi. |
| **Terminal** | Sipariş girilen her cihaz (kasa, tablet, el terminali). Bazı fiyatlandırmalar buna göre yapılır. |

---

## 2. QR menü nedir, ne değildir

QR menü, misafirin masadaki karekodu telefon kamerasıyla okutarak açtığı dijital menüdür.
Uygulama indirme şartı koyan bir çözüm, okutma oranını ciddi biçimde düşürür — menü tarayıcıda
açılmalıdır.

**İki farklı şeye aynı ad veriliyor. Fark önemli:**

| Konu | Menüyü PDF/görsele bağlayan QR kod | QR menü yazılımı |
|---|---|---|
| Mobil okunabilirlik | Yakınlaştırma ve kaydırma gerekir | Telefon ekranına göre tasarlanmış |
| Güncelleme | Yeni dosya hazırlanır | Panelden anında |
| Alerjen / kalori alanları | Sayfaya sığdırmak zordur | Ürün kartında ayrı alan |
| Çoklu dil | Her dil için ayrı dosya ve kod | Tek kod, misafir dili seçer |
| Sipariş | Yok | Menüden sipariş gönderilebilir |
| Ölçüm | Yok | Görüntülenme ve ürün ilgisi izlenebilir |
| Maliyet | Ücretsiz | Abonelik |

**Kritik teknik kural:** QR kod, **kalıcı bir sayfa adresine** bağlanmalı; içerik o sayfanın
arkasında değişmelidir. Kod doğrudan bir dosya adresine bağlanırsa, dosya değiştiğinde ya da
taşındığında masadaki tüm kodlar ölür ve yeniden basım gerekir.

**Baskı ayrıntıları:** kod en az 2,5–3 cm, mat yüzeye basılmalı, misafirin oturduğu taraftan
okunabilecek konumda olmalı ve yanında tek satırlık yönlendirme bulunmalıdır.

---

## 3. Adisyon programı / restoran POS: modül haritası

Bir adisyon programını değerlendirirken özellik listesinin uzunluğuna değil, tek bir siparişin
uçtan uca kaç adımda tamamlandığına bakın. Aşağıdaki başlıklar sektörde standart kabul edilen
modül grupları — hangi ürünü alırsanız alın, teklifte bunların hangilerinin dahil olduğunu
sorun.

**Masa ve salon**
- Alan/kat ayrımı, masa durumları (boş, açık, hesap istendi, rezerve, temizlikte)
- Rezervasyon, kişi sayısı
- Masa birleştirme, masadan masaya sipariş taşıma

**Sipariş**
- Sipariş tipleri: masada servis, gel-al, paket (kurye)
- Ürün seçenekleri (boy, malzeme, ekstra), ürün notu
- Kalem iptali, ikram, sipariş ve kalem bazlı indirim

**Mutfak**
- Mutfak ekranı (KDS) veya mutfak yazıcısı
- Kalem durum akışı ve hazırlık süresi takibi
- İstasyon ayrımı (ızgara, bar, tatlı ayrı ekranlara düşüyor mu?)

**Kasa ve ödeme**
- Vardiya açma/kapama, kasa hareketleri, gün sonu
- Nakit, kart, online ve veresiye tahsilat; bahşiş
- Hesap bölme ve karma ödeme desteği

**Stok, reçete, maliyet**
- Malzeme kartları, reçete, satışta otomatik stok düşümü
- Alım/tedarikçi kaydı, fire, kritik stok uyarısı
- Ürün maliyeti ve kâr marjı, gider dağıtımı

**Personel**
- Rol ve yetki matrisi (kim indirim yapabilir, kim iptal edebilir?)
- Garson bazlı satış ve bahşiş, avans, izin, bordro kaydı

**Raporlar**
- Gün özeti, günlük satış, en çok satan ürünler, kategori satışları
- Saatlik yoğunluk (personel planlamasının temel girdisi)
- Masa performansı, iptal/iade, finansal özet, kâr/zarar

**Çok şubeli işletmeler**
- Merkezi ürün ve fiyat yönetimi
- Şube bazlı ve toplam raporlama

---

## 4. Bulut ile yerel kurulum farkı

| Konu | Yerel kurulum | Bulut tabanlı |
|---|---|---|
| Yazılımın yeri | İşletmedeki bilgisayar | Sağlayıcının sunucusu |
| İnternet kesintisi | Yerel ağ çalışırsa devam eder | Bağlantı gerekir |
| Donanım arızası | Veri kaybı riski işletmede | Veri sunucuda |
| Yedekleme | İşletmenin sorumluluğu | Sağlayıcının sorumluluğu |
| Güncelleme | Genelde yıllık bakım bedeliyle | Abonelik kapsamında |
| Uzaktan erişim | Ek kurulum gerekir | Tarayıcıdan |
| İlk maliyet | Yüksek (lisans + sunucu) | Düşük |
| Uzun vade | Bakım bedeli sürer | Abonelik sürer |

Bulut tabanlı bir sistem seçtiyseniz **ikinci bir internet hattı** (ör. mobil veri yedeği)
kasa donanımı kadar temel bir gerekliliktir. Yerel sistem seçtiyseniz **yedekleme prosedürünüzü
yazılı hâle getirin** ve düzenli test edin — yedeğin çalıştığı ancak geri yüklenirken anlaşılır.

---

## 5. Yazarkasa (ÖKC) ve mali mevzuat

Yeme-içme işletmelerinde satışın belgelenmesi ödeme kaydedici cihaz mevzuatına tabidir.
Yeni nesil ÖKC kullanımı ve bu cihazların satış/adisyon yazılımlarıyla birlikte çalışması
düzenlemeye bağlanmıştır; yükümlülüğe uymayan işletmeler için özel usulsüzlük cezaları
öngörülür. Ceza tutarları ve kapsam her yıl güncellendiği için **güncel durumu Gelir İdaresi
Başkanlığı kaynağından teyit edin.**

Yazılım seçerken bu başlıkta sorulacak sorular:

1. Yazılım hangi ÖKC marka/modelleriyle çalışıyor, listesi var mı?
2. Entegrasyon ek ücretli mi, tek seferlik mi, yıllık mı?
3. Adisyon kapandığında mali belge süreci nasıl işliyor?
4. Cihazı zaten varsa mevcut cihazla çalışıyor mu, yenisini almak gerekiyor mu?
5. Entegrasyon yoksa süreç nasıl yürüyecek ve bu sizin için kabul edilebilir mi?

**Not:** Her adisyon yazılımı ÖKC ile entegre değildir. Entegrasyon yoksa bu, yazılımın
kötü olduğu anlamına gelmez — ama mali süreci nasıl yürüteceğinizi **satın almadan önce**
netleştirmeniz gerekir. "Sonra hallederiz" denen konuların başında bu gelir.

---

## 6. Menüde bulunması gereken bilgiler

Yeme-içme işletmelerinde ürün içeriği ve alerjen bilgisinin tüketiciye sunulmasına ilişkin
düzenlemeler bulunur ve zaman içinde güncellenir. Kapsamı ilgili mevzuattan teyit edin.

Uygulamada menüde bulunması beklenenler:

- İçindekiler / bileşenler
- Alerjen uyarıları
- Kalori bilgisi
- Hayvansal içerik beyanı
- Alkol içeren ürünlerin beyanı
- Fiyatın vergiler dâhil gösterimi

Dijital menü bu bilgiler için basılı menüden daha uygundur: alan sınırı yoktur, güncelleme
anında yapılır ve bilgi ürünün yanında durur. **Bu alanları ayrı bir PDF'e gömmek yerine ürün
kartında görünür tutun** — hem tüketici bulabilsin hem de menü değiştiğinde tek yerde
güncellensin.

---

## 7. Fiyat modelleri ve gizli maliyetler

**Üç ana model:**

| Model | Nasıl işler | Dikkat |
|---|---|---|
| Aylık abonelik | Aylık ücret, güncelleme ve destek dahil | Ücret genelde şube/terminal/kullanıcı ile çarpılır |
| Yıllık kullanım bedeli | Yılda bir ödeme | Kapsamın "her şey dahil" mi olduğu sözleşmede net olmalı |
| Tek seferlik lisans | Bir kez satın alınır | Güncelleme/destek çoğunlukla ayrı yıllık bakım bedeli |

**Teklifte görünmeyen kalemler — her birini tek tek sorun:**

- Terminal veya kullanıcı başına ek ücret
- Modül ücretleri (stok, reçete, maliyet, cari, bordro, raporlar ayrı mı?)
- Kurulum, menü aktarımı ve personel eğitimi
- Destek seviyesi ve saatleri (akşam servisinde sistem durursa kimi arayacaksınız?)
- Donanım: termal yazıcı, tablet, el terminali, Android POS
- ÖKC cihazı, cihazın yıllık bedeli ve entegrasyon
- Eski sistemden veri aktarımı
- **Veri çıkışı:** ayrılmak isterseniz kendi verinizi hangi biçimde alabiliyorsunuz?
- Yenileme artışı: ikinci yıl fiyatı nasıl belirleniyor, üst sınır var mı?

**Karşılaştırmanın tek doğru yolu:** aynı senaryoyu tüm satıcılara verin — "şu kadar masa, şu
kadar terminal, şu kadar kullanıcı, şu modüller, bir yıl" — ve gelen teklifleri bu senaryonun
**bir yıllık toplam maliyeti** üzerinden kıyaslayın. Aylık rakamlar bu hesap yapılmadan
karşılaştırılamaz.

---

## 8. İşletme tipine göre öncelikler

| İşletme | Öne çıkan ihtiyaç |
|---|---|
| **Restoran** | Masa ve servis akışı, hesap bölme, rezervasyon, garson yetkileri |
| **Kafe / kahve dükkânı** | Sipariş hızı, seçenekli ürünler (boy, süt, ekstra), gel-al, vardiyalı kasa |
| **Bar** | Hızlı adisyon, açık hesap, vardiya devri, stok hassasiyeti (ölçülü satış) |
| **Fast-food** | Yoğun saat performansı, KDS, paket/kurye, sipariş tipi ayrımı |
| **Pastane** | Gramajlı satış, üretim-reçete ilişkisi, günlük fire |
| **Otel restoranı** | Oda hesabına aktarım, çoklu nokta, ayrı raporlama |
| **Çok şubeli** | Merkezî ürün/fiyat yönetimi, şube karşılaştırmalı rapor |

---

## 9. Değerlendirme kontrol listesi (22 madde)

Demo sırasında bu listeyi elinizde tutun. Cevapları satıcıdan **yazılı** isteyin.

- [ ] Bir siparişi açıp kapatmak kaç dokunuş sürüyor?
- [ ] Sık satılan ürünlere kaç dokunuşta ulaşılıyor?
- [ ] Ürün seçenekleri (boy, malzeme, ekstra) ayrı ürün açmadan tanımlanabiliyor mu?
- [ ] Sipariş mutfağa kaç saniyede düşüyor, düştüğü doğrulanabiliyor mu?
- [ ] Mutfakta istasyon ayrımı yapılabiliyor mu?
- [ ] Masa birleştirme ve sipariş taşıma var mı?
- [ ] Hesap bölme / karma ödeme destekleniyor mu?
- [ ] Veresiye ve cari takibi var mı?
- [ ] Reçete tanımlanınca stok gerçekten otomatik düşüyor mu?
- [ ] Fire ve zayiat ayrı kaydediliyor mu?
- [ ] Rapordaki "kâr" hangi giderleri içeriyor?
- [ ] Saatlik yoğunluk raporu var mı?
- [ ] İptal ve iade ayrı raporlanıyor mu?
- [ ] Yetki matrisi ne kadar ince ayarlanabiliyor (kim indirim yapabilir, kim iptal edebilir)?
- [ ] Terminal/kullanıcı sayısı fiyatı değiştiriyor mu?
- [ ] Şube eklenince fiyat ve raporlar nasıl değişiyor?
- [ ] ÖKC entegrasyonu var mı, hangi cihazlarla?
- [ ] İnternet kesildiğinde ne oluyor?
- [ ] Yedekleme kimde, ne sıklıkla, geri yükleme test edilmiş mi?
- [ ] Kurulum, eğitim, güncelleme ve destek fiyata dahil mi?
- [ ] Verilerimi dışa aktarabiliyor muyum, ayrılırsam ne oluyor?
- [ ] İkinci yıl fiyatı sözleşmede yazılı mı?

---

## 10. Kurulum ve geçiş planı

Yeni sisteme geçişi servis saatinde denemeyin. Sırayla:

1. **Menü verisini hazırlayın.** Kategoriler, ürünler, fiyatlar, görseller, seçenek grupları,
   alerjen ve kalori alanları. Bu adım en çok zaman alan kısımdır ve sonraki her şeyi belirler.
2. **Masa ve alan düzenini kurun.** Salon, teras, bahçe; masa numaraları fiziksel düzenle
   birebir örtüşsün.
3. **Yetkileri tanımlayın.** Kimin indirim yapabileceğini, iptal edebileceğini, rapor
   görebileceğini baştan belirleyin.
4. **Reçeteleri en çok satan 20 üründen başlayarak girin.** Hepsini birden girmeye
   çalışmak projeyi durdurur.
5. **Bir hafta çift kayıt yürütün.** Eski yöntem ve yeni sistem birlikte; rakamlar tutuyor mu?
6. **Personeli servis dışında eğitin.** Yoğun saatte öğrenilen sistem, yoğun saatte terk edilir.
7. **İlk ay sonunda raporları okuyun.** Saatlik yoğunluk, en çok satan, fire ve kâr marjı —
   ilk gerçek kazanç bu okumadan çıkar.

---

## 11. Sık yapılan hatalar

| Hata | Sonucu |
|---|---|
| QR kodu dosya adresine bağlamak | Menü değişince tüm kodlar geçersiz olur |
| Seçenekleri ayrı ürün olarak açmak | Menü şişer, satış raporu anlamsızlaşır |
| Reçete girmeden "kâr" raporuna bakmak | Rapordaki kâr gerçek değildir |
| Fireyi kaydetmemek | Stok her ay tutmaz, sebebi bulunamaz |
| Herkese tam yetki vermek | İptal ve indirim izlenemez hâle gelir |
| Tek internet hattıyla bulut sisteme geçmek | Hat düştüğünde satış durur |
| Menüyü servis saatinde taşımak | İlk günden personel direnci oluşur |
| Sadece aylık fiyata bakmak | Terminal/modül çarpanları toplamı ikiye katlayabilir |
| Veri çıkışını sormamak | Sistemden ayrılmak istediğinizde veriniz rehin kalır |
| ÖKC tarafını sonraya bırakmak | Mali süreç işlemez, ceza riski doğar |

---

## Kaynaklar

Yalnızca resmî kaynaklar:

- [Gelir İdaresi Başkanlığı](https://www.gib.gov.tr/) — ödeme kaydedici cihaz mevzuatı, tebliğler
- [Mevzuat Bilgi Sistemi](https://www.mevzuat.gov.tr/) — Vergi Usul Kanunu genel tebliğleri, Türk Gıda Kodeksi düzenlemeleri
- [Ticaret Bakanlığı — Tüketici Bilgi Sistemi](https://tuketici.ticaret.gov.tr/) — fiyat gösterimi ve tüketici hakları
- [Tarım ve Orman Bakanlığı](https://www.tarimorman.gov.tr/) — gıda etiketleme ve alerjen bilgilendirmesi

İlgili rehber: [E-Ticaret Sitesi Hukuki Uyum Rehberi](https://github.com/alestaweb/eticaret-hukuki-uyum-rehberi)

---

## Katkı

Düzeltme ve ekleme için issue veya pull request açabilirsiniz. Kabul edilmeyenler: belirli bir
yazılım veya hizmetin reklamı, ücret/sözleşme bilgileri, kaynağı gösterilmemiş hukuki yorum.

## Lisans

MIT

---

Bu rehber, restoran ve kafeler için QR menü ve adisyon yazılımı geliştiren
[Alesta WEB](https://alestaweb.com/adisyon-programi) tarafından derlenmiştir.
