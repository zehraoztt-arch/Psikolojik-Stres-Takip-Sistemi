# Psikolojik-Stres-Takip-Sistemi
2030 yılı meslek senaryosu kapsamında Python ile geliştirilen psikolojik stres takip ve analiz sistemi.
# Psikolojik Stres Takip ve Analiz Sistemi

## 1. Proje Hakkında

Bu proje, 2030 yılında psikolojik danışmanlık ve ruh sağlığı alanında kullanılabilecek dijital takip sistemlerinden yola çıkılarak Python programlama diliyle geliştirilmiştir.

Sistem, kullanıcıların günlük stres seviyelerini, uyku sürelerini ve ruh hâllerini kaydederek bu bilgileri analiz etmeyi amaçlamaktadır.

Proje eğitim amacıyla hazırlanmıştır ve psikolojik tanı koyma amacı taşımamaktadır.

## 2. Projenin Amacı

- Günlük stres seviyelerini takip etmek.
- Uyku süresi ve ruh hâli bilgilerini kaydetmek.
- Stres seviyelerini düşük, orta ve yüksek olarak sınıflandırmak.
- Ortalama stres ve uyku süresini hesaplamak.
- Günlük kayıtları listelemek.
- Analiz sonuçlarını TXT dosyasına kaydetmek.
- Hatalı kullanıcı girişlerini kontrol etmek.

## 3. Programın Özellikleri

Program beş seçenekten oluşan bir ana menüye sahiptir:

1. Yeni Stres Kaydı Ekle
2. Günlük Kayıtları Listele
3. Genel Stres Analizi Yap
4. Stres Raporunu Dosyaya Kaydet
5. Programdan Çık

### Stres sınıflandırması

| Stres puanı | Kategori |
|---|---|
| 1–3 | Düşük |
| 4–6 | Orta |
| 7–10 | Yüksek |

Bu sınıflandırma proje kapsamında örnek olarak belirlenmiştir ve klinik değerlendirme ölçütü değildir.

## 4. Kullanılan Teknolojiler

- Python 3
- Google Colab
- GitHub
- TXT dosya işlemleri

Programda kullanılan Python yapıları:

- Değişkenler ve veri tipleri
- Listeler ve sözlükler
- Fonksiyonlar
- `if`, `elif`, `else` koşulları
- `while` ve `for` döngüleri
- `try` ve `except` ile hata kontrolü
- Dosya okuma/yazma işlemleri
- Matematiksel hesaplamalar

## 5. Programın Çalıştırılması

1. Projedeki `Psikolojik_Stres_Takip_FINAL.ipynb` dosyasını indirin.
2. Google Colab üzerinden açın.
3. Kod hücresini çalıştırın.
4. Ana menüden yapmak istediğiniz işlemi seçin.
5. Stres, uyku ve ruh hâli bilgilerini girin.
6. Analiz sonuçlarını görüntüleyin.
7. İsterseniz raporu TXT dosyasına kaydedin.

Alternatif olarak Python 3 kurulu bir bilgisayarda `psikolojik_stres_takip_final.py` dosyası çalıştırılabilir.

## 6. Test Senaryoları

| Test | Beklenen sonuç | Gözlemlenen sonuç |
|---|---|---|
| Stres puanı 8 | Yüksek stres | Yüksek stres |
| Stres puanı 3 | Düşük stres | Düşük stres |
| Stres puanı 5 | Orta stres | Orta stres |
| Menüye 9 girilmesi | Hatalı seçim uyarısı | Uyarı gösterildi |
| Geçersiz ruh hâli | Hata uyarısı | Uyarı gösterildi |
| Stres puanı 15 | Geçersiz puan uyarısı | Uyarı gösterildi |
| Menüden 5 seçilmesi | Programdan çıkış | Program kapandı |

## 7. Örnek Analiz Sonuçları

Dört örnek kayıtla yapılan son sürüm testinde:

- Toplam kayıt: 4
- Ortalama stres seviyesi: 5.5
- Ortalama uyku süresi: 6.5 saat
- Düşük stres: 2 kayıt
- Orta stres: 0 kayıt
- Yüksek stres: 2 kayıt

## 8. Projenin Sınırlılıkları

Program kayıtları çalışma sırasında bellekte tutmaktadır. Program yeniden başlatıldığında kayıt listesi sıfırlanır.

Oluşturulan TXT raporu, analiz sonuçlarının dosyaya kaydedilmesini sağlar.

Sistem psikolojik tanı, tedavi veya profesyonel değerlendirme yerine geçmez.

## 9. Yapay Zekâ Kullanımı

Projenin geliştirilmesi sırasında ChatGPT'den kod oluşturma, fonksiyonları açıklama, hataları belirleme, giriş doğrulama ve test senaryoları hazırlama konularında destek alınmıştır.

Kodlar Google Colab ortamında çalıştırılarak test edilmiş, karşılaşılan hatalar incelenmiş ve gerekli düzenlemeler yapılmıştır.

Yapay zekâ ile çalışma süreci ayrıca PROMPTLAR.md dosyasında belgelenecektir.

## 10. Proje Dosyaları

- `psikolojik_stres_takip_final.py` — Python kaynak kodu
- `Psikolojik_Stres_Takip_FINAL.ipynb` — Google Colab defteri
- `stres_raporu-3.txt` — Örnek stres analiz raporu
- `README.md` — Proje açıklaması
- `PROMPTLAR.md` — Yapay zekâ kullanım süreci

## 11. Sonuç

Psikolojik Stres Takip ve Analiz Sistemi, Python programlama dilinin temel yapılarını kullanarak günlük verilerin kaydedilmesini, analiz edilmesini ve raporlanmasını sağlayan eğitim amaçlı bir uygulamadır.

Proje kapsamında kullanıcı etkileşimi, veri doğrulama, koşullu işlemler, döngüler, fonksiyonlar ve dosya işlemleri uygulamalı olarak kullanılmıştır.
