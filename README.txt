DYSON TEKNİK BİLGİ MERKEZİ — GÜNCELLENMİŞ ARAYÜZ

Bu klasördeki index.html, app.js, config.js, manifest.webmanifest, sw.js ve icon.svg dosyaları web arayüzünü oluşturur.

YAYINA ALMA
1. GitHub deposundaki mevcut uygulama klasörünü yedekleyin.
2. Bu klasördeki dosyaları, sitenin kök dizinine aynı dosya adlarıyla yükleyin.
3. Mevcut Supabase projesini ve servis-ai-generate Edge Function'ını değiştirmeyin.
4. Supabase SQL Editor'da yeni SQL çalıştırmayın; mevcut kayıtlar Supabase'de kalır.
5. Uygulamayı HTTPS üzerinden açıp Supabase bağlantısını, bilgi eklemeyi ve soru sormayı deneyin.

ÖNEMLİ
- config.js içindeki Supabase adresi ve tarayıcıda kullanılabilen publishable anahtar, önceki projedeki ayarlarla aynıdır.
- Gemini gizli anahtarı tarayıcıya konulmaz; mevcut Edge Function üzerinden kullanılır.
- Bilgi kayıtları mevcut public.records tablosundan okunur/yazılır. Bu paket tabloya veya RLS politikalarına müdahale etmez.
- Günlük soru ve bilgi ekleme sayaçları bu tarayıcıda yerel olarak tutulur; Supabase kayıtları gibi cihazlar arasında ortaklaşmaz.
- Kategori ve alt kategori ağacı tarayıcıda saklanır ve mevcut yedekleme biçimine dahil edilir.
- Eski NOVA/Servis Asistanı yedekleri geri yükleme akışıyla uyumlu kalır.

ÖZELLİKLER
- NOVA arayüzünün koyu/neon tasarım dili korunarak Dyson markasına uyarlanmıştır.
- Ana ekranda Bilgi Yükle ve Soru Sor yan yana iki ana kutudur.
- Toplam bilgi istatistikleri ve günlük kullanım sayaçları ayrı kutulardadır.
- Son Eklenen Bilgi alanı yalnızca en son kaydı gösterir; ilk 1 saat yeşil, sonrasında kırmızı neon nabız efekti verir. Başlığa tıklayınca tüm içerik açılır.
- 10 dakika, 50 dakika ve elle dakika girerek mola başlatılabilir.
- Bilgi ekleme, fotoğraf kırpma, PDF metin çıkarma, yapay zekâ taslağını kontrol etme, soru-cevap, arama, düzenleme, silme, tam yedek ve geri yükleme korunmuştur.
