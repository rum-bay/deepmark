# Ürün seçimi ve kaynak incelemesi

## Seçilen ürün

**Deepmark TR — Türkçe kişisel araştırma hafızası.** Kullanıcı web sayfalarını ve başka içerikleri kaydeder; daha sonra başlığını hatırlamasa bile içerikten, kısa nottan veya anlamsal çağrışımından bulur. Prototip, Hacker News’te 2026’da tanıtılan Deepmark bookmark-search fikrinin temel akışını klonlar. Yerel uyarlama olarak Türkçe karakter normalleştirmesi, Türkçe/İngilizce basit eş anlamlılar ve AFAD, GİB, YÖK, İzmir temalı örnekler eklenmiştir.

## Teknolojik kırılma ve neden şimdi?

Geleneksel yer imi yöneticisi çoğunlukla başlık ve URL saklar. Kullanıcı içeriği konuşma, görsel, altyazı veya sayfanın gövdesi içindeyse eski yöntem aradığı parçayı bulamayabilir. Çok kipli yapay zekâ; metin çıkarımı, konuşmayı yazıya dönüştürme ve görsel içeriğini açıklama gibi işlemleri tek bir kayıt akışında birleştirmeyi mümkün kılıyor. Böylece arama “hangi sayfaydı?” sorusunun yanında “videoda anlatılan yöntem neydi?” gibi yaklaşık hatırlamaya da yanıt verebilir.

Bu değişim için seçilen ürün, çok kipli indekslemeyi kişisel bilgi erişimine uyguluyor. Prototipte gerçek çok kipli indeksleme yoktur; fikir ve etkileşim modeli gösterilir, demo araması örnek metin ve notlarda çalışır.

## Hacker News sinyali

2026 tarihli [Show HN: Deepmark — Search your bookmarks by what’s inside them, not the title](https://news.ycombinator.com/item?id=49288896) gönderisi ürünü içerik içinden aranan yer imi kütüphanesi olarak tanıtıyor. Görünen sayfa anlık görüntüsünde gönderi 5 puan ve 5 yorum almış. Bir yorumcu, HN’de beğenilen gönderileri aramanın yararlı olacağını söylüyor; başka bir yorum çoklu kaynak ve medya indekslemesini tarayıcının temel yer imi aramasından ayrıştırıyor.

Bu, fikir için erken topluluk ilgisi ve kullanım sorunu sinyalidir; küçük puan/yorum sayısı pazar doğrulaması ya da geniş talep kanıtı değildir.

## YC / RFS sinyali

YC’nin [Fall 2026 Requests for Startups](https://www.ycombinator.com/rfs) sayfasındaki **The Primer** bölümü, her kullanıcıya uyum sağlayan, zaman içinde öğretme biçimini değiştiren AI öğrenme ürünlerini teşvik ediyor. Deepmark TR, doğrudan çocuk öğretmeni geliştirmiyor. Bunun yerine kullanıcının kendi seçtiği kaynakları geri çağırmasını ve onlardan öğrenmesini sağlayan kişisel hafıza katmanını prototipliyor. RFS burada ürün yönü için bağlamdır; Deepmark için YC yatırım veya onay beyanı değildir.

## Ürün akışı ve yerel katkı

1. Kullanıcı örnek içerik kütüphanesinde hatırladığı bir ifadeyle arama yapar.
2. Başlık, not, özet, etiket ve alan adı eşleşmeleri puanlanır.
3. Kayıt ayrıntısı, kaynak bağlantısını ve hatırlama notunu gösterir.
4. Kütüphanene sor demo akışı eşleşen kayıtları ve dayandığı kaynakları listeler.
5. Kullanıcı bağlantı/not ekler veya tarayıcı yer imi dosyasını içe aktarır; verisini JSON olarak dışa alabilir.

Yerelleştirme, arayüzün Türkçe olmasının ötesine geçer: ı/İ ve aksan normalizasyonu, sınırlı karşı dil eşleştirmesi, Türkiye’de kullanılan kurum alan adları ve yerel gündelik içerik örnekleri vardır. Bir sonraki yenilik adımı, kullanıcı onayıyla Türkçe ders notlarından küçük öğrenme kartları ve kaynaklı tekrar soruları üretmek olabilir.

## Ürün adı uyarısı

Deepmark adı başka ürünlerce de kullanılıyor. Bu projede kastedilen, [Hacker News Show HN paylaşımındaki](https://usedeepmark.com/) yer imi ve içerik arama ürünüdür. YC’nin [DeepMark şirket dizinindeki](https://www.ycombinator.com/companies/deepmark) aynı adlı girişim ise AI sesine makinece okunabilir kimlik işareti gömen ayrı bir ses doğrulama şirketidir. Ödev prototipinde istenen fikir adına Deepmark adı tutuldu; gerçek bir yayın öncesinde marka ve alan adı araştırması yapılmalıdır.

## Kaynaklar

1. Hacker News, [Show HN: Deepmark — Search your bookmarks by what’s inside them, not the title](https://news.ycombinator.com/item?id=49288896) — 2026 gönderisi ve topluluk yorumları.
2. Deepmark, [ürün sayfası](https://usedeepmark.com/) — ürün özellikleri ve performans iddiaları ürün sahibinin beyanıdır; bağımsız ölçüm olarak sunulmamıştır.
3. Deepmark, [gizlilik açıklaması](https://usedeepmark.com/privacy) — çevrim içi ürünün saklama/işleme modeli; yerel prototipin veri tercihiyle karşılaştırma.
4. Y Combinator, [Requests for Startups](https://www.ycombinator.com/rfs) — Fall 2026 The Primer başlığı.
5. Y Combinator, [DeepMark şirket profili](https://www.ycombinator.com/companies/deepmark) — isim benzerliğini ayırmak için.
