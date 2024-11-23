# aygaz_veri_analizi_bootcamp_projesi

  Veri Bilimi LinkedIn İş İlanları Veri Seti: Analiz ve Bulgular

  Bu veri seti, LinkedIn üzerinden toplanan ve Veri Bilimi alanındaki iş ilanlarını içeren önemli bir kaynaktır. İlanlar; iş unvanları, şirket isimleri, iş yerleri, iş bağlantıları, ilanların ilk görünüş tarihi, şehir ve ülke bilgileri, iş seviyeleri, iş türleri, iş özetleri ve gerekli iş becerileri gibi önemli bilgileri kapsamaktadır. Bu veri setine Kaggle üzerinden aşağıdaki bağlantıyı takip ederek erişebilirsiniz.

Veri Bilimi LinkedIn İş İlanları Veri Seti: https://www.kaggle.com/code/salihanur/proje2
### Değişkenler
- **job_title**: İş unvanı, her iş ilanının başlığını belirtir.
- **company**: İlanı yayınlayan şirketin adı.
- **job_location**: İşin fiziksel veya uzaktan çalışma koşullarını belirten konum bilgisi.
- **job_link**: İlgili iş ilanına doğrudan bağlantı.
- **first_seen**: İş ilanının LinkedIn'de ilk göründüğü tarih.
- **search_city**: Arama yapılan şehir bilgisi.
- **search_country**: Arama yapılan ülke bilgisi.
- **job level**: İşin seviyesi (örneğin, junior, senior, vs.).
- **job_type**: İş türü (tam zamanlı, yarı zamanlı, sözleşmeli, vs.).
- **job_summary**: İş ilanının kısa özeti.
- **job_skills**: İş için gerekli beceriler.

### Temel Bulgular ve İşlemler
Veri seti toplamda **10 sütun** ve **800 iş ilanı** içermektedir. 'job_level' ve 'job_type' gibi sütunlar kategorik, geri kalan değişkenler ise sayısal verilerdir. Veri setinin temel işleme adımlarında:
- **'job_title'** sütunu, iş ilanlarının unvanlarını içermektedir ve bazı iş unvanları birden fazla pozisyonu gösterecek şekilde virgüllerle ayrılmaktadır. Bu sütunda yapılan patlatma işlemi ile her bir iş unvanı ayrı bir satır olarak ele alınmıştır.
- **'job_skills'** sütununda, her bir iş ilanı için gerekli beceriler virgüllerle ayrılmıştır. Bu beceriler de patlatılarak sıklıkları analiz edilmiştir.

#### Başlıca Bulgular:
- **En Talep Edilen İş Unvanları**: Veri bilimcisi, veri analisti ve makine öğrenimi mühendisliği gibi iş unvanlarının sıklığına bakıldığında, **Veri Bilimci** unvanı en fazla tercih edilen iş unvanı olarak öne çıkmaktadır.
- **Gerekli Beceri Seti**: En çok talep edilen beceriler arasında **Python, SQL, ve makine öğrenimi algoritmaları** yer almaktadır. Bu becerilerin sıklığına bakıldığında, Python'un veri bilimindeki önemi açıkça görülmektedir.
- **İş Türü ve Seviyesi Dağılımı**: Çoğu ilan, **tam zamanlı** iş türünde ve genellikle **orta düzey** ve **senior** seviyelerinde açılmıştır. İş türleri açısından, çok sayıda sözleşmeli pozisyon da yer almaktadır.

### Diğer Analizler:
- **İş Türlerine Göre İş Düzeyi**: İlanlar, iş türüne göre gruplandığında, **tam zamanlı** pozisyonların genellikle daha yüksek seviyelerde açıldığı gözlemlenmiştir.
- **Şirket ve Konum Dağılımı**: Çoğu iş ilanı **ABD**'de yer almaktadır ve büyük teknoloji şirketlerinden çoğu pozisyonu açmaktadır.
  
### Modelleme ve Performans:
  Veri setinde yapılan analizlere ek olarak, **makine öğrenimi modelleri** kurarak iş ilanlarını sınıflandırmak için denemeler yapılmıştır. Bu modellerde:
- **Doğruluk oranı** genel olarak **%95** seviyelerinde olmuştur.

### Sonuç ve Öneriler:
  Veri Bilimi alanında, iş ilanları ve gereken beceriler hakkında yapılan bu analiz, veri bilimcilerin hangi becerilere sahip olmaları gerektiği ve hangi seviyede iş ilanlarının yoğunlukla yayımlandığı hakkında önemli bilgiler sunmaktadır. Veri setindeki dengesiz dağılımlar ve eksik veri setlerinden ötürü, daha fazla jenerasyon ve veri ekleyerek modelin doğruluğu artırılabilir.

  Bu çalışma, iş gücü pazarındaki eğilimleri analiz etmek ve iş arayanlar için stratejik kararlar almak açısından faydalı olabilecek bir temel oluşturur.

  Saliha Nur Çelik
