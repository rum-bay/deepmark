# Deepmark TR

**Kaydettiklerini başlığa göre değil, hatırladığın şeye göre bul.** Deepmark TR; web bağlantılarını, videoları ve notları tek yerde toplayan, Türkçe arama ve yerel içerik örnekleriyle uyarlanmış bir araştırma hafızası prototipidir.

Bu proje, 2026’da Hacker News’te tanıtılan Deepmark bookmark-search ürününün temel akışını klonlar ve Türkiye odaklı bir demo olarak yeniden yorumlar. Tek dosyalı uygulamadır; kurulum veya derleme gerekmez.

## Çalıştırma

1. index.html dosyasını güncel bir tarayıcıda aç.
2. Arama kutusunda mahalle deprem planı, kahve köpüğü veya KOBİ yapay zekâ gibi terimleri dene.
3. Bağlantı kaydet ile URL, not ve etiket ekle.
4. Chrome veya Firefox’tan dışa aktardığın yer imi HTML dosyasını Yer imlerini içe aktar ile yükle.
5. Kütüphanene sor düğmesiyle örnek kütüphanede sor; yanıtla ilişkili kayıtları kaynak olarak aç.

Kayıtlar tarayıcının localStorage alanında tutulur. Verilerimi indir kütüphaneyi JSON olarak dışa aktarır. GitHub Pages gibi statik barındırma servislerinde de çalışacak şekilde harici paket veya API kullanmaz.

## Neler var?

- İçerik notu, başlık, etiket ve alan adı üzerinde arama; Türkçe karakter normalleştirmesi ve birkaç Türkçe/İngilizce eş anlamlı terim.
- Bağlantı ekleme, favori, okundu/okunmadı, kayıt silme ve kaynak bağlantısını açma.
- Yer imi HTML içe aktarma; aynı URL’yi ikinci kez eklememe.
- Kaynak kayıtları gösteren demo Kütüphanene sor akışı.
- Web, YouTube, Instagram ve PDF için filtreler; mobil uyumlu görünüm.
- Türkçe ve Türkiye bağlamlı örnek içerikler: AFAD, GİB, YÖK ve İzmir.

## Ödev gereklilikleriyle eşleşme

| Gereklilik | Projedeki karşılığı |
| --- | --- |
| Hacker News, YC ve RFS incelemesi | RESEARCH.md içinde 2026 Show HN sinyali ve YC Fall 2026 RFS bağlantıları, değerlendirme ve kapsam notuyla belgelenmiştir. |
| 2026 ve sonrası teknolojik değişimden ürün seçimi | Çok kipli içerik çıkarımı ve anlam temelli arama, güncel teknolojik fırsat olarak ele alınmıştır. |
| En azından clone uygulama | index.html, arama-kütüphane-kayıt ayrıntısı ve kaynak gösteren soru akışını çalışan, bağımsız bir ön yüz prototipi olarak sunar. |
| Yerelleştirme / yenilikçilik | Türkçe sorgu normalleştirmesi, yerel örnek kaynaklar ve kişisel kayıtlardan öğrenme yönü eklenmiştir. |
| 85 sayfa üst sınırı | Proje kısa bir README ve araştırma notundan oluşur; uzun rapor gerektirmez. |

## Kapsam ve sınırlamalar

Bu bir ders prototipidir; örnek kütüphane demo verisidir. Uygulama harici sayfa içeriğini otomatik çekmez, videoyu transkribe etmez, sosyal medya hesabına bağlanmaz ve gerçek bir üretken AI modeli ya da vektör veritabanı çalıştırmaz. Arama, tarayıcıda tutulan başlık, not, özet ve etiketleri eşleştirir; Kütüphanene sor eşleşen örnek kayıtların özetini ve kaynaklarını gösterir. Bu yüzden ürün sayfasındaki çok dilli transkripsiyon ve derin medya indeksleme özellikleri bu klonda varmış gibi sunulmamıştır.

Gerçek ürüne geçişte sayfa/video indeksleme, izinli platform bağlantıları, sunucu tarafı arama, hesaplar arası senkronizasyon ve KVKK’ya uygun veri yönetimi ayrıca tasarlanmalıdır.

## Dosyalar

- index.html — uygulama, stil ve JavaScript tek dosyada.
- README.md — kurulum, işlevler ve ödev gereklilikleri.
- RESEARCH.md — ürün tezi, kaynaklar ve isim çakışması notu.

