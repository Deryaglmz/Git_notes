# Git_notes
### git pull (git fetch + git merge) :  komutu, yerel bir Git deposundaki çalışma kopyasını ve geçerli dalı güncellemek için kullanılır. Bu komut, uzak depodaki en son değişiklikleri alır ve mevcut yerel dalınızı bu güncellemelerle birleştirir.
#### git pull remote branch
#### remote : güncellemelerin alınacağı uzak depoyu belirtir. Örneğin, origin genellikle varsayılan olarak kullanılan isimdir ve genellikle bir uzak depoyu temsil eder.

#### branch : güncellemelerin alınacağı uzak dalı belirtir. Bu, güncelleme yapmak istediğiniz dalı temsil eder.

git pull komutu, aslında git fetch ve ardından git merge komutlarını otomatik olarak gerçekleştirir. İlk olarak, git fetch komutu ile uzak depodaki güncel bilgileri alır ve ardından yerel dalınız ile uzaktaki dal arasında birleştirme işlemi yapar.
git pull komutunu kullanırken, yereldeki değişikliklerinizi kaydedip commitlediğinizden emin olun. Çünkü birleştirme işlemi, yereldeki değişiklikleri geçersiz kılabilir.
Uzak depodaki değişiklikler, yerelde yapılan değişikliklerle çakışabilir. Bu durumda, Git çakışan değişiklikleri belirtir ve çakışmayı çözmeniz gerekebilir.
git pull origin master

### NOT : git fetch komutu, git pull komutundan farklıdır. git pull komutu, git fetch komutunu çağırır ve ardından otomatik olarak mevcut branch ile uzaktaki branch arasında birleştirme işlemi yapar. Bu nedenle, git fetch komutunu kullanarak güncel bilgileri alıp, ardından birleştirme işlemi için ayrıca git merge veya git rebase gibi komutları kullanmanız gerekebilir.

### git clone : git clone, bir uzak Git deposundan bir kopya oluşturmak için kullanılan bir Git komutudur. Bu komut, uzak depodaki tüm dosyaları ve geçmişi alarak tam bir kopya oluşturur. git clone komutu, bir Git deposunu tamamen indirir ve tüm geçmiş, dallar ve dosyaları kopyalar. Bu şekilde, başka birisinin sahip olduğu bir depoyu kendi çalışma ortamınıza getirebilir ve değişiklikler yapmaya başlayabilirsiniz.

#### git clone <repository_url> <destination_directory>

### repository_url : kopyalanacak uzak Git deposunun URL'sini belirtir. Bu genellikle bir HTTPS veya SSH bağlantısıdır.

### destination_directory : kopyanın yerel sistemde hangi dizine yerleştirileceğini belirtir. İsteğe bağlı olarak belirtilebilir. Belirtilmezse, uzak depodaki deposunun adıyla aynı bir dizin oluşturulur ve kopya bu dizine yerleştirilir.

### fork : Git'te "fork", bir Git deposunun kopyasını almak ve bu kopyayı kendi hesabınız altında yönetmek için kullanılan bir işlemdir.

Fork işlemi, başka birisinin sahip olduğu bir depoyu kendi hesabınıza almanızı ve bu depoyu bağımsız olarak düzenleyebilmenizi sağlar.

Fork işlemi genellikle açık kaynak projelerinde ve işbirliği projelerinde kullanılır.

Başka birisinin depo projesine katkıda bulunmak veya değişiklik yapmak istediğinizde, önce o depoyu kendi hesabınıza fork edersiniz. Bu, sizin kişisel bir kopyanızı oluşturur ve bu kopya üzerinde istediğiniz değişiklikleri yapabilirsiniz.

Fork edilen depo, sizin hesabınız altında bir bağımsız projeyi temsil eder.

Fork işlemi ile elde ettiğiniz kopya depo, sizin kontrolünüz altındadır. 

Bu kopya depoyu, kendi hesabınızda değişiklik yapmak, yeni branch'ler oluşturmak, commit'ler yapmak ve bunları yayınlamak gibi işlemleri gerçekleştirebilirsiniz.
Ayrıca, fork edilen depoyu istediğiniz şekilde güncelleyebilir ve geliştirebilirsiniz.

Fork edilen depoda yaptığınız değişiklikleri ana depoya entegre etmek isterseniz, bir "pull request" (çekme isteği) göndererek değişikliklerin orijinal depoya entegre edilmesini talep edebilirsiniz. Ana depo sahibi bu talebi değerlendirir ve değişikliklerin ana depoya entegre edilip edilmeyeceğine karar verir.

Fork işlemi, katkıda bulunma ve işbirliği yapma sürecinde önemli bir adımdır. Fork işlemi sayesinde başka projelerle etkileşime geçebilir, değişiklik yapabilir ve projelere katkıda bulunabilirsiniz.

### private : Git'te "private" (özel) özelliği, bir Git deposunun gizlilik seviyesini belirtmek için kullanılır. Bir depo özel olarak ayarlandığında, sadece depo sahibi ve gerekli izinlere sahip olanlar tarafından erişilebilir ve görüntülenebilir. Diğer kullanıcılar veya herkese açık bir şekilde depoya erişemezler.
private özelliği, özellikle hassas veya ticari bilgilere sahip projelerde projenin güvenliğini ve gizliliğini sağlamak için önemlidir. Böylece, yalnızca yetkili kullanıcılar projeye erişebilir ve projenin içeriği korunmuş olur.


