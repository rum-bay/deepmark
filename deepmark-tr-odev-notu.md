# Deepmark TR — Kişisel araştırma hafızası

**Ödev fikri:** 2026 ve sonrasında hızlanan çok kipli yapay zekâ ile, kaydedilen bağlantıların içerik ve anlam üzerinden aranabildiği kişisel bilgi kütüphanesi.

**Ürün:** Deepmark TR — Deepmark’ın yer imlerini içerik içinde arama yaklaşımının Türkçe, bölgesel ve öğrenme odaklı prototipi.

**Çalışan prototip:** [deepmark-tr.html](deepmark-tr.html)

## Ürün tezi

İnsanlar bağlantı, video, PDF ve sosyal medya gönderilerini “sonra bakarım” diye kaydediyor; ancak başlığını hatırlamadıklarında yeniden bulamıyor. Yapay zekâdaki kırılma, bu kayıtlara yalnızca başlık ve URL olarak değil; metin, konuşma, görseldeki yazı ve anlamsal bağlam olarak bakmayı mümkün kılıyor. Böylece kullanıcı arşivine “geçen hafta izlediğim, kahveyi soğuk suyla demleyen video hangisiydi?” diye sorabiliyor.

Türkiye sürümünün farkı Türkçe arama davranışına ve yerel bilgi kaynaklarına odaklanması: Türkçe karakter toleransı, Türkçe/İngilizce terimlerle arama, AFAD ve GİB gibi kaynaklardan örnekler, ayrıca bulunan yanıtı kaynağıyla birlikte gösterme. İkinci katmanda, kullanıcının kendi kayıtlarından küçük öğrenme yolları üretmek hedefleniyor. Bu, YC’nin Fall 2026 RFS’inde anlattığı kişiye uyum sağlayan “Primer” fikrini kişisel araştırma ve öğrenmeye taşıyan bir ürün yönü.

## Neden şimdi?

- **Hacker News sinyali:** 2026 tarihli Show HN gönderisi Deepmark’ı “yer imlerini başlıktan değil, içeriğinden arama” ürünü olarak tanıtıyor. İlk gönderi 5 puan ve 5 yorum almış; bu erken ve sınırlı bir sinyal, pazar kanıtı değil. Yorumlarda bir kullanıcı HN’de beğendiklerini aramanın da faydalı olacağını söylüyor; başka bir yorumcu bu tür çok kaynaklı derin indekslemenin tarayıcıların yer imi aramasından farklılaştığını belirtiyor.
- **Teknoloji kırılması:** Deepmark’ın ürün açıklaması sayfa metni, ses/video transkripti, karelerdeki yazı ve görsel açıklamalarını aynı kütüphanede aranabilir yaptığını belirtiyor. Ürün, bazı 99 dilde arama ve farklı diller arasında sorgu desteği sunduğunu iddia ediyor. Bunlar ürün sahibinin yayımladığı özellik ve performans beyanlarıdır.
- **YC / RFS yönü:** YC Fall 2026 RFS, AI’ı kişiye uyum sağlayan, zaman içinde öğretme biçimini değiştiren bir “Primer” olarak tarif ediyor. Deepmark TR’nin ilk sürümü bir çocuk öğretmeni değil; kişinin kendi seçtiği kaynaklardan geri çağırma ve öğrenme sağlayan hafıza katmanı. RFS, bu ürünün doğrudan talebi olduğuna dair kanıt değil; kişiselleştirilmiş bilgi ürünleri için yön gösteren bir çerçeve.

## Prototipte neler çalışıyor?

- Önceden yüklenmiş Türkçe örnek kütüphanede arama; içerik özeti, başlık, etiket ve alan adında eşleştirme.
- Türkçe karakterlerin normalleştirilmesi ve sınırlı eş anlamlı terim eşlemesi.
- Bağlantı, not ve etiketle yeni kayıt ekleme; yıldızlama, okundu işaretleme ve silme.
- Chrome/Firefox yer imi yöneticilerinden dışa aktarılan HTML dosyasını seçerek içe alma.
- “Kütüphanene sor” penceresinde bulunan örnek kayıtları ve kaynak bağlantılarını gösterme.
- Kütüphaneyi JSON olarak dışa aktarma; kayıtların tarayıcıda saklanması.
- Türkiye bağlamlı demo kayıtları: AFAD, GİB, YÖK, TÜBİTAK ve İzmir gibi yerel arama örnekleri.

## Dürüst kapsam notu

Bu, tek HTML dosyasında çalışan bir arayüz ve etkileşim prototipidir. Örnek kayıtlar demodur. Bu sürüm sayfaları taramaz, videoları yazıya dökmez, sosyal ağ hesaplarına bağlanmaz ve gerçek bir dil modeli ya da vektör arama kullanmaz. İçe aktarılan yer imleri başlık ve URL üzerinden aranır; yeni bağlantıların özeti kullanıcının girdiği nota dayanır. “Kütüphanene sor” demo eşleşmelerini kaynaklarıyla sunar. Gerçek ürün aşamasında içerik işleme, OAuth/eklenti bağlantıları, güvenli hesap senkronizasyonu ve KVKK’ya uygun veri saklama ayrıca geliştirilmelidir.

## İsim notu

“Deepmark” adı çakışıyor. Bu ödevde kopyalanan ürün, Hacker News’te gösterilen ve [usedeepmark.com](https://usedeepmark.com/) adresinde bulunan yer imi/içerik arama ürünüdür. Y Combinator şirket dizininde aynı isimle görünen [DeepMark](https://www.ycombinator.com/companies/deepmark) ise AI sesine kimlik işareti gömen ayrı bir ses doğrulama girişimidir. Ödev demosunda istek doğrultusunda Deepmark adı korunmuştur; kamuya açık gerçek bir lansmanda farklı bir ad seçmek gerekir.

## Kaynaklar

1. [Show HN: Deepmark — Search your bookmarks by what’s inside them, not the title](https://news.ycombinator.com/item?id=49288896) — 2026 topluluk paylaşımı ve yorumlar.
2. [Deepmark — ürün açıklaması](https://usedeepmark.com/) — çok kaynaklı kayıt, içerik indeksleme, çok dilli arama ve kütüphaneye agent erişimi ürün beyanları.
3. [Y Combinator — Requests for Startups, Fall 2026](https://www.ycombinator.com/rfs) — The Primer: kişiye uyumlu AI öğrenme ürünü çağrısı.
4. [Y Combinator — DeepMark](https://www.ycombinator.com/companies/deepmark) — aynı isimli ayrı ses kimlik doğrulama şirketi.
5. [Deepmark gizlilik açıklaması](https://usedeepmark.com/privacy) — çevrim içi ürünün sakladığı içerik ve üçüncü taraf işleme bilgileri; yerel prototip tercihi için karşılaştırma.

## Demo

`deepmark-tr.html` dosyasını güncel bir tarayıcıda aç. Arama kutusuna örneğin “mahalle deprem planı”, “kahve köpüğü” veya “KOBİ yapay zekâ” yaz. “Bağlantı kaydet” ile kayıt ekleyebilir, “Yer imlerini içe aktar” ile tarayıcıdan dışa aktarılan `.html` yer imi dosyasını yükleyebilirsin. “Kütüphanene sor” sonuçları kaynak kayıtlarla birlikte açar. Veriler bu tarayıcıda kalır; “Verilerimi indir” ile JSON dışa aktarımı yapılır.
