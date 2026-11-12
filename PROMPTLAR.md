# Yapay Zekâ Kullanım Süreci — PROMPTLAR.md

## 1. Proje Hakkında

**Proje Adı:** Psikolojik Stres Takip ve Analiz Sistemi

**Programlama Dili:** Python

**Geliştirme Ortamı:** Google Colab

**Yapay Zekâ Aracı:** ChatGPT

Bu projede yapay zekâdan proje planlama, Python kodlarının oluşturulması, kodların açıklanması, hata kontrolü, test senaryoları ve dokümantasyon hazırlanması aşamalarında destek alınmıştır.

## 2. Yapay Zekâya Yöneltilen İstekler

### Prompt 1 — Proje Planlama

**İstek örneği:**

"2030 yılında kullanılabilecek, Python ile geliştirilecek bir psikolojik stres takip sistemi projesi hazırlamak istiyorum. Projeyi adım adım planlamama yardımcı olur musun?"

**Yapay zekânın katkısı:**

Projenin amacı ve temel özellikleri belirlendi. Kullanıcıdan stres puanı, uyku süresi ve ruh hâli bilgisi alınmasına karar verildi.

### Prompt 2 — Kullanıcıdan Veri Alma

**İstek örneği:**

"Kullanıcıdan 1 ile 10 arasında stres puanı, günlük uyku süresi ve ruh hâli bilgisi alan Python kodunu oluşturmama yardımcı olur musun?"

**Yapay zekânın katkısı:**

Kullanıcı girdilerini alan fonksiyonlar hazırlandı. Girilen bilgilerin sözlük yapısında tutulması ve kayıtların bir listeye eklenmesi sağlandı.

### Prompt 3 — Stres Seviyesini Sınıflandırma

**İstek örneği:**

"Girilen stres puanını düşük, orta veya yüksek olarak sınıflandıran bir fonksiyon hazırlayabilir misin?"

**Yapay zekânın katkısı:**

Koşullu ifadeler kullanılarak stres puanları üç kategoriye ayrıldı:

- 1–3: Düşük
- 4–6: Orta
- 7–10: Yüksek

Bu kategoriler eğitim amaçlı proje kurallarıdır.

### Prompt 4 — Ana Menü Oluşturma

**İstek örneği:**

"Programın kullanıcı tarafından kolayca kullanılabilmesi için kayıt ekleme, listeleme, analiz, rapor oluşturma ve çıkış seçeneklerinden oluşan bir menü hazırlayabilir misin?"

**Yapay zekânın katkısı:**

`while` döngüsü ve koşullu ifadeler kullanılarak beş seçenekli bir ana menü oluşturuldu.

### Prompt 5 — Analiz Fonksiyonları

**İstek örneği:**

"Kaydedilen stres puanlarının ve uyku sürelerinin ortalamasını hesaplayan, stres kategorilerinin dağılımını gösteren bir analiz fonksiyonu hazırlamama yardımcı olur musun?"

**Yapay zekânın katkısı:**

Toplam kayıt sayısı, ortalama stres puanı, ortalama uyku süresi ve stres kategorilerinin dağılımını hesaplayan fonksiyonlar hazırlandı.

### Prompt 6 — Rapor Oluşturma

**İstek örneği:**

"Programdaki analiz sonuçlarını bir TXT dosyasına kaydeden Python kodunu oluşturabilir misin?"

**Yapay zekânın katkısı:**

Dosya yazma işlemleri kullanılarak analiz sonuçlarının `stres_raporu.txt` dosyasına aktarılması sağlandı.

### Prompt 7 — Hatalı Girişlerin Kontrolü

**İstek örneği:**

"Kullanıcı geçersiz stres puanı, ruh hâli veya menü seçimi girerse programın hata vermeden uyarı göstermesini sağlayabilir miyiz?"

**Yapay zekânın katkısı:**

Giriş doğrulama işlemleri ve hata kontrolü geliştirildi. Geçersiz değerlerde kullanıcıya açıklayıcı uyarılar gösterildi.

### Prompt 8 — Kodların Birleştirilmesi

**İstek örneği:**

"Google Colab'da hazırladığımız bütün fonksiyonları tek bir çalışır Python programında birleştirebilir misin?"

**Yapay zekânın katkısı:**

