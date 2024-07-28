# Otellerde Drone ile Teslimat

## Giriş

Günümüzde drone'lar ile yapılan ve bazı ülkelerde testleri halen sürmekte olan
birçok proje mevcut. Bu projelerin birçoğu şehir içinde kargo, yemek, içecek, gıda ürünleri vb. gibi ürünleri teslimat için tasarlanmıştır. Bu konseptte drone projelerinin gelişimi ve test aşamaları oldukça zor ve maliyetlidir. Drone'ların bakımı, satın alınıp modifiye edilmesi, gömülü yazılımları ve eğer varsa yapay zeka modellerini üretmek zaten ciddi bir yatırım ve zaman ister. Bunun yanında şehir içinde elektrik tellerinden düzensiz ve birbirinden alakasız yapılanmaya kadar birçok engel drone'ların bozulmasına neden olur. Test aşamalarının sivil güvenliği dikkate alınarak yapılması ise apayrı bir zorluktur. Bu proje, fikir aşamasında olmakta olup yukarıdaki birçok riski önemli ölçüde azaltır ve birçok zorluğu daha hızlı çözüme kavuşturabilme kapasitesine sahiptir.

## Fikir

Projenin ana fikri, basit bir şekilde **"drone ile otel sahillerinde teslimat"** şeklinde açıklanabilir. Otel sahillerinde müşterilerin gıda taleplerini karşılayan büfe, market tarzı noktalar bulunur. Müşteriler sahilde eşyalarının olduğu yerden bu noktalara yürüyerek gider gelirler. Eğer bir drone ile dağıtım merkezi olsaydı ve ürünler büfeden müşterilerin şezlongta yattığı yere kadar teslim edilebilseydi bu gerçekten tatil konforunu ikiye katlardı diye düşünüyorum.

## Projenin Farklı Açılardan İncelenmesi

Şimdi proje hakkında temel bir bilgiye sahibiz ve birçok açıdan projenin artı ve eksilerini değerlendirebiliriz. Bu konuları şu şekilde sıralayabiliriz:

1. **Pazarlama:** Otel yönetimi neden bu projeyi istesin?
2. **Pazarlama:** Otel müşterilerinin drone hizmeti hakkındaki fikirleri ve talepleri
3. **Pazarlama:** Drone'ların ayrıca bir ürün olarak satılması yani _seri üretim_
4. **Test:** Drone'ların testi ve test için gerekli alan
5. **Teknik Yazılım:** Dağıtım ağını yönetmek için **Getir**, **Yemeksepeti** gibi bir platformun yazılması
6. **Seri Üretim:** Drone'lara bağlı ürünleri servis edecek ayrı bir robotik platform
7. **Teknik Problem:** Drone'ların müşterinin tam yanına gelmesi sorunu
8. **Teknik Problem:** Drone'ların otomatik güzergah çizmeleri ve büfeye geri dönmeleri
9. **Müşteri Segmenti:** Hangi müşteri segmentine (zengin, orta, fakir) hizmet sunulacağı

Bu alanları kendi başlıkları altında birer birer incelemeden önce ilerde lazım olabilecek bazı kavramlarının sunumu yapılmalıdır.

## Kavramlar

- **Fiyat Segmentasyonu:** Müşteriler veya ürünlerin alım gücü ve ücretlendirme kapsamında gruplara ayrılması
- - Yüksek, Orta, Düşük şeklinde 3 grupta incelenecektir.
- **Müşteri Segmentasyonu:** Müşterilerin alım gücüne göre gruplara ayrılması
- - Yüksek, Orta, Düşük (Zenginden fakire) şeklinde 3 grupta incelenecektir.
 
### 1. Pazarlama: Otel Yönetimi

Türkiye'de birçok otel bulunmakta ve her biri farklı müşteri segmentine hitap etmektedir ve hitap ettikleri müşteri segmentine göre otellerde birbirinden fiyat segmentlerine göre ayrılmaktadır.

Bu projenin yazılım platformu ve drone'larının tam hazır olduğu varsayılırsa ilk müşterimiz otel yönetimleri olacaktır. Bizim bu otel yönetimlerinden hangi segmentasyonu hedefleyeceğimiz ise kritik bir önem taşımaktadır. Bunu daha kolay anlaşılması için otel yönetimlerinin gözünden incelemekte fayda var:

1.1 **Otel Yönetimlerine Göre Projenin Reklam Kapasitesi**

        Otel yönetimi, projeyi bir reklam aracı olarak görüp kullanmak isteyebilir. bu durumda hem drone 
        sistemininin otele entegre edilmesi, bakımı gibi ücretleri karşılayıp hem de bunları kâra dönüştürmesi
        gereken otel müşteri çekmek için bu projeyi reklam aracı olarak kullanabilir. 
        Bu durumda drone'ların yoğun kullanılmasından çok reklam amacı gütmesi bizim açımızdan
        çok fark yaratır.

1.2 **Otel Yönetimlerine Göre Projenin Kâr Etme Kapasitesi**

        Otel yönetimi, projeyi kar elde etme aracı olarak görebilir ve yatırımını titizlikle yapar.
        Bu durumda drone'un sahillerde kullanılması bir ücretlendirmeye tâbi tutulacağından drone'ların 
        kullanım oranlarının yüksek olması için müşteri segmentinin yüksek olması gerekir.



### 2. Pazarlama: Otel Müşterileri


