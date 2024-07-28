# Otellerde Drone ile Teslimat Projesi

## Giriş
Günümüzde drone'lar ile yapılan ve bazı ülkelerde testleri halen sürmekte olan
birçok proje mevcut. Bu projelerin birçoğu şehir içinde kargo, yemek, içecek, gıda ürünleri vb. gibi ürünleri teslimat için tasarlanmıştır. Bu konseptte drone projelerinin gelişimi ve test aşamaları oldukça zor ve maliyetlidir. Drone'ların bakımı, satın alınıp modifiye edilmesi, gömülü yazılımları ve eğer varsa yapay zeka modellerini üretmek zaten ciddi bir yatırım ve zaman ister. Bunun yanında şehir içinde elektrik tellerinden düzensiz ve birbirinden alakasız yapılanmaya kadar birçok engel drone'ların bozulmasına neden olur. Test aşamalarının sivil güvenliği dikkate alınarak yapılması ise apayrı bir zorluktur. Bu proje, fikir aşamasında olmakta olup yukarıdaki birçok riski önemli ölçüde azaltır ve birçok zorluğu daha hızlı çözüme kavuşturabilme kapasitesine sahiptir.

## Fikir
Projenin ana fikri, basit bir şekilde **"drone ile otel sahillerinde teslimat"** şeklinde açıklanabilir. Otel sahillerinde müşterilerin gıda taleplerini karşılayan büfe, market tarzı noktalar bulunur. Müşteriler sahilde eşyalarının olduğu yerden bu noktalara yürüyerek gider gelirler. Eğer bir drone ile dağıtım merkezi olsaydı ve ürünler büfeden müşterilerin şezlongta yattığı yere kadar teslim edilebilseydi bu gerçekten tatil konforunu ikiye katlardı diye düşünüyorum.

## Projenin Farklı Açılardan İncelenmesi
Şimdi proje hakkında temel bir bilgiye sahibiz ve birçok açıdan projenin artı ve eksilerini değerlendirebiliriz. Bu konuları şu şekilde sıralayabiliriz:

Projenin teknik tarafı bittikten sonra:
1. **Pazarlama:** Otel yönetimi ve müşterilerinin drone hizmeti hakkındaki fikirleri ve talepleri
2. **Seri Üretim:** Drone'lara bağlı ürünleri servis edecek ayrı bir robotik platform
3. **Bakım:**: Droneların bakımı için ayrı bir iş bölümü

Projenin teknik tarafı:
4. **Drone İmalatı:** Drone sıfırdan mı üretilecek yoksa satın mı alınacak?
5. **Teknik Yazılım:** Dağıtım ağını yönetmek için **Getir**, **Yemeksepeti** gibi bir platformun yazılması
6. **Teknik Problem:** Drone'ların müşterinin tam yanına gelmesi sorunu
7. **Teknik Problem:** Drone'ların pisti ve şarjı
8. **Test:** Drone'ların testi ve test için gerekli alan

İleriye Dönük:
9. **Projenin gelecekteki seyri:** Proje tamamlandıktan sonra nereye, nasıl evrilebilir?


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



### 2. Pazarlama: Seri Üretim
Bu projenin bize getireceği ikinci önemli sorumluluk ise tıpkı bir drone satıcısı gibi drone'ları pazarlayacağımız gerçeği. Bu projeyi sadece bir **"proje"** olarak değil aynı zamanda drone tacirliği gibi de ele almak gerekir. Projenin fikrini ayrı, drone'ların kendilerini ayrı pazarlamak gerekecektir. Seri üretimle birlikle çok önemli bir **bakım hizmeti** de sunulması gerekir ve bu başlı başına ayrı bir iş bölümü ihtiyacı anlamına geliyor.

### 3. Bakım: Droneların Bakımı
Drone'ların seri üretimden çıkıp satıldıktan sonra devamlı bakım ve onarımlarının yapılması gerekir. Bu noktada ciddi bir yatırım ve iş bölümü daha açılması gerekir.

### 4. Drone İmalatı: Drone Nasıl İmal Edilecek?
Projede kullanılacak drone'ları 3. parti bir satıcıdan mı alacağız yoksa kendimiz mi üreteceğiz? Bu konunun ayrıntılı konuşulması gerekmektedir.

### 5. Teknik Yazılım: Dağıtım Ağı Platformu
Müşterilerin sipariş etmesi, drone'lara emir gitmesi, siparişin teslim edilmesi, iade, müşteri hizmetleri gibi süreçleri yönetmek ve müşteriye kolaylık sağlamak için **Getir**, **Yemeksepeti** gibi bir platform geliştirilecektir. Bu platformun sürdürülebilir olması, ölçeklendirmeye uygun olması için backend tarafında kullanılacak mimarinin kapsamlı bir değerlendirmeden sonra seçilmesi gerekmektedir.

### 6. Teknik Problem: Drone'ların Müşterinin Tam Yanına Gelmesi
Müşteri ürünü sipariş ettiğinde Drone GPS ile müşterinin yakınına gelebilir ancak GPS sinyalleri her zaman tam nokta belirtmez. Bu yüzden drone'un müşteriyi bulması gerekir. Bu noktada birkaç çözüm önerisi var:

- Drone, müşteri tarafından telefonundaki platform aracılığıyla kontrol edilebilir.
- Drone, yapay zeka ile müşterinin yüzünü tanıyabilir (Diplomasik sorunlara neden olabilir)
- Drone, müşteriye otel girişinde verilecek bilekliklerde bulunan bir sensör sayesinde müşteriyi bulabilir

### 7. Teknik Problem: Drone'ların Pisti
Drone'ların dağıtım esnasında şarj olacakları ve siparişleri alacakları bir pistinin olması gerekmektedir. 

- Bu pist, yağmur, rüzgar, kar gibi etkenlere karşı korunaklı olmalıdır
- Pist, büfe'deki çalışanların kolaylıkla ulaşabileceği yakınlıkta olmalıdır (Bu, müşteri yoğunluğunun çok     olduğu dönemlerde oldukça önem arz edecektir)
- Pist, şarj istasyonlarına uygun tasarlanmalıdır
- Drone'ların otomatik pisti tanımaları ve giriş yapıp park etmeleri gerekir
- Drone'lar pistten güvenle otomatik çıkış yapıp müşteriye gitmelidir

### 8. Test: Drone'ların Testi ve Test İçin Alan
Bu raporda bahsedilen tüm bu teknik geliştirmelerin test edilmesi çok önemlidir. Bunun için test alanı, test uzmanı (test alanında tecrübeli) kişi ve bolca zaman gerekmektedir.
