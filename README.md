# Sahillerde Drone ile Teslimat Projesi

## Giriş
Günümüzde drone'lar ile yapılan ve bazı ülkelerde testleri halen sürmekte olan
birçok proje mevcut. Bu projelerin birçoğu şehir içinde kargo, yemek, içecek, gıda ürünleri vb. gibi ürünleri teslimat için tasarlanmıştır. Bu konseptte drone projelerinin gelişimi ve test aşamaları oldukça zor ve maliyetlidir. Drone'ların bakımı, satın alınıp modifiye edilmesi, gömülü yazılımları ve eğer varsa yapay zeka modellerini üretmek zaten ciddi bir yatırım ve zaman ister. Bunun yanında şehir içinde elektrik tellerinden düzensiz ve birbirinden alakasız yapılanmaya kadar birçok engel drone'ların bozulmasına neden olur. Test aşamalarının sivil güvenliği dikkate alınarak yapılması ise apayrı bir zorluktur. Bu proje, fikir aşamasında olmakta olup yukarıdaki birçok riski önemli ölçüde azaltır ve birçok zorluğu daha hızlı çözüme kavuşturabilme kapasitesine sahiptir.

## Fikir
Projenin ana fikri, basit bir şekilde **"drone ile otel sahillerinde teslimat"** şeklinde açıklanabilir. Otel sahillerinde müşterilerin gıda taleplerini karşılayan büfe, market tarzı noktalar bulunur. Müşteriler sahilde eşyalarının olduğu yerden bu noktalara yürüyerek gider gelirler. Eğer bir drone ile dağıtım merkezi olsaydı ve ürünler büfeden müşterilerin şezlongta yattığı yere kadar teslim edilebilseydi bu gerçekten tatil konforunu ikiye katlardı diye düşünüyorum.

## Başlıklar
1. **Prototip Üretim**
    * Drone
    * Teslimat Ünitesi
    * Test
    * Kritikler
2. **Yazılım**
3. **Üretim**
4. **Pazarlama**
5. **Satış Sonrası Servis**
6. **Projenin gelecekteki seyri**

---

### 1. Prototip Üretim

1.1 **Drone**

    

1.2 **Teslimat Ünitesi**

    

1.3 **Test**

    Bu raporda bahsedilen tüm bu teknik geliştirmelerin test edilmesi çok önemlidir. 
    Bunun için test alanı, test uzmanı (test alanında tecrübeli) kişi ve bolca zaman gerekmektedir.

1.4 **Kritikler**

    Müşteri ürünü sipariş ettiğinde Drone GPS ile müşterinin yakınına gelebilir ancak GPS 
    sinyalleri her zaman tam nokta belirtmez. Bu yüzden drone'un müşteriyi bulması gerekir. 
    Bu noktada birkaç çözüm önerisi var:

    - Drone, müşterinin telefonundaki uygulama aracılığıyla manuel olarak müşteri
    tarafından yönlendirilerek teslimat sağlanabilir.
    - Drone, yapay zeka ile müşterinin yüzünü tanıyarak ürün teslimatını yapabilir
    - Drone, müşteriye otel girişinde verilecek bilekliklerde bulunan bir sensör 
    sayesinde müşteriyi bulabilir ( bunun en büyük dezavantajı otel dışında kullanıma
    uygun olmamasıdır )

    Drone'ların şarj olacakları ve siparişleri teslim alabilecekleri bir pist alanına
    ihtiyaç duyulacaktır. 

    - Pist, yağmur, rüzgar, kar gibi etkenlere karşı korunaklı olmalıdır
    - Pist, büfe'deki çalışanların kolaylıkla ulaşabileceği yakınlıkta olmalıdır (Bu, müşteri yoğunluğunun çok olduğu dönemlerde oldukça önem arz edecektir)
    - Pist, şarj istasyonlarına uygun tasarlanmalıdır
    - Drone'lar otonom olarak pisti bulabilmeli ve otonoö şekilde piste iniş kalkış yapabilmelidir

---

### 2. Yazılım
Müşterilerin ürün siparişi vermeleri, drone'lara emir gitmesi, siparişin teslim edilmesi, iade, müşteri hizmetleri gibi süreçleri yönetmek ve müşteriye kolaylık sağlamak için **Getir**, **Yemeksepeti** gibi bir platform geliştirilecektir. Bu platformun sürdürülebilir olması, ölçeklendirmeye uygun olması için backend tarafında kullanılacak mimarinin kapsamlı bir değerlendirmeden sonra seçilmesi gerekmektedir.

---

### 3. Üretim
Projede kullanılacak drone'ları 3. parti bir satıcıdan mı alacağız yoksa kendimiz mi üreteceğiz? Bu konunun ayrıntılı konuşulması gerekmektedir.
Teslimat ünitesi ise ayrı bir konu

---

### 4. Pazarlama
Türkiye'de birçok otel bulunmakta ve her biri farklı müşteri segmentine hitap etmektedir ve hitap ettikleri müşteri segmentine göre otellerde birbirinden fiyat segmentlerine göre ayrılmaktadır.

Bu projenin yazılım platformu ve drone'larının tam hazır olduğu varsayılırsa ilk müşterimiz otel yönetimleri olacaktır. Bizim bu otel yönetimlerinden hangi segmentasyonu hedefleyeceğimiz ise kritik bir önem taşımaktadır. Bunu daha kolay anlaşılması için otel yönetimlerinin gözünden incelemekte fayda var:

1.1 **Projenin Yeni Müşteriler Kazandırma Potansiyeli**

        Otel yönetimi, projeyi bir reklam aracı olarak görüp kullanmak isteyebilir. bu durumda hem drone 
        sistemininin otele entegre edilmesi, bakımı gibi ücretleri karşılayıp hem de bunları kâra dönüştürmesi
        gereken otel müşteri çekmek için bu projeyi reklam aracı olarak kullanabilir. 

1.2 **Projenin Otel Satışlarını ve Karlılığı Artırma Kapasitesi**

        Otel yönetimi, projeyi kar elde etme aracı olarak görebilir ve yatırımını titizlikle yapar.
        Bu durumda drone'un sahillerde kullanılması bir ücretlendirmeye tâbi tutulacağından drone'ların 
        kullanım oranlarının yüksek olması için müşteri segmentinin yüksek olması gerekir.

Bu projenin bize getireceği ikinci önemli sorumluluk ise tıpkı bir drone satıcısı gibi drone'ları pazarlayacağımız gerçeği. Bu projeyi sadece bir **"proje"** olarak değil aynı zamanda drone tacirliği gibi de ele almak gerekir.

---

### 5. Satış Sonrası Servis
Drone'ların seri üretimden çıkıp satıldıktan sonra devamlı bakım ve onarımlarının yapılması gerekir. Bu noktada ciddi bir yatırım ve iş bölümü daha açılması gerekir.
Seri üretimle birlikle çok önemli bir **bakım hizmeti** de sunulması gerekir ve bu başlı başına ayrı bir iş bölümü ihtiyacı anlamına geliyor.

---

### 6. Projenin Gelecekteki Seyri