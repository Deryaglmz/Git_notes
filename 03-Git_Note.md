# Git_notes
### merge conflict (birleştirme çakışması)  :iki veya daha fazla kullanıcı aynı dosyanın aynı satırında farklı değişiklikler yaparsa veya aynı dosyanın farklı isimlendirilmiş bir kopyasını eklerse bir merge conflict meydana gelebilir. git  çakışmaları kullanıcıya sunar ve kullanıcının çakışmayı çözmesi için müdahale etmesi gerekmektedir. 

### stash (sakalmak, depolamak): ayrı bir yerde git bunları saklar istediğin zaman geri alabilirsin. Git'te "stash" (saklama) işlemi, geçici olarak çalışma dizinizdeki değişiklikleri kaydetmenize ve daha sonra geri getirmenize olanak sağlayan bir mekanizmadır.
#### Stash yapmanız gereken birkaç durum vardır:
                                      Değişikliklerinizi tamamlamadan başka bir görev veya branch üzerinde çalışmaya geçmek istediğinizde.
                                      
                                      Yarım kalmış veya tamamlanmamış değişikliklerinizi geçici olarak saklamak istediğinizde.
                                      
                                      Değişikliklerinizi commit etmeden önce biraz temizlik yapmak veya başka bir geliştiriciyle paylaşmadan önce kontrol etmek istediğinizde.

### git restore (ilkbolum.txt) : en son committe ne durumdaysan oraya döndürür

### pop : Git deposunda yapılacak değişikliklerle ilgili geçmişe yönelik işlemleri geri almak için kullanılır.

### git stash pop :  en son saklanan değişiklikleri geri almak ve saklama alanından kaldırmak.

### git stash list : komutu ile mevcut saklanan değişikliklerin listesini görüntülenir.


### git stash apply : komutu en son saklanan değişiklikleri geri almak için kullanılır. Bu komut, değişiklikleri uygular ancak saklama alanını temizlemez, yani saklanan değişiklikler hala saklama alanında kalır.

### git stash clear : komutu kullanılarak tüm saklanmış değişiklikler kalıcı olarak silinir.


