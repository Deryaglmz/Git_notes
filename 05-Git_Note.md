# Git_notes
### git : Versiyon kontrol sistemidir . Özgür ve açık kaynaklı bir yazılımdır.
Git servis sağlayıcıları, örneğin GitHub veya GitLab, özel depolar oluşturma ve yönetme konusunda desteği sağlar. Bu servisler, kullanıcılara özel projeler oluşturma, kullanıcı izinlerini yönetme ve özel depoları koruma gibi işlevselliği sağlar.

### gitHub : Git tabanlı projelerin barındırıldığı, paylaşıldığı ve işbirliği yapılan bir bulut tabanlı platformdur. GitHub, açık kaynaklı topluluklar için önemli bir platformdur. Geliştiriciler, projelerini GitHub üzerinde paylaşarak geri bildirim alabilir, katkıda bulunabilir ve projeleri kolayca takip edebilirler.

### git fetch : uzaktaki bir Git deposundan güncel bilgileri almak için kullanılan bir Git komutudur. Bu komut, yerel depodaki bilgileri değiştirmeksizin, uzak depodaki güncel değişiklikleri kontrol etmenizi sağlar.
bazı yaygın kullanım senaryoları şunlardır:

                                   Uzak depodaki diğer kullanıcıların yaptığı değişiklikleri kontrol etmek ve güncellemeleri yerel depoya almak.
                                   
                                   Uzaktaki bir branch'i takip etmek ve onun güncel halini görmek, ancak yerelde mevcut bir çalışma kopyası oluşturmadan.
                                   
                                   Uzak depodaki değişiklikleri incelemek ve yerelde yapacağınız değişikliklere uyum sağlamak.

### git branch -r : Uzak depodaki tüm dalların listesini görüntülemek için kullanılan bir Git komutudur. "r" seçeneği, "remote" (uzak) anlamına gelir.


### git checkout :  komutu, Git deposunda farklı dallar arasında geçiş yapmak, belirli bir commit'i veya dosyayı kurtarmak, yeni bir dal oluşturmak veya mevcut bir dalı oluşturmak için kullanılan bir Git komutudur.
geçiş yapmak istediğiniz dal veya commit ile ilgili dosyaları günceller ve çalışma kopyasını değiştirir. Bu nedenle, dikkatlice kullanmanız önemlidir ve üzerinde çalıştığınız dosyaların kaydedildiğinden emin olmanız gerekmektedir.

#### Dal Değiştirme: git checkout branch_name
Bu komut, mevcut çalışma kopyasını branch_name adlı bir dala geçiş yapmak için kullanılır. Yapılan değişiklikler, belirtilen dalda yapılacak olanlarla değiştirilir.

#### Commit'e Geçiş: git checkout commit_hash
commit_hash parametresi, geçiş yapmak istediğiniz belirli bir commit'in benzersiz kimliğini temsil eder. Bu komutla, belirli bir geçmiş noktasına geçebilir ve bu noktadaki dosyaları görüntüleyebilirsiniz. Ancak bu durumda, dosyalar salt okunur olacak ve değişiklikleri doğrudan kaydedemezsiniz.

### Dosya Kurtarma: git checkout -- file_path
Bu komut, belirli bir dosyanın son kaydedilen hâline geri dönmenizi sağlar. Dosya adını ve yolunu belirtirken -- kullanarak, dosyanın Git tarafından takip edilen bir dosya olduğunu belirtirsiniz.

### Yeni Dal Oluşturma: git checkout -b new_branch_name
-b bayrağı, aynı anda yeni bir dal oluşturup o dala geçiş yapmanızı sağlar. Bu komut, bir dalı oluşturup üzerinde çalışmaya başlamak için sıklıkla kullanılır.
git checkout origin / master

### git push :  komutu, yerel bir Git deposundaki değişiklikleri uzak bir Git deposuna göndermek için kullanılır. Bu komut, yerelde yaptığınız değişiklikleri paylaşmanızı sağlar.
git push <remote> <branch>
<remote>, değişikliklerin gönderileceği uzak depoyu belirtir. Örneğin, origin genellikle varsayılan olarak kullanılan isimdir ve genellikle bir uzak depoyu temsil eder.
<branch>, göndermek istediğiniz yerel dalı temsil eder. Yapılan değişiklikler bu dala aitse, bu dalı uzak depoya göndermek için kullanılır.

git push komutunu kullanmadan önce, yereldeki değişiklikleri kaydettiğinizden ve commitlediğinizden emin olun. Aksi takdirde, push işlemi reddedilebilir.

git push komutu, yerel dal ile uzaktaki dal arasındaki farkları kontrol eder ve sadece farklılık olan dosyaları ve commitleri gönderir.

İlk kez push işlemi yaparken, uzak depoda aynı isimde bir dal oluşturulur ve yereldeki değişiklikler bu dalda saklanır. Daha sonraki push işlemleri, bu dal üzerindeki değişiklikleri günceller.
git push -u origin master

