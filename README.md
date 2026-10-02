# Debug Kutusu — Ödül Çekme Uygulaması

GDG On Campus Biruni University stand haftası için ödül çekme uygulaması. Oyunu kazanan kişi için stand görevlisi butona basar; kutu sallanır, içinden bir kart fırlar, kart döner ve ödül açılır.

**Canlı sürüm:** https://idillkaradeniz.github.io/DebugBox/

## Çalıştırma

- **Yerelde:** `index.html` dosyasına çift tıklayın. Sunucu ve internet gerekmez.
- **İnternetten:** Yukarıdaki GitHub Pages adresini açın.

Stoklar, olasılıklar ve geçmiş tarayıcının `localStorage` alanında tutulur. Bu veriler o bilgisayara ve o tarayıcıya özeldir; yerel dosya ile GitHub Pages sürümü ayrı veri tutar. Stand boyunca hep aynı bilgisayarı, aynı tarayıcıyı ve aynı adresi kullanın.

## Kart türleri

| Kart türü | Ödüller | Olasılık |
|---|---|---|
| Küçük Ödül (mavi) | Atıştırmalık, Sticker | %70 |
| Orta Ödül (yeşil) | Kalem, Çakmak | %25 |
| Büyük Ödül (kırmızı) | Defter | %2,5 |
| Altın Bilet (altın) | Kalem, Çakmak veya Defter | %2,5 |

Tür seçildikten sonra ödül, kalan stoğa göre ağırlıklı olarak seçilir. Stoğu biten ödül çıkmaz. Bir türün tüm ödülleri bitince o tür çekilişten çıkar.

## Kısayollar

| Tuş | İşlev |
|---|---|
| Boşluk / Enter / ekrana tıklama | Kart çek |
| Ctrl + Z (Mac: Cmd + Z) | Son çekilişi geri al |
| F | Tam ekran |
| M | Ses aç/kapat |
| Ctrl + Shift + A | Yönetici paneli |

## Yönetici paneli

Bu panelden stokları düzenleyebilir, ödül ekleyip silebilir ve olasılıkları değiştirebilirsiniz. Panelde istatistik ve son 50 çekilişin geçmişi de görünür; geçmişi CSV olarak indirebilir, 1000 çekilişlik test simülasyonu çalıştırabilir ve verileri sıfırlayabilirsiniz.

Kalıcı varsayılan değerler `index.html` dosyasının başındaki `CONFIG` nesnesindedir.
