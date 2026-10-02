# Ledolet Sipariş Sözleşmesi

Ledolet sipariş formunu tarayıcıda doldurup A5 PDF olarak indirmeye yarayan tek sayfalık web uygulaması.

## Özellikler
- 20 ürün satırı (Cinsi, Miktarı, Birim Fiyatı); satır tutarı, Ara Toplam, İskonto, K.D.V. ve Genel Toplam otomatik hesaplanır
- İskonto tutar (`500`) veya oran (`%10`) olarak girilebilir
- K.D.V. oranı seçilebilir (%20 / %10 / %1 / yok)
- Sıralı sipariş numarası: PDF indirildiğinde numara kullanılmış sayılır, "Yeni form" bir sonrakini açar
- Taslak ve sayaç tarayıcının yerel hafızasında (localStorage) saklanır
- Kaşe/imza alanı boş bırakılır (ıslak imza için)

## Kurulum (GitHub Pages)
1. Yeni bir repo oluşturun ve `index.html` ile `README.md` dosyalarını yükleyin.
2. **Settings → Pages** bölümünde *Source* olarak `main` dalını ve `/ (root)` klasörünü seçin.
3. Birkaç dakika sonra uygulama `https://<kullanici-adi>.github.io/<repo-adi>/` adresinde açılır.

## İlk kullanım
Üst çubuktaki **Sipariş No** kutusuna koçandaki sıradaki numarayı (ör. `02054`) yazın. Sonraki formlar buradan devam eder.

## Notlar
- Numara sayacı **her tarayıcıda ayrı** tutulur. Farklı bilgisayarlardan kullanılacaksa ortak bir sayaç (ör. Google Apps Script + Sheets) eklenmelidir.
- Firma adresi, telefon ve e-posta `index.html` içindeki `COMPANY` sabitinden değiştirilebilir.
- Harici kütüphaneler: html2canvas 1.4.1 ve jsPDF 2.5.1 (cdnjs üzerinden).
