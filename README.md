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

Projenin sunulabilmesi, ortaya çıkacak drone'un incelenebilmesi için yazılımından testlerine kadar her aşaması bitirilmiş bir prototip ürün geliştirilmelidir. Bu ürün, tam anlamınya seri üretime hazır, sürdürülebilir şekilde tasarlanmış olmalıdır.

1.1 **Drone**
> İlk olarak drone prototipi hazırlanmalıdır. Sırasıyla:

> * Drone'un temel iskeletinin nasıl elde edileceği belirlenmeli (Satın alınma veya sıfırdan üretim)

> * Eğer drone sıfırdan geliştirilecekse dış iskelet ve iç iskeletin ayrı ayrı tasarlanması ve ürettirilmesi gerekektedir.

> * Drone'un yazılımı geliştirilmelidir. Yazılım, uzaktan kumanda edilmesi, pist alanınının otonom şekilde tanınması, geliştirilecek yazılım ile bağlantının kurulması, uçarken otonom güzergâh belirleme ve müşteriye teslimatın sağlanması aşamalarının tamamını içermelidir.

1.2 **Teslimat Ünitesi**
> İkinci aşamada drone'a bağlı olan ve teslim edilecek ürünlerin taşınacağı bir teslimat ünitesi prototipi tam kullanıma hazır olacak şekilde üretilmelidir. Bu ünite üretilirken:

> * Ürünlerin teslimat sırasında sarsılmaması ve kırılmaması ve içeceklerin dökülmemesi,
> * Büfe çalışanının kolayca ürünleri yerleştirebilmesi,
> * Müşterinin ürünleri kolayca teslim alabilmesi,
> * ana yazılıma bağlanarak authentication işlemini yapabilmesi,
> * Yağmur, kar, kış gibi etkenlere dayanıklı olması

> gibi özelliklere sahip olmalıdır.
    

1.3 **Test**

> Bu raporda bahsedilen tüm bu teknik geliştirmelerin detaylıca test edilmesi çok önemlidir. Bu testler için bir alan gerekmektedir. Testlerin bolca tekrardan oluşması ve dolayısıyla uzun zaman süreceği de göz önüne alınmalıdır.

1.4 **Kritikler**

> Müşteri ürünü sipariş ettiğinde Drone GPS ile müşterinin yakınına gelebilir ancak GPS 
sinyalleri her zaman tam nokta belirtmez. Bu yüzden drone'un müşteriyi bulması gerekir. 
Bu noktada birkaç çözüm önerisi var:

> * Drone, müşterinin telefonundaki uygulama aracılığıyla manuel olarak müşteri
tarafından yönlendirilerek teslimat sağlanabilir. (Burada müşteri kaynaklı bir arıza veya kaza olması durumunda sıkıntı oluşabilir)
> * Drone, yapay zeka ile müşterinin yüzünü tanıyarak ürün teslimatını yapabilir.
> * Drone, müşteriye otel girişinde verilecek bilekliklerde bulunan bir sensör 
sayesinde müşteriyi bulabilir. (bunun en büyük dezavantajı otel dışında kullanıma
uygun olmamasıdır)

> Drone'ların şarj olacakları ve siparişleri teslim alabilecekleri bir piste ihtiyaç duyulacaktır.

> * Pist, yağmur, rüzgar, kar gibi etkenlere karşı korunaklı olmalıdır.
> * Pist, büfe'deki çalışanların kolaylıkla ulaşabileceği yakınlıkta olmalıdır. (Bu, müşteri yoğunluğunun çok olduğu dönemlerde oldukça önem arz edecektir)
> * Pist, şarj istasyonlarına uygun tasarlanmalıdır.
> * Drone'lar otonom olarak pisti bulabilmeli ve otonoö şekilde piste iniş kalkış yapabilmelidir.

---

### 2. Yazılım

Ana Platform:

> Müşterilerin ürün siparişi vermeleri, drone'lara emir gitmesi, siparişin teslim edilmesi, iade, müşteri hizmetleri gibi süreçleri yönetmek ve müşteriye kolaylık sağlamak için **Getir**, **Yemeksepeti** gibi bir platform geliştirilecektir. Bu platformun sürdürülebilir olması, ölçeklendirmeye uygun olması için backend tarafında kullanılacak mimarinin kapsamlı bir değerlendirmeden sonra seçilmesi gerekmektedir.

Drone'lara Gömülü Yazılım:
> 

---

### 3. Üretim
Projede kullanılacak drone'ları 3. parti bir satıcıdan mı alacağız yoksa kendimiz mi üreteceğiz? Bu konunun ayrıntılı konuşulması gerekmektedir.
Teslimat ünitesi ise ayrı bir konu

---

### 4. Pazarlama
Türkiye'de birçok otel bulunmakta ve her biri farklı müşteri segmentine hitap etmektedir ve hitap ettikleri müşteri segmentine göre otellerde birbirinden fiyat segmentlerine göre ayrılmaktadır.

Bu projenin yazılım platformu ve drone'larının tam hazır olduğu varsayılırsa ilk müşterimiz otel yönetimleri olacaktır. Bizim bu otel yönetimlerinden hangi segmentasyonu hedefleyeceğimiz ise kritik bir önem taşımaktadır. Bunu daha kolay anlaşılması için otel yönetimlerinin gözünden incelemekte fayda var:

1.1 **Projenin Yeni Müşteriler Kazandırma Potansiyeli**

> Oteller müşteri çekebilmek için farklı reklam stratejileri izleyebilirler. Bu durumda bizim projemiz bir reklam aracı olarak kullanılabilir. Örneğin "Drone ile Ayağınıza Teslimat" gibi reklam kampanyaları ile daha fazla müşteri toplama yoluna gidilebilir.

1.2 **Projenin Otel Satışlarını ve Karlılığını Artırma Potansiyeli**

> Otel, projeyi kar elde etme aracı olarak görebilir ve yatırımını titizlikle yapar. Bu durumda drone'un sahillerde kullanılması bir ücretlendirmeye tâbi tutulacağından drone'ların kullanım oranlarının yüksek olması için müşteri segmentinin yüksek olması gerekir. Yani eğer otel yüksek fiyat segmentli ise yüksek ihtimalle bu yolu kullanarak kâr elde edecektir.

Başka bir açıdan incelendiğinde proje sadece kendisini pazarlama aracı olarak kullanmaz. Drone'ların otellere satılması, satış sonrası servisler de bu işin bir başka ekonomik boyutunu ve kâr elde etme yolunu bize gösterir.

---

### 5. Satış Sonrası Servis
Drone'ların seri üretimden çıkıp satıldıktan sonra devamlı bakım ve onarımlarının yapılması gerekir. Bu noktada ciddi bir yatırım gerekecektir.
Seri üretimle birlikle **bakım hizmeti**, başlı başına ayrı bir **"iş bölümü"** ihtiyacı anlamına da geliyor.

---

### 6. Projenin Gelecekteki Seyri
1. Proje, doğası gereği drone'ları tam hakimiyet ile yönetebilmeyi gerektirmektedir. Bu beceriye sahip bir işletme ise yeni sahillere açılabilme ve işi büyütebilme avantajına sahiptir. Sadece Türkiye'de bir sürü sahil bulunmakta ve bu da bir sürü müşteri anlamına gelmektedir.

2. Drone'lar, başarılı testler sonucunda şehir içi teslimat için de kullanılabilir. Proje, ileride bu yönde de genişleme gösterebilecek bir potansiyele sahiptir.
