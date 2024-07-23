 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
    </a> 
    <br> ATM Application <br>
Bu kod, bir ATM simülasyonunu JavaScript kullanarak oluşturuyor. Kullanıcıların bakiye görüntüleme, para çekme, para yatırma, kredi çekme ve çıkış işlemlerini gerçekleştirebileceği bir program sunuyor. İşte kodun detaylı açıklaması:

Değişken Tanımlamaları
yenisatırr: Satır sonu karakteri (\r\n), yeni bir satıra geçişi sağlar.
kredisınırı: Kredi çekme limiti, 100000 TL olarak belirlenmiş.
atmbakiye: ATM'deki başlangıç bakiyesi, 1000 TL olarak belirlenmiş.
yatırmasınırı: Günlük para yatırma limiti, 10000 TL olarak belirlenmiş.
atmmetin: Kullanıcıya sunulacak olan ATM menü metni.
Menü ve Kullanıcı Seçimi
Kullanıcıya aşağıdaki seçenekler sunuluyor:

Bakiye görüntüleme
Para çekme
Para yatırma
Kredi çekme
Çıkış
Kullanıcı bu seçeneklerden birini seçer ve switch ifadesi ile seçime göre ilgili işlem gerçekleştirilir.

İşlem Açıklamaları
1. Bakiye Görüntüleme
Kullanıcı "1" seçerse, mevcut ATM bakiyesi (atmbakiye) kullanıcıya gösterilir.
2. Para Çekme
Kullanıcı "2" seçerse, çekmek istediği tutar sorulur.
Eğer çekilecek tutar mevcut bakiyeden küçükse, işlem gerçekleştirilir ve yeni bakiye hesaplanarak kullanıcıya bildirilir.
Eğer çekilecek tutar mevcut bakiyeden büyükse, işlem reddedilir ve kullanıcıya yetersiz bakiye uyarısı yapılır.
3. Para Yatırma
Kullanıcı "3" seçerse, yatırmak istediği tutar sorulur.
Eğer yatırılacak tutar günlük yatırma sınırından (yatırmasınırı) büyükse, işlem reddedilir ve kullanıcıya günlük limit uyarısı yapılır.
Eğer yatırılacak tutar uygun ise, tutar mevcut bakiyeye eklenir ve güncel bakiye kullanıcıya bildirilir.
4. Kredi Çekme
Kullanıcı "4" seçerse, çekmek istediği kredi miktarı sorulur.
Eğer çekilecek kredi tutarı kredi sınırından (kredisınırı) büyükse, işlem reddedilir ve kullanıcıya limit uyarısı yapılır.
Eğer kredi tutarı uygun ise, kredi çekme işlemi onaylanır ve kullanıcıya bildirilir.
5. Çıkış
Kullanıcı "5" seçerse, programdan çıkış işlemi yapılır ve kullanıcıya çıkış mesajı gösterilir.
Hatalı Giriş
Kullanıcı geçersiz bir seçenek girerse, kullanıcıya geçerli bir işlem seçmesi gerektiği bildirilir.
Bu yapı, kullanıcıların çeşitli ATM işlemlerini simüle etmelerini sağlar ve temel bankacılık işlemlerini gerçekleştirmek için kullanılabilir.

 <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> 
    </a> 
    <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> 
    </a> 
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
    </a> 
<br>Clock<br>

Bu kod, web sayfasında hem dijital hem de analog bir saat oluşturur. İşte adım adım açıklaması:

HTML Yapısı:

<!DOCTYPE html> ve diğer temel HTML etiketleri kullanılarak bir HTML belgesi tanımlanır.
#clock-container adlı bir div, hem dijital hem de analog saati içerecek şekilde yerleştirilir.
#digital-clock adlı bir div, dijital saat için ayrılmıştır.
#analog-clock adlı bir div, analog saat için ayrılmıştır. Bu divin içinde saat, dakika ve saniye göstergelerini temsil eden üç div daha bulunur (#hour-hand, #minute-hand, #second-hand).
CSS Stilleri:

body etiketi, sayfanın ortasında saatlerin yer almasını sağlayacak şekilde stillendirilmiştir.
#clock-container, saatlerin ortalanması için metin hizalaması yapılmıştır.
Dijital saat (#digital-clock) için font boyutu ve alt marj ayarlanmıştır.
Analog saat göstergeleri (#hour-hand, #minute-hand, #second-hand) için boyut, renk ve konum stilleri tanımlanmıştır.
JavaScript:

updateTime fonksiyonu, saati güncellemek için kullanılır. Bu fonksiyon her saniyede bir çalışacak şekilde ayarlanmıştır.
updateTime fonksiyonunda:
Date nesnesi kullanılarak mevcut zaman alınır.
Dijital saat için, #digital-clock divinin içeriği mevcut zamanla güncellenir.
Analog saat için, saat, dakika ve saniye değerleri hesaplanarak uygun açıya döndürülür ve bu değerler saat, dakika ve saniye göstergelerine uygulanır (rotate CSS özelliği kullanılarak).
Zamanın Güncellenmesi:

setInterval fonksiyonu, updateTime fonksiyonunun her saniye çalışmasını sağlar.
Sayfa yüklendiğinde updateTime fonksiyonu hemen çalıştırılarak saatlerin anında görüntülenmesi sağlanır.
Sonuç olarak, bu kod bir web sayfasında hem dijital hem de analog bir saatin gerçek zamanlı olarak gösterilmesini sağlar. Dijital saat, mevcut zamanı metin olarak gösterirken, analog saat göstergeleri saniye, dakika ve saat ibreleri ile görselleştirilir.








