 <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> 
    </a> 
    <br>
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







