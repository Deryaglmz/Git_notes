# Git_notes
### git checkout : Git deposunda çalışırken farklı dallar arasında geçiş yapmak, dosyalarda geri alma işlemleri yapmak veya geçmişteki durumlara erişmek gibi durumlar için bu komutu kullanırız.

### git reset : istediğin committen itibaren üsttekileri silmek , değişiklikleri geri almak, geçmişi değiştirmek için kullanılır.

### git reset --hard : geçmişi ve çalışma dizinindeki dosyaları , içerikleri tamamen siler. 

### git revet <commit> :  belirtilen bir commiti geri almak için kullanılır. geri alma işlemini yeni bir commit oluşturarak yapılır .geri alınan commit etkisi hala geçerli bir geçmişte kalırken, yeni bir commit eklenir.

### git diff : belli başlı yerlerdeki ( commit , branch ,dosya ) bunlar arasındaki farkları gösterir. 

### git diff HEAD : son commite göre neleri değiştirdik onu gösterir.
#### HEAD(son commiti ifade eder) 

### git diff : iki commit arasındaki farkları gösterir. (İki commit , branch)

### merge commit (birleştirme commit'i) :  iki veya daha fazla dalın farklı noktalardaki değişikliklerini birleştiren özel bir commit'tir. 

### git rebase master : Rebase işlemi, mevcut dalınızın temel aldığınız dalın en son durumu ile "yeniden tabanlama" anlamına gelir. Bu, mevcut dalınızın temel dalını (genellikle "master" dalını) takip etmesini sağlar. Yeniden tabanlama, projenin geçmişini düzgün ve sade tutmaya yardımcı olur, çünkü rebase işlemi birleştirme commit'lerini yeniden uygulayarak temiz bir tarihçe oluşturur. Eğer paylaşılan bir dala rebase işlemi uygularsanız, geçmişteki commitlerinizi değiştirirsiniz ve başkalarının çalışmalarını etkileyebilirsiniz.
                 git checkout feature-branch: Öncelikle, yeniden tabanlamak istediğiniz dalı seçin (örneğin, "feature-branch").
                 git rebase master: Ardından, git rebase komutunu kullanarak mevcut dalınızı "master" dalının en son durumu üzerine yeniden tabanlayın.
### NOT : Rebase işlemi, birleştirme (merge) işleminden farklıdır. Rebase, birleştirme taahhütlerini yeniden uygulayarak bir dalın geçmişini yeniden şekillendirirken, birleştirme işlemi ise ayrı bir birleştirme commit'i oluşturarak iki dala yapılan değişiklikleri birleştirir.

