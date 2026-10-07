# Nine Lives Spirit Cats sitesini yayına alma

Bu klasör senin gerçek web siten. Sitede görünen tüm yazı, ürün ve fiyatlar `site.json` dosyasında,
görseller `img/` klasöründe duruyor. Kurulum bir kez yapılır. Toplam süre yaklaşık 20–30 dakika.

Senin yapacakların: 3 ücretsiz hesap açmak ve alan adını satın almak. Hesap açma ve ödeme adımlarını
senin yerine yapamam.

---

## 1. GitHub: dosyaların durduğu yer (ücretsiz)

1. https://github.com adresine gir ve **Sign up** ile hesap aç.
2. Sağ üstteki **+** → **New repository**.
   - Repository name: `ninelives-site`
   - **Private** seç (dosyaların sadece sende kalsın).
   - **Create repository**'ye bas.
3. Açılan sayfada **uploading an existing file** linkine tıkla.
4. Bilgisayarında `NineLives_Site` klasörünü aç ve **içindeki her şeyi** seç (Ctrl+A).
   Seçime `img` klasörü ve `.pages.yml` dosyası da girmeli. Hepsini tarayıcıdaki kutuya sürükle.
   (Klasörün kendisini değil, **içindekileri** sürükle.)
5. Aşağıdaki **Commit changes** butonuna bas.

## 2. Netlify: siteyi internette yayınlayan yer (ücretsiz)

1. https://app.netlify.com adresine gir → **Sign up** → **GitHub ile giriş** seç.
2. **Add new project** → **Import an existing project** → **GitHub**.
3. Listeden `ninelives-site`'ı seç. Ayarlarda hiçbir şeyi değiştirme
   (Build command boş, Publish directory boş kalsın).
4. **Deploy**'a bas. Yaklaşık 1 dakika sonra siten `xxxx.netlify.app` adresinde açılır.
5. İstersen **Project configuration → Change project name** ile adresi
   `ninelivesspiritcats.netlify.app` gibi bir adla değiştir.

## 3. Pages CMS: siteyi düzenleyeceğin panel (ücretsiz)

1. https://app.pagescms.org adresine gir → **Sign in with GitHub**.
2. GitHub uygulamasını kurmanı isteyecek. **Only select repositories** → `ninelives-site` → **Install**.
3. Panelde `ninelives-site`'ı aç. Solda **Site (yazılar ve ürünler)** göreceksin.
   - **Ürünler**: ad, fiyat, görsel, efsane, Etsy linki. Yeni ürün eklemek için **Add an entry**.
     Sırayı sürükleyerek değiştirirsin.
   - **Sayfa yazıları**: başlıklar, hikâye, notlar.
   - **Etsy mağaza linki**: doldurunca sitede "Shop on Etsy" butonu çıkar.
4. İşin bitince **Save**'e bas. Netlify değişikliği görür ve siten **1–2 dakika içinde** güncellenir.

Panel Türkçe etiketli. Panelin kendi menüleri İngilizce olabilir.

## 4. Alan adı (yılda yaklaşık 10–15 $)

En kolay yol, alan adını doğrudan Netlify'dan almak. Böylece ayar yapman gerekmez.

1. Netlify'da projeni aç → **Domain management** → **Add a domain**.
2. İstediğin adı yaz (ör. `ninelivesspiritcats.com`). Boştaysa fiyatını gösterir.
3. Satın al. Netlify adresi siteye kendisi bağlar ve güvenli bağlantıyı (https) kendisi açar.
   Bu işlem birkaç dakika ile birkaç saat sürebilir.

Başka bir yerden (Namecheap, Cloudflare, GoDaddy) aldıysan: Netlify'da **Add a domain**
ekranındaki yönergeleri izle, sana verdiği DNS ayarlarını alan adını aldığın sitede gir.

---

## Sorun çıkarsa

- **Sitede ürünler görünmüyor:** `site.json` dosyası GitHub'a yüklenmemiş olabilir. GitHub'daki
  dosya listesinde `site.json`, `index.html`, `img` ve `.pages.yml` görünmeli.
- **Panelde "configuration" hatası:** `.pages.yml` dosyası eksik. Windows bu dosyayı gizleyebilir.
  GitHub'da **Add file → Upload files** ile tekrar yükle.
- **Kaydettim ama site değişmedi:** 2 dakika bekle, sonra sayfayı Ctrl+F5 ile yenile.
