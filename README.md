# 🎬 Sine-Sinema | Web 3.0 Film Keşif Platformu

Sine-Sinema, sinema verilerini Web 1.0'dan Web 3.0'a uzanan bir teknoloji yelpazesinde sunan, anlamsal veri odaklı bir web uygulamasıdır. Bu proje, **BBY262 Semantik Bilgi Yönetimi** dersi kapsamında, verinin yapılandırılması (XML) ve anlamsal bir ağa (RDF) dönüştürülmesini somutlaştırmak amacıyla geliştirilmiştir.


---

## 🛠 Kullanılan Teknolojiler
* **Arayüz (Web 2.0):** HTML5, CSS3 (Modern Flex & Grid), JavaScript (ES6+).
* **Veri Yapılandırma:** XML (Extensible Markup Language).
* **Veri Doğrulama:** XSD (XML Schema Definition).
* **Semantik Katman (Web 3.0):** RDF (Turtle Formatı), RDFa (HTML Anotasyonları).
* **Ontoloji Standartları:** Schema.org, RDFS, Dublin Core.

---

## 📂 Proje Yapısı ve Dosyalar
* `index.html`: Uygulamanın ana arayüzü ve XML verilerini işleyen JavaScript motoru.
* `movies.xml`: 21 adet film kaydını içeren ana veri dosyası.
* `directors.xml`: Yönetmen bilgilerini tutan ilişkisel XML dosyası.
* `categories.xml`: Film türlerini/kategorilerini tutan XML dosyası.
* `schema.xsd`: XML dosyalarının yapısal doğruluğunu denetleyen şema.
* `movies.ttl`: Verilerin anlamsal bağlarını (triples) içeren Turtle dosyası.

---

## ⚙️ Kurulum ve Çalıştırma Talimatları

Proje, istemci taraflı (client-side) çalıştığı için herhangi bir veritabanı kurulumu gerektirmez. Ancak tarayıcıların **CORS (Cross-Origin Resource Sharing)** güvenlik politikaları nedeniyle, XML dosyalarının okunabilmesi için bir sunucu üzerinden çalıştırılması **zorunludur**.

### 1. Yerel Bilgisayarda Çalıştırma (VS Code)
1.  Bu depoyu bilgisayarınıza indirin veya klonlayın.
2.  VS Code editörünü açın.
3.  Eklentiler kısmından **"Live Server"** eklentisinin kurulu olduğundan emin olun.
4.  `index.html` dosyasına sağ tıklayıp **"Open with Live Server"** seçeneğine basın.
5.  Uygulama varsayılan tarayıcınızda `http://127.0.0.1:5500` adresinde açılacaktır.

### 2. Sunucuya Yükleme (Hacettepe Sunucusu vb.)
1.  Tüm proje dosyalarını sunucunuzdaki hedef klasöre (örn: `public_html/proje2/`) yükleyin.
2.  Dosya izinlerinin (CHMOD) okunabilir olduğundan emin olun.
3.  Tarayıcıdan ilgili URL'ye giderek sistemi kullanmaya başlayabilirsiniz.

---

## 💡 Öne Çıkan Özellikler
* **Dinamik İlişki Haritası:** Bir filme tıklandığında, semantik bağlar (Linked Data) kullanılarak aynı yönetmene veya aynı türe ait diğer filmler otomatik olarak önerilir.
* **Veri Entegrasyonu:** Sistem 3 farklı XML dosyasını anlık olarak birleştirerek (Join) anlamlı bir bütün oluşturur.
* **Semantik Anotasyonlar:** Sayfa içeriği RDFa ile işaretlenmiştir; böylece arama motorları içeriği yapılandırılmış veri olarak algılayabilir.
* **Anlık XML İndirme:** Kullanıcılar ilgilendikleri filmin verisini tek tıkla yapılandırılmış XML olarak bilgisayarlarına indirebilirler.

---

## 📝 Lisans ve Akademik Bilgi
Bu proje **Hacettepe Üniversitesi Bilgi ve Belge Yönetimi Bölümü** bünyesinde yürütülen Semantik Bilgi Yönetimi dersi final projesidir.

**Geliştirici:** Esra :)
