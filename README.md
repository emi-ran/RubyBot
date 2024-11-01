# PGRuby Discord Botu

PGRuby, Ruby programlama dili ile ilgili sorulara yardımcı olmak için tasarlanmış bir Discord botudur. Google’ın Generatif AI teknolojisini kullanarak, kullanıcıların sorularına Türkçe cevaplar sunar ve sohbet geçmişini tutarak daha bağlamlı yanıtlar verir.

## Özellikler

- **Slash Komutları**: Kullanıcılar `/sor` komutunu kullanarak soru sorabilir.
- **Sohbet Geçmişi**: Her kullanıcı için son 20 etkileşimi kaydederek bağlam bilinci sağlar.
- **AI Yardımı**: Google Generative AI kullanarak programlama sorularına yanıtlar üretir.

## Gereksinimler

- Node.js (16 veya daha yüksek sürüm)
- SQLite veritabanı
- Bir Discord bot token'ı
- Google Generative AI API anahtarları

## Kurulum

1. Bu depoyu klonlayın:

   ```bash
   git clone https://github.com/emi-ran/RubyBot.git
   cd RubyBot
   ```

2. Bağımlılıkları yükleyin:

   ```bash
   npm install
   ```

3. Aşağıdaki yapıda bir `config.json` dosyası oluşturun:

   ```json
   {
     "DCToken": "DISCORD_BOT_TOKENİNİZ",
     "geminiAPIs": [
       "İLK_API_ANAHTARINIZ",
       "İKİNCİ_API_ANAHTARINIZ",
       "...ek anahtarlar..."
     ]
   }
   ```

4. SQLite veritabanı dosyası oluşturun:
   ```bash
   touch chatHistory.db
   ```

## Kullanım

1. Botu başlatın:

   ```bash
   node index.js
   ```

2. Botu Discord sunucunuza davet edin ve Ruby hakkında soru sormak için `/sor` komutunu kullanın.

## Komut

- `/sor <metin>`: Botu Ruby ile ilgili bir soru sormak için kullanın.

Bot, yanıtları Türkçe verir ve kod bloklarını kolay kopyalanabilir şekilde biçimlendirir.

## Lisans

Bu proje MIT Lisansı altında lisanslanmıştır.

```
Dilediğiniz gibi düzenleyebilir veya eklemeler yapabilirsiniz!
```