Fonksiyonlar tek bir programda birleştirildi. Ana menü ile diğer fonksiyonlar arasındaki bağlantılar düzenlendi ve final sürümü oluşturuldu.

### Prompt 9 — GitHub ve Dokümantasyon

**İstek örneği:**

"Tamamladığım Python projesini GitHub'a nasıl yükleyebilirim? README ve yapay zekâ kullanım dosyalarını hazırlamama yardımcı olur musun?"

**Yapay zekânın katkısı:**

GitHub'a dosya yükleme adımları açıklandı. Projenin tanıtımı ve yapay zekâ kullanım süreci için dokümantasyon taslakları hazırlandı.

## 3. Test Süreci

Program Google Colab ortamında farklı girdilerle test edildi.

| Test girdisi | Beklenen davranış | Sonuç |
|---|---|---|
| Stres puanı: 8 | Yüksek stres olarak sınıflandırma | Başarılı |
| Stres puanı: 3 | Düşük stres olarak sınıflandırma | Başarılı |
| Stres puanı: 15 | Geçersiz değer uyarısı | Başarılı |
| Menü seçimi: 9 | Hatalı menü seçimi uyarısı | Başarılı |
| Geçersiz ruh hâli seçimi: 9 | Tekrar giriş isteme | Başarılı |
| Menü seçimi: 4 | TXT raporu oluşturma | Başarılı |
| Menü seçimi: 5 | Programdan çıkma | Başarılı |

## 4. Karşılaşılan Sorunlar ve Çözümleri

### Sorun 1 — Geçersiz Kullanıcı Girdileri

Kullanıcıdan alınan değerlerin belirlenen aralıkların dışında olabilmesi bir sorun olarak değerlendirildi.

**Çözüm:** Giriş doğrulama ve hata kontrolü eklenerek programın geçersiz değerleri kabul etmemesi sağlandı.

### Sorun 2 — Kodların Farklı Hücrelerde Bulunması

Google Colab'da farklı aşamalarda oluşturulan kodların tek bir program hâline getirilmesi gerekti.

**Çözüm:** Fonksiyonlar düzenlenerek final sürümünde birleştirildi.

### Sorun 3 — Tekrarlanan Veri Girişi

Test sırasında aynı örnek kayıtlar birden fazla kez girildiğinde ortalamaların değiştiği gözlemlendi.

**Çözüm:** Kayıt sayısı ve hesaplamalar kontrol edildi. Programın mevcut kayıtlar üzerinden doğru sonuç verdiği görüldü.

### Sorun 4 — IPYNB Dosyasının Açılması

Proje dosyaları başka bir bilgisayara aktarıldığında `.ipynb` dosyası doğrudan açılamadı.

**Çözüm:** Dosya Google Colab'a yüklenerek açıldı ve GitHub'a aktarılabildi.

## 5. Yapay Zekâ Çıktılarının Kontrolü

Yapay zekâ tarafından önerilen kodlar Google Colab ortamında çalıştırıldı. Programın kullanıcı girdilerine verdiği yanıtlar incelendi.

Özellikle geçersiz değerler, stres sınıflandırması, ortalama hesaplamaları, rapor oluşturma ve programdan çıkış işlemleri kontrol edildi.

## 6. Yapay Zekânın Avantajları ve Sınırlılıkları

**Avantajları:**

- Python fonksiyonlarının geliştirilmesine yardımcı olması
- Hata kontrolü için çözüm önerileri sunması
- Kodların daha anlaşılır biçimde açıklanması
- Test senaryolarının hazırlanmasını kolaylaştırması
- Dokümantasyon sürecini desteklemesi

**Sınırlılıkları:**

- Üretilen kodların çalıştırılarak doğrulanması gerekir.
- Önerilen çözümler her ortamda aynı şekilde çalışmayabilir.
- Yapay zekâ çıktılarının proje gereksinimleriyle karşılaştırılması önemlidir.

## 7. Sonuç

Bu proje kapsamında ChatGPT, yazılım geliştirme sürecinde yardımcı bir araç olarak kullanılmıştır.

Yapay zekâ desteğiyle hazırlanan program Google Colab ortamında test edilmiş, kullanıcı girdileri kontrol edilmiş ve analiz sonuçları incelenmiştir.

Bu süreç, Python programlama yapılarının uygulanması ve yapay zekâ destekli yazılım geliştirme konusunda deneyim kazanılmasını sağlamıştır.
