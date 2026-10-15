# AeXp Source Media

Masaüstü medya indirici ve dönüştürücü. Tek video, oynatma listesi ve toplu bağlantı indirir; ses ve video formatlarına dönüştürür.

Sürüm: 1.0.0
Geliştirici: Abdullah Ekşi — [abdullaheksi.tr](https://abdullaheksi.tr) / [aexpan.tr](https://aexpan.tr)

## İndir

**[AeXp Source Media 1.0.0 Setup.exe'yi indir](https://github.com/abdullah-eksi/aexp_mediasource/releases/download/v1.0.0/AeXp.Source.Media.1.0.0.Setup.exe)**

Tüm sürümler: [Releases](https://github.com/abdullah-eksi/aexp_mediasource/releases)

## Ne Yapar?

- Tek video, playlist ve çoklu URL ile toplu indirme
- Ön izleme: bağlantıları çözüp başlık + kapak gösterir, tekrarları tespit eder
- Ses çıktıları: MP3, M4A, OPUS, WAV, FLAC (128K–320K / Otomatik)
- Video çıktıları: MP4, WEBM, MKV (360p–4K / En iyi)
- Kuyruk: 1–5 paralel indirme, duraklat / sürdür, hemen başlat, tekrar dene, iptal, sil
- Kapak gömme ve dosya bilgisi (metadata) ekleme
- İlk açılışta eksik bileşenleri otomatik kurar, internet yoksa daha sonra tekrar dener
- Kullanıcı dostu hata mesajları, teknik detaylar log dosyasına yazılır

## Kullanılan Araçlar

| Araç | Amaç |
|---|---|
| Electron | Uygulamayı Windows masaüstü programı olarak çalıştırır |
| Node.js | Dosya, kuyruk ve arka plan işlemlerini yönetir |
| yt-dlp | Video / ses / playlist indirme motoru |
| FFmpeg | Ses-video birleştirme ve format dönüştürme |
| Deno | yt-dlp'nin site doğrulamaları için gereken JS çalıştırıcısı |
| electron-builder (NSIS) | Kurulum dosyası (Setup) üretir |
| yauzl | İndirilen zip içinden program dosyası çıkarmak için |
| ffmpeg-static | Kurulum paketine hazır FFmpeg eklemek için |

## Kurulum

AeXp Source Media Setup Exe Dosyasını Çalıştırın Basit Şekilde Kurun !

- `AeXp Source Media 1.0.0 Setup.exe` — klasik kurulum (Masaüstü + Başlat menüsü kısayolu)

1. Setup dosyasını çalıştırıp kayıt klasörünü seçin.
2. Uygulamayı açın, ilk açılışta bileşenler otomatik hazırlanır.
3. Bağlantıyı yapıştırıp format + kalite seçin, `Kuyruğa ekle`ye basın.

Varsayılan kayıt klasörü: `Masaüstü / AeXp Media`
