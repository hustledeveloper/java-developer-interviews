# java-developerMulakat-Sorulari

### _Java ve OOP_

### _Temel Web Geliştirme_

<details>

<summary>HTTP istek türleri nelerdir? Get ve Post arasındaki fark nedir?
?</summary>
GET: Bir kaynağın sunucudan alınması için kullanılır. URL üzerinden veri gönderirken, parametreler URL’in bir parçası olarak iletilir. GET isteği, sunucudaki kaynakları okumak için kullanılır ve idempotent bir işlem olarak kabul edilir (yani aynı isteği birden fazla kez göndermek sonuçları değiştirmemelidir).
POST: Bir kaynağa veri göndermek için kullanılır. POST isteği, sunucuya veri göndermek veya bir kaynağı değiştirmek için kullanılır. Veri, isteğin gövdesinde (body) taşınır ve genellikle bir HTML formu aracılığıyla gönderilir. POST isteği, sunucuda bir kaynağı oluşturabilir, güncelleyebilir veya silme işlemleri gerçekleştirebilir.
PUT: Bir kaynağı güncellemek veya oluşturmak için kullanılır. PUT isteği, sunucuya belirli bir URL altında kaynak oluşturmak veya güncellemek için kullanılır. PUT isteği, sunucuda belirtilen URL altında kaynak varsa güncelleme işlemi yapar, yoksa yeni bir kaynak oluşturur.
DELETE: Bir kaynağı silmek için kullanılır. DELETE isteği, sunucuda belirtilen bir URL altında kaynağın silinmesini sağlar.
PATCH: Bir kaynağın kısmi güncellemeleri için kullanılır. PATCH isteği, sunucuda belirtilen bir URL altındaki kaynağın belirli bir bölümünü güncellemek için kullanılır.

</details>

<details>

<summary>Bildiğin veri yapıları hakkında kısaca bilgi verebilir misin?
?</summary>

Dizi (Array):

Dizi, aynı türdeki verilerin bir araya getirildiği bir veri yapısıdır. Bellekte ardışık olarak yer kaplar ve her bir elemanı bir indeksle erişilebilir. Elemanlarına sabit sürede erişim sağlar.
Bağlı Liste (Linked List):

Bağlı liste, verilerin düğümler halinde saklandığı bir veri yapısıdır. Her düğüm, veriyi ve bir sonraki düğümün referansını içerir. Bağlı listeler, dinamik boyuta sahip olup, eleman ekleme ve silme işlemleri için uygundur. Erişim zamanı O(n)’dir.
Yığın (Stack):

Yığın, son giren ilk çıkar (LIFO) prensibiyle çalışan veri yapısıdır. Verilerin eklenip çıkarıldığı tek bir uç (top) bulunur. En son eklenen eleman en üstte tutulur. Eklenen ve çıkarılan elemanlar sabit sürede gerçekleşir.
Kuyruk (Queue):

Kuyruk, ilk giren ilk çıkar (FIFO) prensibiyle çalışan veri yapısıdır. Verilerin eklenip çıkarıldığı iki uç (ön ve arka) bulunur. En eski eklenen eleman ön tarafta, en yeni eklenen eleman ise arka tarafta tutulur.
Ağaç (Tree):

Ağaç, hiyerarşik bir yapıda düğümlerin birleştirildiği bir veri yapısıdır. Bir kök düğümü ve onun altındaki dallardan oluşur. Her düğüm birden fazla alt düğüm içerebilir. Ağaç veri yapısı, verileri organize etmek, arama ve sıralama gibi işlemleri hızlı bir şekilde gerçekleştirmek için kullanılır.
Graf (Graph):

Graf, düğümlerin ve bu düğümler arasındaki kenarların birleştiği bir veri yapısıdır. Düğümler, çeşitli ilişkileri temsil ederken, kenarlar bu ilişkileri gösterir. Graf veri yapısı, karmaşık ilişkileri ve bağlantıları modellerken kullanılır.

</details>

<details>

<summary>Büyük O (Big O) Gösterimi nedir?
?</summary>

Büyük O gösterimi, bir algoritmanın veya veri yapısının zaman ve/veya bellek karmaşıklığını ifade etmek için kullanılan bir notaçtır. Algoritmanın veya veri yapısının performansının, veri boyutuna bağlı olarak nasıl değiştiğini gösterir. Örneğin, O(1), O(n), O(n²) gibi ifadeler kullanılır. O(1) sabit zamanlı, O(n) lineer zamanlı, O(n²) ise karesel zamanlı karmaşıklığı ifade eder.

</details>

<details>

<summary>JWT token nedir?
?</summary>

JWT ile üretilen token Base64 ile kodlanmış 3 ana kısımdan oluşmaktadır. Bunlar Header(Başlık), Payload(Veri), Signature(İmza) kısımlarıdır.
Tokenın geçerli olup olmadığı JWT ile doğrulanır. JWT doğrulama işlemi oldukça basittir. Gelen tokenda Header(1. kısım) ve Payload(2. kısım) sunucumuzda bulunan gizli anahtar ile imzalanır ve 3. kısım hesaplanır. Daha sonra bu oluşturulan imza(3. kısım) client tarafından gelen imza ile karşılaştırılır. Eğer imzalar aynı ise token geçerli sayılır ve kullanıcıya erişim verilir.

</details>

<details>

<summary>REST API ve SOAP API arasındaki temel farklar nelerdir?
?</summary>

REST API ve SOAP API Arasındaki Temel Farklar:

1. Mimarisi:

REST: HTTP protokolü ve JSON/XML gibi hafif veri formatları üzerine kuruludur.
SOAP: XML tabanlı bir mesajlaşma protokolü üzerine kuruludur. 2. Karmaşıklık:

REST: Daha basit ve daha az karmaşıktır.
SOAP: Daha karmaşık ve daha fazla yapılandırmaya ihtiyaç duyar. 3. Performans:

REST: Daha hızlı ve daha hafiftir.
SOAP: Daha yavaş ve daha fazla kaynak kullanır. 4. Güvenlik:

REST: Güvenlik, ek modüller ile sağlanır.
SOAP: Kendiliğinden güvenlik mekanizmaları içerir. 5. Kullanım Alanları:

REST: Web servisleri, mobil uygulamalar, IoT cihazları gibi alanlarda kullanılır.
SOAP: Web servisleri, SOA (Service Oriented Architecture) gibi alanlarda kullanılır.
Kısaca:

REST, daha basit, daha hızlı ve daha hafif bir API'dir.
SOAP, daha karmaşık, daha güvenli ve daha fazla yapılandırmaya ihtiyaç duyan bir API'dir.

</details>

<details>

<summary>Refresh Token ve Acces Token nedir? Farkları nelerdir?
?</summary>

Access Token: Access Token, bir kullanıcının belirli kaynaklara (örneğin web API’larına) erişmesine izin veren ve sınırlı bir süre boyunca geçerli olan bir kimlik doğrulama belgesidir. Genellikle kısa ömürlüdür ve sınırlı erişim haklarına sahip olabilir. Access Token, bir kullanıcının kimlik doğrulama sürecinden geçtiğinde ve başarılı bir şekilde yetkilendirildiğinde elde edilir. Bu token, her istekte sunucuya gönderilir ve kullanıcının yetkilendirilmiş kaynaklara erişmesine olanak sağlar. Access Token, genellikle JSON Web Token (JWT) formatında veya benzer bir formatta oluşturulur ve içinde kullanıcının kimlik bilgilerini (örneğin kullanıcı kimliği, roller, izinler vb.) taşır.
Refresh Token: Refresh Token, Access Token’ın süresi dolduğunda yenilenmesini sağlayan ve daha uzun bir süre boyunca geçerli olan bir kimlik doğrulama belgesidir. Refresh Token, kullanıcının yetkilendirme işlemi sonucunda elde edilir ve güvenli bir şekilde saklanmalıdır, çünkü yeniden erişim belgesi almak için kullanılır. Refresh Token, sunucuya gönderildiğinde, sunucu tarafından değerlendirilir ve geçerli bir Refresh Token varsa, yeni bir Access Token oluşturulur ve kullanıcıya geri döndürülür. Bu sayede kullanıcı sürekli olarak oturum açma işlemi yapmadan ve kimlik doğrulama sürecini tekrarlamadan erişim belgesini yenileyebilir. Refresh Token’lar genellikle daha uzun süreli geçerlilik sürelerine sahiptir ve kullanıcının erişim yetkisini yenilemesini sağlar.
Refresh Token ve Access Token’lar, birlikte çalışarak kullanıcının yetkilendirme sürecini kolaylaştırır ve güvenli bir şekilde kaynaklara erişim sağlar. Access Token’lar sınırlı sürelerle kontrol edilen ve sınırlı yetkilere sahip olan erişim belgeleridir, Refresh Token’lar ise daha uzun süreli ve yeniden erişim belgesi almak için kullanılan kimlik doğrulama belgeleridir. Bu şekilde, kullanıcıların kimliklerini doğrulayarak güvenli bir şekilde uygulamalara ve kaynaklara erişmeleri sağlanır.

</details>

<details>

<summary>temel oop kavramlarını açıklar mısın?</summary>

Abstraction: Bir sınıfta davranış ve özelliklerin tanımlanmasıdır.
Encapsulation: Kapsülleme sayesinde, hangi özellik ve davranışların program dışına gösterilip gösterilmeyeceğini belirleriz.
Inheritance: : Sınıfların birbirinden türeme durumudur. Farklı sınıflar arasındaki ilişki “is a” şeklinde ifade edilir.
Inferface: Uygulamaların donanım yapılarıyla ve birbirleriyle iletişim kurması için kullandığı bir yapıdır. Zorunlu olarak tanımlanması gereken metotları belirtir.
Polymorphism: Methodların objeye göre farklı çıktılar üretmesi veya farklı işler yapmasıdır. Örneğin: Alt sınıfların farklı davranışları göstermesi.

</details>

<details>

<summary>Javada ”public static void main(String[ ] args)” neden kullanmalıyız?</summary>

JVM kodları çalışırken yazılmış classlar arasından başlayacağı noktayı bilmesi gerekmektedir. JVM, publicstaticvoidmain(String[ ] args) metodunu arar ve oradan çalışmaya başlar.

</details>

<details>

<summary>javada veri tipleri kaça ayrılır?</summary>

Java'da veri tipleri 3 ana kategoriye ayrılır:

1. Temel Veri Tipleri (Primitive Data Types)
   Tam Sayılar:
   byte (8 bit)
   short (16 bit)
   int (32 bit)
   long (64 bit)
   Ondalıklı Sayılar:
   float (32 bit)
   double (64 bit)
   Karakterler:
   char (16 bit)
   Mantıksal Değerler:
   boolean (true veya false)
2. Referans Tipleri (Reference Types)
   Nesneleri ve dizileri saklamak için kullanılır.
   Sınıflar
   Arabirimler
   Diziler
3. Özel Veri Tipleri (Special Data Types)
void
null
Temel veri tipleri, bellekten sabit miktarda yer kaplar ve doğrudan bellekte saklanır. Referans tipleri ise bellekten bir nesnenin veya dizinin başlangıç ​​adresini saklar.
Özel veri tipleri:
void fonksiyonların geri dönüş değerini belirtmek için kullanılır.
null bir referans tipinin değerinin boş olduğunu gösterir.
</details>

<details>

<summary>Implement, extend ve instanceof kavramlarını açıklayınız?
</summary>

Implement: Bir sınıfın belirli bir davranışa sahip olduğunu belirtmek için kullanılmalıdır. Bu davranış arayüzde tanımlanır ve sınıf bu arayüzü implement ederek bu davranışı sağlamalıdır.
Extend: Bir sınıftan yeni bir sınıf oluşturmak ve üst sınıfa ait özellikleri ve metotları kullanarak yeni bir davranış eklemek istediğinizde kullanılır.
Instanceof operatörü, bir nesnenin belirli bir sınıftan veya arayüzden olup olmadığını kontrol etmek için kullanılır.

</details>

<details>

<summary>Java'da Encapsulation Nedir?</summary>

Encapsulation, bir sınıfın üyelerini (değişkenler ve metotlar) korumak ve saklamak için kullanılan bir tekniktir. Bu teknik, sınıfın iç yapısını kullanıcılardan gizleyerek ve sadece belirli erişim izinleri sağlayarak kodun daha güvenli ve sağlam olmasını sağlar.
Encapsulation'ın faydaları:
Güvenlik: Sınıfın üyelerini yetkisiz erişimden korur.
Değişiklik esnekliği: Sınıfın iç yapısını değiştirmeyi kolaylaştırır.
Kodun sağlamlığı: Hatalı kodların ve veri tutarsızlıklarının önüne geçer.
Bakım kolaylığı: Kodun daha okunabilir ve anlaşılır olmasını sağlar.
Encapsulation nasıl uygulanır:

<figure><img src="assets/tables/unnamed (2).png" alt=""><figcaption></figcaption></figure>

Erişim belirteçleri: Sınıf üyelerinin erişim seviyelerini belirlemek için public, private ve protected gibi erişim belirteçleri kullanılır.
Getter ve setter metodları: Sınıfın private üyelerine erişmek için getter ve setter metodları kullanılır.

```java
public class Person {

    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}

```

Bu örnekte, Person sınıfının name ve age üyeleri private olarak belirtilmiştir. Bu üyelere doğrudan erişilemez. Erişim için getName(), setName(), getAge() ve setAge() metotları kullanılmalıdır.
Encapsulation, Java'da önemli bir programlama tekniğidir. Sınıfların üyelerini korumak ve saklamak için kullanılır. Bu teknik, kodun daha güvenli, sağlam ve bakımı kolay olmasını sağlar.

</details>

<details>

<summary>Java'da Polymorphism Nedir?
?</summary>

Polymorphism, birden fazla işlemin tek bir kod ile gerçekleştirilebilme özelliğidir. Java'da polymorphism iki şekilde gerçekleşir:

1. Overloading: Aynı isimdeki metotların farklı parametre listeleri ile tanımlanmasıdır. Bu sayede, aynı isimdeki metot farklı işlevler için kullanılabilir.
   Örnek:

```java
public class Overloading {

    public static void main(String[] args) {
        System.out.println(topla(2, 3)); // 5
        System.out.println(topla(2.5, 3.5)); // 6.0
    }

    public static int topla(int x, int y) {
        return x + y;
    }

    public static double topla(double x, double y) {
        return x + y;
    }
}
```

Bu örnekte, topla metodu iki farklı şekilde tanımlanmıştır. Birincisi int parametreler alır ve int değer döndürür. İkincisi ise double parametreler alır ve double değer döndürür.

2. Overriding: Bir alt sınıfta, bir üst sınıftaki metodun farklı bir şekilde tanımlanmasıdır. Bu sayede, alt sınıf, üst sınıftan devraldığı metodu kendi ihtiyacına göre özelleştirebilir.
   Örnek:

```java
public class Animal {

    public void speak() {
        System.out.println("Hayvan ses çıkarıyor.");
    }
}

public class Dog extends Animal {

    @Override
    public void speak() {
        System.out.println("Havlıyor.");
    }
}

public class Cat extends Animal {

    @Override
    public void speak() {
        System.out.println("Miyavlıyor.");
    }
}

public class Main {

    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.speak(); // Hayvan ses çıkarıyor.

        Dog dog = new Dog();
        dog.speak(); // Havlıyor.

        Cat cat = new Cat();
        cat.speak(); // Miyavlıyor.
    }
}
```

Bu örnekte, Animal sınıfındaki speak metodu, Dog ve Cat sınıflarında farklı şekilde override edilmiştir. Bu sayede, her hayvan kendi türüne özgü ses çıkarabilir.
Polymorphism'in faydaları:
Kodun daha az tekrarlı olmasını sağlar.
Kodun daha okunabilir ve anlaşılır olmasını sağlar.
Kodun daha esnek ve genişletilebilir olmasını sağlar.
Bakım kolaylığı sağlar.
Polymorphism, Java'da önemli bir programlama tekniğidir. Kodun daha az tekrarlı, daha okunabilir, daha esnek ve daha bakımı kolay olmasını sağlar.

</details>

<details>

<summary>Java’da hata ayıklanması (exception handling) nasıl yapılır?
?</summary>

Java'da hata ayıklama, try-catch blokları ve throw anahtar sözcüğü ile yapılır.
try-catch Blokları:
try bloğu, hataya neden olabilecek kodları içerir.
catch bloğu, hataya ne zaman ve nasıl tepki verileceğini tanımlar.
throw Anahtar Sözcüğü:
throw anahtar sözcüğü, kasıtlı olarak bir hata oluşturmak için kullanılır.

</details>

<details>

<summary>throw ile throws arasındaki fark nedir??</summary>

Throw ve Throws Arasındaki Fark
Throw ve throws, Java'da hata fırlatmak ve yönetmek için kullanılan iki anahtar kelimedir. Amaçları ve kullanımları bakımından farklıdırlar.
Throw:
Bir hata oluştuğunda program akışını durdurmak ve hatayı yukarıdaki katmana fırlatmak için kullanılır.
Bir try-catch bloğunun içinde veya dışında kullanılabilir.
Fırlatılan hata bir Exception veya Error nesnesi olmalıdır.
Tek bir hata fırlatmak için kullanılır.
Throws:
Bir metodun hangi hataları fırlatabileceğini bildirmek için kullanılır.
Metodun başında, parametre listesinden sonra yer alır.
Fırlatılabilecek hatalar bir veya daha fazla Exception nesnesi olarak belirtilir.
Metodun hata fırlatıp fırlatmayacağını garanti etmez.
Hata fırlatma işlemi try-catch bloğunda kontrol edilir.

<figure><img src="assets/tables/unnamed (1).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>Java’da nesneleri karşılaştırıken .equals() ile == kullanmanın farkı nedir?</summary>

Java'da nesneleri karşılaştırmak için iki yöntem kullanılır:

1. == Operatörü:
   == operatörü, iki nesnenin referanslarının aynı olup olmadığını kontrol eder.
   İki nesnenin referansları aynıysa, == operatörü true döndürür.
   String s1 = "Merhaba";
   String s2 = "Merhaba";

if (s1 == s2) {
System.out.println("Nesneler aynı!");
} else {
System.out.println("Nesneler farklı!");
}

2. .equals() Metotu:
   .equals() metodu, iki nesnenin içeriklerinin aynı olup olmadığını kontrol eder.
   .equals() metodu true döndürürse, iki nesnenin içerikleri aynıdır.
   Ne zaman neyi kullanmalıyız?
   Nesnelerin referanslarının aynı olup olmadığını kontrol etmek istiyorsanız == operatörünü kullanmalısınız.
   Nesnelerin içeriklerinin aynı olup olmadığını kontrol etmek istiyorsanız .equals() metodunu kullanmalısınız.
   Dikkat:
   == operatörü, primitive tipler için de kullanılabilir. Primitive tipler için == operatörü, iki değerin aynı olup olmadığını kontrol eder.
   .equals() metodu, Object sınıfından miras alınır. Bu nedenle, tüm nesneler .equals() metoduna sahiptir.

```java
kodlar kodlar
```

</details>

<details>

<summary>Java’da bir alt sınıf üstün private metodları kullanabilir mi?
?</summary>

Hayır, bir alt sınıf, üst sınıfın private olarak tanımlanmış metotlarını doğrudan kullanamaz.
Sebep:
private erişim belirteci, metodun sadece tanımlandığı sınıf tarafından erişilebilir olmasını sağlar. Alt sınıflar, üst sınıftan miras almış olsalar bile, private metotları doğrudan kullanamazlar.

</details>

<details>

<summary>Java’da multi inheritance var mıdır, neden?</summary>

Hayır, Java'da çoklu kalıtım (multi inheritance) doğrudan desteklenmez. Bunun sebeplerinden biri Diamond Problemidir:
Bir sınıf birden fazla sınıftan miras alırsa ve bu sınıflardan birkaçı aynı metodu veya field'ı tanımlarsa, hangisinin kullanılacağına karar vermede belirsizlik oluşur. Bu duruma diamond problemi denir.
Örnek:

```java

public interface Animal {
    void makeSound();
}

public interface Dog {
    void makeSound();
}

public class Cat implements Animal, Dog {
    // Hangi makeSound() metodu kullanılacak?
}

```

</details>

<details>

<summary>Java’da multithreading nedir?</summary>

Java'da çoklu iş parçacıklılık (multithreading, bir uygulamanın içerisinde birden fazla iş parçacığının (thread) eş zamanlı olarak çalışmasına olanak tanıyan bir programlama tekniğidir. Bu iş parçacıkları, uygulamanın farklı görevlerini aynı anda yürütmeyi mümkün kılar, programın daha duyarlı ve verimli olmasını sağlar.
İş parçacığı (thread), işletim sistemi tarafından yönetilen ve CPU zaman dilimi içinde bağımsız olarak yürütülen bir kod parçasıdır. Bir uygulama aynı anda birden fazla iş parçacığına sahip olabilir ve bu iş parçacıkları birbirlerinden bağımsız olarak çalışır.
Avantajlar:
Duyarlılık: Kullanıcı arayüzünün donmadan diğer görevleri yerine getirmenizi sağlar. Örneğin, bir program müzik çalarken aynı anda dosya indirebilir.
Verimlilik: Birden fazla CPU çekirdeği varsa, her çekirdeği kullanan iş parçacıkları ile uygulamanın performansını artırabilirsiniz.
Uzun süreli işlemler: Ağ bağlantısı gibi uzun süreli işlemleri arka planda gerçekleştirerek kullanıcı arayüzünün duyarlı kalmasını sağlayabilirsiniz.
Dezavantajlar:
Karmaşıklık: Çoklu iş parçacıklı programlama tek iş parçacıklı programlamaya göre daha karmaşıktır. İş parçacıklarının senkronize edilmesi ve veri yarışlarını önlemek için dikkatli kod yazımı gerekir.
Hata ayıklama: Çoklu iş parçacıklı program hatalarını ayıklamak daha zor olabilir. Bir hata farklı iş parçacıklarının etkileşiminden kaynaklanabilir.
Java'da çoklu iş parçacıklılık:
Java, Thread sınıfı ve iş parçacıklarını senkronize etmek için çeşitli mekanizmalar (kilitler, semaforlar) ile çoklu iş parçacıklı programlama desteği sunar. Bunların yanı sıra, ExecutorService ve Callable arayüzleri gibi daha yüksek seviyeli API'ler de mevcuttur.
Örnek:

```java
public class Example {
  public static void main(String[] args) {
    Thread thread1 = new Thread(() -> {
      // İş parçacığı 1'in yapacağı iş
    });
    Thread thread2 = new Thread(() -> {
      // İş parçacığı 2'nin yapacağı iş
    });

    thread1.start();
    thread2.start();
  }
}
```

Bu örnekte, thread1 ve thread2 adında iki iş parçacığı oluşturulur ve her biri farklı bir işi yürütecek şekilde programlanır. Her iki iş parçacığı da aynı anda başlatılır ve kendi görevlerini bağımsız olarak yerine getirir.

</details>

<details>

<summary>Java’da thread safe yöntemleri nelerdir?
?</summary>

Java'da thread-safe yöntemler, birden fazla thread tarafından aynı anda erişildiğinde tutarsızlık veya veri bozulması oluşmadan çalışabilen yöntemlerdir. Bu yöntemler, thread'lerin birbirleriyle senkronize olmasını ve veri erişimini kontrol etmesini sağlayarak programın stabilitesini ve güvenliğini artırır.
Thread-safe yöntemleri oluşturmak için:

1. Synchronized Anahtar Sözcüğü:
   synchronized anahtar sözcüğü, bir metodun veya kod bloğunun bir anda sadece bir thread tarafından erişilebilir olmasını sağlar. Bu sayede, bir thread metodu çalıştırırken diğer thread'ler o metodun tamamlanmasını bekler.
   public synchronized void someMethod() {
   // Thread-safe kod
   }
2. Kilitler (Locks):
   Kilitler, bir resource'a erişimi kontrol etmek için kullanılan nesnelerdir. Bir thread bir resource'a erişmek istediğinde kilidi alır ve işini tamamladıktan sonra kilidi serbest bırakır. Bu sayede, birden fazla thread aynı resource'a erişmeye çalışırken veri bozulması önlenir.
   private final Lock lock = new ReentrantLock();
   public void someMethod() {
   lock.lock();
   try {
   // Thread-safe kod
   } finally {
   lock.unlock();
   }
   }
3. Atomik İşlemler:
   Atomik işlemler, tek bir adımda tamamlanan ve bölünemeyen işlemlerdir. Bu işlemler, birden fazla thread tarafından aynı anda erişilse bile tutarsızlık oluşmaz. Java'da AtomicInteger gibi atomik değişkenler ve compareAndSet() gibi atomik işlemler mevcuttur.

private final AtomicInteger counter = new AtomicInteger();

public void incrementCounter() {
counter.incrementAndGet();
} 4. Değişmez Nesneler (Immutable Objects):
Değişmez nesneler, oluşturulduktan sonra değiştirilemeyen nesnelerdir. Bu nesneler, birden fazla thread tarafından erişilse bile tutarsızlık oluşmaz. Java'da String ve Integer gibi değişmez nesneler mevcuttur.

private final String name = "John Doe";

public String getName() {
return name;
} 5. Thread-safe Kütüphaneler:
Java'da java.util.concurrent paketi gibi thread-safe kütüphaneler mevcuttur. Bu kütüphaneler, thread-safe koleksiyonlar, senkronizasyon araçları ve diğer yardımcı sınıflar içerir.
Thread-safe yöntemleri kullanmanın faydaları:
Veri tutarsızlığı ve bozulmasını önler
Programın stabilitesini ve güvenliğini artırır
Thread'ler arasında veri yarışlarını (data races) önler
Programın performansını optimize etmeye yardımcı olur
Thread-safe yöntemleri kullanırken dikkat edilmesi gerekenler:
Gereksiz yere synchronized anahtar sözcüğü kullanmaktan kaçının, performansı düşürebilir.
Doğru kilit türünü seçin, ReentrantLock gibi.
Atomik işlemleri doğru kullanın.
Değişmez nesneleri tercih edin.
Thread-safe kütüphanelerden yararlanın.

</details>

<details>

<summary>Java’da koleksiyon yapıları olan list ve set arasındaki farklar nedir??</summary>

Java'da List ve Set Arasındaki Farklar
Java'da list ve set, verileri depolamak için kullanılan iki temel koleksiyon yapıdır. Her ikisinin de kendine özgü özellikleri ve kullanım alanları vardır.
List:
Sıralıdır: Elemanlar belirli bir sırayla depolanır.
Tekrarlara izin verir: Aynı eleman birden fazla kez listede bulunabilir.
Farklı tiplerde elemanlar barındırabilir: Elemanların türü generics ile belirtilir.
Dinamik olarak büyüyebilir: Listeye yeni elemanlar eklendikçe boyutu artar.
Elemanlara erişmek için indis kullanılır: Belirli bir indisteki elemana doğrudan erişilebilir.
Set:
Sırasızdır: Elemanların sırası rastgeledir.
Tekrarlara izin vermez: Her eleman sadece bir kez sette bulunabilir.
Farklı tiplerde elemanlar barındırabilir: Elemanların türü generics ile belirtilir.
Dinamik olarak büyüyebilir: Sete yeni elemanlar eklendikçe boyutu artar.
Elemanlara erişmek için indis kullanılmaz: Belirli bir elemana doğrudan erişmek zordur.
Kullanım Alanları:
List: Sıralı verileri depolamak için kullanılır. Örneğin, bir alışveriş listesi, öğrenci listesi veya isimler listesi.
Set: Benzersiz elemanları depolamak için kullanılır. Örneğin, bir kelime listesi, kullanıcı kimliği listesi veya ürün katalogu.

<figure><img src="assets/tables/unnamed (8).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>+Java’da nesneleri nasıl sıralayabiliriz?
?</summary>

Java'da nesneleri sıralamak için iki temel yöntem vardır:

1.  Comparable Kullanarak:
    Comparable arayüzünü uygulayan nesneler karşılaştırılabilir hale gelir.
    Bu arayüz, compareTo() adında bir metodu tanımlar.
    Bu metot, iki nesneyi karşılaştırarak hangisinin daha büyük veya daha küçük olduğunu belirler.
    Örnek:
    Java
    public class Person implements Comparable<Person> {
    private String name;
    private int age;

        public Person(String name, int age) {
            this.name = name;
            this.age = age;
        }

        @Override
        public int compareTo(Person other) {
            return this.age - other.age;
        }

    }

// Sıralama
List<Person> people = Arrays.asList(
new Person("Ahmet", 25),
new Person("Ayşe", 30),
new Person("Mehmet", 20)
);

Collections.sort(people);

// Yaş sırasına göre yazdırma
for (Person person : people) {
System.out.println(person.name + " - " + person.age);
}

2. Stream Kullanarak:
   Java 8'den itibaren Stream API'si kullanılarak nesneleri sıralamak daha kolay hale gelmiştir.
   sorted() metodu, bir stream'deki nesneleri belirli bir kritere göre sıralar.
   Örnek:
   Java
   List<Person> people = Arrays.asList(
   new Person("Ahmet", 25),
   new Person("Ayşe", 30),
   new Person("Mehmet", 20)
   );

people.stream()
.sorted(Comparator.comparingInt(Person::getAge))
.forEach(System.out::println);

Farklı Sıralama Kriterleri:
Comparable ile sıralama yaparken sadece tek bir kritere göre sıralama yapılabilir.
Stream API ile birden fazla kritere göre sıralama yapılabilir.
sorted() metodu ile sıralama yönü de belirlenebilir (artan veya azalan).
Özet:
Comparable arayüzünü kullanarak nesneleri karşılaştırılabilir hale getirebilirsiniz.
Stream API'si ile nesneleri daha kolay ve esnek bir şekilde sıralayabilirsiniz.
Hangi yöntemi kullanacağınız, ihtiyaçlarınıza ve sıralama kriterlerinize bağlıdır.

</details>

<details>

<summary>Java 8 ile gelen yenilikler nelerdir? (stream, addtype, gibi)
?</summary>

Java 8 ile gelen yenilikler, Java'da programlama yapmayı daha kolay, daha güçlü ve daha esnek hale getirmiştir. Bu yeniliklerden bazıları şunlardır:

1. Lambda İfadeleri:
   Fonksiyonları daha kısa ve öz bir şekilde yazmamızı sağlar.
   Örnek:
   Java
   // Java 7
   List<String> names = Arrays.asList("Ahmet", "Ayşe", "Mehmet");
   Collections.sort(names, new Comparator<String>() {
   @Override
   public int compare(String o1, String o2) {
   return o1.compareTo(o2);
   }
   });

// Java 8
names.sort((o1, o2) -> o1.compareTo(o2));

2. Stream API:
   Koleksiyonlar üzerinde daha kolay ve işlevsel bir şekilde işlem yapmamızı sağlar.
   Örnek:

// Java 7
List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5);
int sum = 0;
for (int number : numbers) {
if (number % 2 == 0) {
sum += number;
}
}

// Java 8
sum = numbers.stream().filter(n -> n % 2 == 0).sum();

3. Method References:
   Metotları daha kısa ve öz bir şekilde referans almamızı sağlar.
   Örnek:
   Java
   // Java 7
   List<String> names = Arrays.asList("Ahmet", "Ayşe", "Mehmet");
   Collections.sort(names, String::compareToIgnoreCase);

// Java 8
names.sort(String::compareToIgnoreCase);

4. Date and Time API:
   Tarih ve saat ile işlemleri daha kolay ve modern bir şekilde yapmamızı sağlar.
   Örnek:

// Java 7
Date date = new Date();
Calendar calendar = Calendar.getInstance();
calendar.setTime(date);

// Java 8
LocalDate localDate = LocalDate.now();
LocalTime localTime = LocalTime.now();

5. Optional Class:
   null değerlerini daha güvenli ve işlevsel bir şekilde yönetmemizi sağlar.
   Örnek:
   Java
   // Java 7
   String name = null;
   if (name != null) {
   System.out.println(name.toUpperCase());
   }

// Java 8
Optional<String> optionalName = Optional.ofNullable(name);
optionalName.ifPresent(System.out::println);

6.  Default ve Static Metotlar:
    Arayüzlere yeni metotlar eklememizi sağlar.
    Örnek:
    Java
    public interface Animal {
    default void makeSound() {
    System.out.println("Ses çıkarıyor...");
    }

        static void printInfo() {
            System.out.println("Hayvan sınıfı");
        }

    }

public class Dog implements Animal {
@Override
public void makeSound() {
System.out.println("Havlıyor!");
}
}

Dog dog = new Dog();
dog.makeSound(); // Havlıyor!
Animal.printInfo(); // Hayvan sınıfı

Default implementasyonun faydaları:
Arayüzlere yeni metotlar eklemeyi kolaylaştırır.
Mevcut arayüzleri yeni fonksiyonlar ile zenginleştirmeye imkan verir.
Arayüzü kullanan sınıflara kod ekleme ihtiyacını azaltır.
Geriye dönük uyumluluğu (backward compatibility) korur.
Default implementasyon kullanırken dikkat edilmesi gerekenler:
Aynı metot ismi ile bir override işlemi yapılmazsa default implementasyon kullanılır.
Metot override edilirse default implementasyon göz ardı edilir.
Abstract metotlar default implementasyon ile somut hale getirilebilir.

Ayrıca:
Static metotlar da arayüzlere eklenebilir.
Private metotlar ise eklenilemez.

7. Nashorn JavaScript Motoru:
   Java'da JavaScript kodlarını çalıştırmamızı sağlar.

Bunlar sadece Java 8 ile gelen yeniliklerden birkaçıdır.

</details>

<details>

<summary>Uçtan uca bir proje yazılmaya başlanırken hangi teknolojiler kullanılır ve neden bunlar kullanılır? 
?</summary>

Yaygın olarak kullanılan bazı teknolojiler ve neden tercih edildikleri hakkında bilgiler yer almaktadır:
Spring Boot:
Java ile uygulama geliştirmeyi kolaylaştıran bir framework
Hızlı ve kolay uygulama başlatma
Dahili Tomcat sunucu
Otomatik konfigürasyon
Çeşitli starter modülleri ile entegrasyon kolaylığı
PostgreSQL:
Nesne-ilişkisel bir veritabanı yönetim sistemi (DBMS)
Güçlü ve güvenilir
Açık kaynak kodlu
Geniş bir özellik yelpazesi
Gelişmiş veri tipleri ve fonksiyonları
MongoDB:
NoSQL bir veritabanı yönetim sistemi (DBMS)
Belge odaklı veri depolama
Hızlı ve ölçeklenebilir
JSON ile kolay veri entegrasyonu
Geliştiriciler için kullanımı kolay

PostgreSQL vs MongoDB:

<figure><img src="assets/tables/unnamed (3).png" alt=""><figcaption></figcaption></figure>

GraphQL:
API'ler için sorgulanan bir dil
Esnek ve güçlü
Veri isteklerini optimize etme
Client ve sunucu arasında güçlü bir sözleşme
Geliştirici deneyimini iyileştirme
Spring Security:
Spring framework için bir güvenlik çözümü
Kullanıcı kimlik doğrulama ve yetkilendirme
Farklı kimlik doğrulama sağlayıcıları ile entegrasyon
CSRF ve XSS gibi saldırılara karşı koruma
Rol ve izin yönetimi
Teknoloji Seçimi Faktörleri:
Projenin gereksinimleri: Veri modeli, performans, ölçeklenebilirlik ve güvenlik gibi gereksinimleri göz önünde bulundurun.
Hedef kitle: Geliştiricilerin ve kullanıcıların beceri seviyesini ve deneyimlerini dikkate alın.
Bütçe ve zaman: Ücretli ve ücretsiz seçenekler arasından bütçenize ve zaman çizelgesine uygun olanları seçin.
Topluluk desteği: Seçtiğiniz teknolojiler için aktif ve destekleyici bir topluluk olduğundan emin olun.

</details>

<details>

<summary>Java’da monolith nedir? mikro servisler nedir ve farkları nelerdir?
?</summary>

Java'da Monolith ve Mikro Hizmetler
Monolith:
Tek bir birim olarak geliştirilen ve dağıtılan bir uygulamadır. Tüm işlevler tek bir kod tabanında ve tek bir sunucuda çalışır.
Monolith'in avantajları:
Geliştirme ve dağıtım basittir.
Hata ayıklama ve test etme daha kolaydır.
Tek bir kod tabanı olduğu için tutarlılık ve uyumluluk sağlanır.
Monolith'in dezavantajları:
Ölçeklendirme zor olabilir.
Bir değişiklik tüm uygulamayı etkiler.
Hata veya gecikme tüm uygulamayı etkileyebilir.
Mikro Hizmetler:
Bağımsız ve birbirinden izole edilmiş küçük hizmetlerden oluşan bir uygulama mimarisidir. Her hizmet kendi kod tabanına, veritabanına ve sunucusuna sahiptir.
Mikro hizmetlerin avantajları:
Ölçeklendirme kolaydır.
Her hizmet bağımsız olarak geliştirilebilir ve dağıtılabilir.
Bir hizmetteki hata veya gecikme diğer hizmetleri etkilemez.
Mikro hizmetlerin dezavantajları:
Geliştirme ve dağıtım daha karmaşıktır.
Hata ayıklama ve test etme daha zor olabilir.
Hizmetler arasındaki iletişimi yönetmek gerekir.
Monolith ve Mikro Hizmetler Arasındaki Farklar:

<figure><img src="assets/tables/unnamed (7).png" alt=""><figcaption></figcaption></figure>

Ek soru Yemeksepeti Neden Monolith Değildir:
Yemeksepeti, milyonlarca kullanıcısı olan bir platformdur. Bu kadar yüksek bir kullanıcı sayısını monolith bir mimari ile desteklemek zordur. Bu nedenle Yemeksepeti, mikro hizmetler mimarisine geçmiştir.
Yemeksepeti'nde Mikro Hizmetler:
Yemeksepeti, farklı işlevler için farklı mikro hizmetler kullanmaktadır. Örneğin, sipariş verme, ödeme ve teslimat için ayrı mikro hizmetler vardır. Bu sayede Yemeksepeti, yüksek kullanıcı sayısını daha kolay yönetebilmektedir.

</details>

<details>

<summary>Java’da heap ve stack nedir??</summary>

Java'da Heap ve Stack
Heap ve stack, Java'da bellek yönetimi için kullanılan iki farklı bölgedir.
Heap:
Nesnelerin saklandığı bölgedir.
Nesneler, new operatörü ile oluşturulduğunda heap'te yer alır.
Heap, garbage collector tarafından yönetilir.
Garbage collector, kullanılmayan nesneleri bellekten siler.
Stack:
Yerel değişkenler, metot parametreleri ve çağrı çerçeveleri gibi geçici verilerin saklandığı bölgedir.
LIFO (Last In First Out) mantığıyla çalışır.
Metot sona erdiğinde, stack'teki ilgili veri silinir.
Heap ve Stack Arasındaki Farklar:

<figure><img src="assets/tables/unnamed (6).png" alt=""><figcaption></figcaption></figure>

Java
public class Main {
public static void main(String[] args) {
int a = 10; // Stack'te saklanır
String s = "Merhaba"; // Heap'te saklanır

        // ...
    }

}

Bu örnekte, a değişkeni stack'te, s değişkeni ise heap'te saklanır. main() metotu sona erdiğinde, a değişkeni stack'ten silinir. s değişkeni ise garbage collector tarafından bellekten silinene kadar heap'te kalacaktır.
Heap ve stack, Java'da bellek yönetimi için önemli iki kavramdır. Bu kavramları anlamak, programınızın bellek kullanımını optimize etmenize yardımcı olacaktır.

Heap ve Stack ile İlgili Ek Bilgiler:
Heap, genellikle sabit bir boyuta sahiptir, ancak gerektiğinde büyüyebilir.
Stack, her thread için ayrı olarak oluşturulur.
Stack'in boyutu, programın karmaşıklığına bağlı olarak değişebilir.
Heap ve stack, sanal bellek adresleri ile yönetilir.
Java'da, new operatörü heap'te yeni bir nesne oluşturur ve null referansı ise heap'te yer almayan bir nesneyi gösterir.
Stack overflow hatası, stack'in dolması durumunda oluşur.
Heap ve stack, Java'da programlama yaparken göz önünde bulundurulması gereken önemli kavramlardır. Bu kavramları anlamak, programınızın bellek kullanımını optimize etmenize ve daha iyi performans elde etmenize yardımcı olacaktır.

</details>

<details>

<summary>soru?</summary>

cevap

</details>

<details>

<summary>Java’da Garbage collection ne işe yarar?
?</summary>

Java'da Garbage Collection Nedir ve Ne İşe Yarar?
Garbage collection (Çöp toplama), Java'da bellek yönetimini otomatik hale getiren bir mekanizmadır. Bu mekanizma, programın bellek kullanımını optimize etmeye ve bellek sızıntılarını önlemeye yardımcı olur.
Garbage collection nasıl çalışır?
Nesne oluşturma: new operatörü ile bir nesne oluşturulduğunda, garbage collector tarafından heap'te bir bellek alanı tahsis edilir.
Nesneye erişme: Bir nesneye referans aracılığıyla erişilir. Referans sayısı, nesneye kaç tane referans olduğunu gösterir.
Nesnenin kullanılmaması: Bir nesneye artık ihtiyaç duyulmadığında, referanslar silinir. Referans sayısı 0'a ulaştığında, nesne garbage collector tarafından işaretlenir.
Garbage collection çalışması: Garbage collector, işaretlenmiş nesneleri bellekten siler ve boş bellek alanlarını tekrar kullanıma sunar.
Garbage collection'ın faydaları:
Bellek yönetimini otomatik hale getirir: Programcıların bellek yönetimi ile uğraşmasına gerek kalmaz.
Bellek sızıntılarını önler: Kullanılmayan nesneler otomatik olarak bellekten silinir.
Programın bellek kullanımını optimize eder: Garbage collector, bellek kullanımını optimize etmek için çeşitli algoritmalar kullanır.
Garbage collection'ın dezavantajları:
Performans üzerinde ek yük oluşturabilir: Garbage collection çalışması, programın performansını geçici olarak etkileyebilir.
Bellek kullanımının tam kontrolünü programcıya vermez: Programcılar, garbage collector'ın ne zaman çalışacağını ve hangi nesneleri sileceğini tam olarak kontrol edemez.
Garbage collection ile ilgili bazı önemli noktalar:
Garbage collector, nesnelerin bellekten silinme sırasını garanti etmez.
finalize() metotu, garbage collector tarafından çağrılmadan önce nesnenin bellekten silinmesini garanti etmez.
System.gc() metotu garbage collector'ı çalıştırmaya zorlar, ancak bu metodun ne zaman ve nasıl çalışacağını garanti etmez.

</details>

<details>

<summary>Java’da builder nedir?
?</summary>

Java'da Builder Nedir?
Builder, karmaşık nesnelerin adım adım oluşturulmasını sağlayan bir tasarım desenidir. Bu desen, nesnelerin birden fazla parametreye sahip olabileceği ve parametrelerin sırasının önemli olduğu durumlarda kullanışlıdır.
Builder deseninin faydaları:
Karmaşık nesnelerin oluşturulmasını kolaylaştırır: Builder, karmaşık nesnelerin tek bir satırda değil, adım adım oluşturulmasını sağlar.
Kodun daha okunabilir ve anlaşılır olmasını sağlar: Builder, kodun daha iyi organize edilmesine ve karmaşık nesnelerin oluşturulmasının daha kolay anlaşılmasına yardımcı olur.
Nesnelerin parametrelerinin sırasını ve değerlerini kontrol etmeyi sağlar: Builder, nesnelerin parametrelerinin doğru sırayla ve doğru değerlerle girilmesini garanti eder.
Değiştirilebilir nesneler oluşturmayı kolaylaştırır: Builder, nesnelerin farklı konfigürasyonlar ile oluşturulmasını kolaylaştırır.
Builder deseninin nasıl uygulandığı:
Builder arayüzü: Nesnenin hangi parametrelere sahip olacağını ve hangi sırayla oluşturulacağını tanımlayan bir arayüz oluşturulur.
Concrete builder: Builder arayüzünü uygulayan ve nesnenin nasıl oluşturulacağını tanımlayan somut sınıflar oluşturulur.
Director: Builder arayüzünü kullanarak nesnenin nasıl oluşturulacağını yöneten bir sınıf oluşturulur.
Client: Nesneyi oluşturmak için director sınıfını kullanır.
Builder deseninin bir örneği:

public interface PersonBuilder {
PersonBuilder setName(String name);
PersonBuilder setAge(int age);
PersonBuilder setAddress(String address);
Person build();
}

public class ConcretePersonBuilder implements PersonBuilder {
private String name;
private int age;
private String address;

    @Override
    public PersonBuilder setName(String name) {
        this.name = name;
        return this;
    }

    @Override
    public PersonBuilder setAge(int age) {
        this.age = age;
        return this;
    }

    @Override
    public PersonBuilder setAddress(String address) {
        this.address = address;
        return this;
    }

    @Override
    public Person build() {
        return new Person(name, age, address);
    }

}

public class Director {
private PersonBuilder builder;

    public Director(PersonBuilder builder) {
        this.builder = builder;
    }

    public Person constructPerson() {
        builder.setName("John Doe");
        builder.setAge(30);
        builder.setAddress("123 Main Street");
        return builder.build();
    }

}

public class Main {
public static void main(String[] args) {
Director director = new Director(new ConcretePersonBuilder());
Person person = director.constructPerson();
System.out.println(person);
}
}

Bu örnekte, Person nesnesi karmaşık bir nesnedir ve birden fazla parametreye sahiptir. Builder deseni kullanılarak, bu nesne adım adım ve kolay bir şekilde oluşturulabilir.
Builder deseninin kullanılabileceği durumlar:
Karmaşık nesnelerin oluşturulması
Nesnelerin parametrelerinin sırasının önemli olduğu durumlar
Değiştirilebilir nesnelerin oluşturulması
Kodun daha okunabilir ve anlaşılır olması istenilen durumlar
Builder deseni, karmaşık nesnelerin oluşturulmasını kolaylaştıran ve kodun daha okunabilir ve anlaşılır olmasını sağlayan bir tasarım desenidir. Bu desenin nasıl uygulandığını ve ne zaman kullanılabileceğini anlamak, programcıların daha iyi Java programları yazmalarına yardımcı olacaktır.

</details>

<details>

<summary>Java nasıl çalışır?  javac java jvm açıkla bunları da
?</summary>

Java Nasıl Çalışır?
Java, platformdan bağımsız bir programlama dilidir. Bu, Java kodunun herhangi bir işletim sisteminde, herhangi bir donanım üzerinde çalıştırılabileceği anlamına gelir. Java'nın bu özelliği, "bir kere yaz, her yerde çalıştır" (WORA) ilkesine dayanır.
Javac:
Java kaynak kodunu (.java dosyaları) bytecode'a dönüştüren bir derleyicidir.
Bytecode, Java Sanal Makinesi (JVM) tarafından anlaşılabilen bir makine kodudur.
Javac, işletim sisteminden bağımsız bytecode üretir.
Java:
Java bytecode'u çalıştıran bir programdır.
JVM, her işletim sistemi için ayrı bir implementation'a sahiptir.
JVM, bytecode'u işletim sisteminin anlayabileceği makine koduna dönüştürür.
JVM:
Java bytecode'u çalıştıran bir sanal makinedir.
JVM, bellek yönetimi, garbage collection, thread yönetimi gibi görevleri yerine getirir.
JVM, işletim sisteminden bağımsız bir şekilde çalışır.
Java'nın Çalışma Prensibi:
Java kaynak kodu (.java dosyası) javac derleyicisi ile bytecode'a dönüştürülür.
Oluşturulan bytecode, JVM tarafından çalıştırılır.
JVM, bytecode'u işletim sisteminin anlayabileceği makine koduna dönüştürür.
Dönüştürülen kod, işletim sistemi tarafından çalıştırılır.
Java'nın Avantajları:
Platformdan bağımsızlık
Nesneye dayalı programlama
Güvenlik
Güçlü bellek yönetimi
Geniş bir kütüphane yelpazesi
Java'nın Dezavantajları:
Performans, yerel dillere göre daha düşük olabilir.
Karmaşık bir dil olabilir.
Java’da this() ve super() arasındaki fark nedir?
this():
Bir sınıfın mevcut örneğini temsil eder.
Aynı sınıfın varsayılan kurucusunu çağırmak için kullanılır.
Mevcut sınıfın yöntemlerine erişmek ve sınıf örneğini işaret etmek için kullanılır.
super():
Bir üst/temel sınıfın geçerli örneğini temsil eder.
Üst/temel sınıfın varsayılan yapıcısını çağırmak için kullanılır.
Temel sınıfın yöntemlerine erişmek ve üst sınıf örneğini işaret etmek için kullanılır.

</details>

<details>

<summary>JDK, JRE ve JWM nedir? 
?</summary>

JDK (Java Development Kit): Java uygulamaları geliştirmek için kullanılan bir yazılım geliştirme paketidir. JDK, aşağıdakileri içeren bir dizi araç ve kütüphane içerir:
Derleyici (javac): Java kaynak kodunu (.java dosyaları) bytecode'a dönüştürür.
Yorumlayıcı (java): Bytecode'u çalıştırır.
Arşivleyici (jar): Birden fazla dosyayı tek bir dosyada birleştirir.
Dokümantasyon oluşturucu (Javadoc): Java API'si için dokümantasyon oluşturur.
Java kütüphaneleri: Java API'sinin bir parçası olan temel sınıflar ve arayüzler.
JRE (Java Runtime Environment): Java uygulamalarını çalıştırmak için gerekli olan bir yazılım ortamıdır. JRE, aşağıdakileri içerir:
Java Sanal Makinesi (JVM): Bytecode'u işletim sisteminin anlayabileceği makine koduna dönüştürür.
Java kütüphaneleri: Java API'sinin bir parçası olan temel sınıflar ve arayüzler.
JVM (Java Virtual Machine): Java bytecode'u çalıştıran bir sanal makinedir. JVM, aşağıdakileri içerir:
Bytecode yorumlayıcısı: Bytecode'u satır satır yorumlar.
Just-In-Time (JIT) derleyicisi: Bytecode'u çalıştırma sırasında yerel makine koduna dönüştürür.
Bellek yönetimi: Nesnelerin bellekten tahsis edilmesini ve silinmesini yönetir.
Garbage collection: Kullanılmayan nesneleri bellekten otomatik olarak siler.
Özet:
JDK, Java uygulamaları geliştirmek için kullanılır.
JRE, Java uygulamalarını çalıştırmak için kullanılır.
JVM, Java bytecode'u çalıştıran bir sanal makinedir.
JDK, JRE ve JVM arasındaki farklar:

<figure><img src="assets/tables/unnamed (9).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>Java’da primitiv, nonprimitiv tipler ve wrapper class nedir?
?</summary>

Non-Primitive Type'larin Bellek Adresleri stack'te saklanir. içerikleri Heap'de saklanir
Primitive Type'lara ulasmak, Non-Primitive type'lara göre daha hazlidar.
Non-Primitive Type'lar null degerini alabilirler.
Non-Primitive Type'larin bellekte tuttuklari alanlar degiskenlik gösterebilir.
Non-Primitive Type'Larin kullanilmayanlari Garbage Collector tarafindan toplanir.
Wrapper class, Java'da ilkel (primitive) veri tiplerini nesne olarak kullanmamızı sağlayan özel sınıflar.
İlkel veri tipleri (int, double, char, boolean, vb.) bellek yönetimi ve bazı işlemler açısından kısıtlamalara sahiptir. Wrapper class'lar ise bu kısıtlamaları aşmamızı ve ilkel veri tiplerini nesneler gibi kullanmamızı mümkün kılar.
Wrapper class'ların başlıca özellikleri:
Her ilkel veri tipine karşılık bir wrapper class vardır (Integer, Double, Character, Boolean, vb.).
Wrapper class'lar, new operatörü ile ilkel veri tiplerinden ve String'lerden oluşturulabilir.
Wrapper class'lar çeşitli metotlar ve sabitler içerir. Bu metotlar, string dönüşümü, aritmetik işlemler, karşılaştırma işlemleri gibi işlemleri gerçekleştirmemizi sağlar.
Wrapper class'lar nesne oldukları için Java'nın nesneye yönelik programlama (OOP) özelliklerini kullanmamızı sağlarlar (özellikleri, metotları, kalıtım, polimorfizm).
Wrapper class'ların faydaları:
İlkel veri tiplerine nesne özelliklerini kazandırır.
Nesnelere özgü işlemleri ilkel veri tipleri üzerinde yapabilmemizi sağlar.
Java'nın OOP özelliklerini ilkel veri tipleri üzerinde kullanmamızı mümkün kılar.
String türünden verileri ilkel veri tiplerine dönüştürmemizi ve tersini yapmamızı sağlar.

// int -> Integer
int sayi = 10;
Integer yeniSayi = new Integer(sayi);

// String -> Integer
String metin = "20";
Integer metinSayi = Integer.parseInt(metin);

// Integer -> String
String yeniMetin = yeniSayi.toString();

// Integer üzerinde metot kullanımı
boolean sonuc = yeniSayi.equals(20);

</details>

<details>

<summary>Java’da pointer kavramı neden yoktur?
?</summary>

Java'da pointer kavramının olmamasının birkaç sebebi vardır:

1. Güvenlik: Pointer'lar, bellek erişimi üzerinde doğrudan kontrol sağlayarak programcıların bellek hataları yapmasına ve sistemin çökmesine yol açabilir. Java, pointer'lar yerine referanslar kullanarak bu riski azaltmayı amaçlar. Referanslar, bellek adreslerini doğrudan değil, nesnelere olan erişimleri temsil eder. Bu sayede bellek hatalarının önüne geçilmiş olur.
2. Otomatik bellek yönetimi: Java, garbage collector (çöp toplama) mekanizması ile bellek yönetimini otomatik hale getirir. Pointer'lar ile bellek yönetimi programcıya bırakıldığında, bellek sızıntıları ve diğer bellek hataları oluşabilir. Garbage collector, kullanılmayan nesneleri otomatik olarak bellekten silerek bellek sızıntılarını önler.
3. Basitleştirilmiş programlama: Pointer'lar, karmaşık ve hata yapmaya açık bir kodlama stili teşvik eder. Java, referanslar ve garbage collector ile programlamayı basitleştirmeyi ve programcıların bellek yönetimi ile uğraşmak zorunda kalmamalarını amaçlar.
4. Platform bağımsızlığı: Pointer'lar, farklı platformlarda farklı bellek adresleme şemaları kullandığından platform bağımsız programlama için uygun değildir. Java, bytecode ve JVM gibi platform bağımsız teknolojiler kullanarak bu sorunu aşar.
5. Nesneye dayalı programlama: Java, nesneye dayalı programlama diline odaklanır. Pointer'lar ise nesneye dayalı programlamanın temel ilkeleri ile tam olarak uyumlu değildir.
   Özetle: Java'da pointer kavramının olmaması, dilin güvenliğini, otomatik bellek yönetimini, basitleştirilmiş programlamayı, platform bağımsızlığı ve nesneye dayalı programlama ilkelerini desteklemek için bir tercihtir.
   Bazı durumlarda pointer'lara ihtiyaç duyulabilir:
   Düşük seviyeli sistem programlama
   Donanım ile doğrudan etkileşim
   Performans optimizasyonu
   Ancak bu gibi durumlarda bile, Java'da NIO (Non-Blocking I/O) gibi alternatif çözümler tercih edilebilir.
   Not: Java'da pointer'ların olmamasının bazı dezavantajları da vardır. Örneğin, bazı işlemler için daha fazla kod yazmak gerekebilir.
   Pointer'ların kullanımının gerekli olup olmadığını ve alternatif çözümlerin varlığını değerlendirmek önemlidir.

</details>

<details>

<summary>Java pass by value mudur pass by reference midir ve bunların farkı nedir??</summary>

Java, pass by value yöntemini kullanır. Bu, bir metoda parametre olarak bir değişken gönderildiğinde, metodun yalnızca değişkenin değerinin bir kopyasını aldığı anlamına gelir. Metot, değişkenin değerini değiştirebilir, ancak bu değişiklik, metottan çıkıldığında kaybolur.
Pass by reference ise, bir metoda parametre olarak bir değişken gönderildiğinde, metodun değişkenin referansını aldığı anlamına gelir. Metot, değişkenin değerini değiştirebilir ve bu değişiklik, metottan çıkıldığında da kalıcı olur.
Pass by value ve pass by reference arasındaki farklar:

<figure><img src="assets/tables/unnamed (12).png" alt=""><figcaption></figcaption></figure>

Pass by value'nun avantajları:
Daha hızlı olabilir.
Daha güvenli olabilir.
Kodun daha okunabilir ve anlaşılır olmasını sağlayabilir.
Pass by value'nun dezavantajları:
Bazı durumlarda daha fazla kod yazmak gerekebilir.
Değişkenin değerini metottan sonra da değiştirmek istendiğinde uygun değildir.
Pass by reference'ın avantajları:
Değişkenin değerini metottan sonra da değiştirmek için uygundur.
Bazı durumlarda daha az kod yazmak gerekebilir.
Pass by reference'ın dezavantajları:
Daha yavaş olabilir.
Daha az güvenli olabilir.
Kodun daha az okunabilir ve anlaşılır olmasını sağlayabilir.
Örnek:
public class PassByValue {

    public static void main(String[] args) {
        int x = 10;
        System.out.println("Değişkenin değeri main metodunda: " + x);
        degistir(x);
        System.out.println("Değişkenin değeri main metodunda: " + x);
    }

    public static void degistir(int y) {
        y = 20;
        System.out.println("Değişkenin değeri degistir metodunda: " + y);
    }

}
Bu örnekte, degistir metodu x değişkenini parametre olarak alır. Metot içinde x değişkeninin değeri 20 olarak değiştirilir. Ancak, metottan çıkıldığında x değişkeninin değeri hala 10'dur.

</details>

<details>

<summary>Java’da static keywordü nedir??</summary>

Static keywordü sınıfa ait degiskenler için kullanılır.
Yani static olan bir method'a ya da bir field'a Class adiyla doğrudan erişilebilir.
Nesne adayla da ulaşılabilir ama best practice degildir.
Static metodlar override edilmezler.
JVM her ayaga kalktiginda static değişkenler, tetiklensin ya da tetiklenmesi
uygulama context in içerisine yüklenir.
JVM' in heap alanindaki perm gen/metaspace alanina yerlesir.
Class'lar static keywordü ile imlenemezler. Yani Class'lar static olmazlar.

</details>

<details>

<summary>Java’da final keyword nedir??</summary>

Final olan bir sey finaldir. Yani degistirilemez.
Final olan Class'lar extend edilemezler.
Final olan metodlar override edilemezler.
Final olan bir field için ya baslangic degeri verilmeli, ya da constructorlarda
ilk deger atamasi yapilmalidir.

</details>

<details>

<summary>Java’da constructor metodlar nedir?
?</summary>

Nesne oluşturulduğunda çağrılan metotlar constructor metodlar denir.
Genellikle public tir.
Class adayla Constructor method adi ayna olmak zorunda.
Geriye değer döndürmezler.
Parametre alabilirler.
Bir Class'ta birden fazla constructor bulunabilir.
Bir Class oluşturduğumuzda constructor method tanimlamadlysak, arka tarafta
Bir tane parametre almayan constructor bizim için olusturulur.

</details>

<details>

<summary>Java’da Composition Aggretion olaylarını açıklayıp karşılaştırınız
?</summary>

Composition ve Aggregation Karşılaştırması
Composition ve aggregation, nesneye dayalı programlamada nesneler arasındaki ilişkileri tanımlamak için kullanılan iki önemli kavramdır. Her iki kavram da bir nesnenin diğer nesnelerle nasıl ilişkilendirilebileceğini tanımlar, ancak aralarında bazı önemli farklılıklar bulunur.
Composition:
Bir nesnenin diğer nesnelerden oluştuğunu ifade eder.
Sahip olma ve parçalar-bütün ilişkisi içerir.
Bütün nesne yok olduğunda, parçalar da yok olur.
Daha güçlü bir ilişkidir.
Bir nesne, birden fazla bileşene sahip olabilir.
Bileşenler, tek başına var olamazlar.
Genellikle "bir şeyin parçası olma" anlamında kullanılır.
Örnek: Bir araba nesnesi, motor, tekerlek ve şanzıman gibi bileşen nesnelerden oluşur. Araba yok olduğunda, bu bileşenler de yok olur.
Aggregation:
Bir nesnenin diğer nesnelerle ilişkili olduğunu ifade eder.
Kullanım veya bağımlılık ilişkisi içerir.
Nesneler birbirinden bağımsızdır.
Daha zayıf bir ilişkidir.
Bir nesne, birden fazla nesneyle ilişkilendirilebilir.
Nesneler, tek başına var olabilirler.
Genellikle "bir şeyle ilişkili olma" anlamında kullanılır.
Örnek: Bir kütüphane nesnesi, kitap nesneleriyle ilişkilidir. Kütüphane yok olduğunda, kitaplar hala var olur.
Farklılıklar:

<figure><img src="assets/tables/unnamed (25).png" alt=""><figcaption></figcaption></figure>

Hangi durumda hangisi kullanılır?
Bir nesnenin diğer nesnelerden oluştuğu durumlarda composition kullanılır.
Bir nesnenin diğer nesnelerle ilişkili olduğu durumlarda aggregation kullanılır.

</details>

<details>

<summary>Java’da neden inheritance yerine composition tercih edilmelidir?
?</summary>

Java'da inheritance yerine composition tercih edilmesinin birçok sebebi vardır:
Esneklik: Composition, inheritance'dan daha fazla esneklik sağlar. Inheritance'da bir sınıf sadece bir üst sınıftan miras alabilirken, composition'da bir sınıf birden fazla sınıftan özellik ve davranışları birleştirebilir.
Bağımlılıklar: Composition, inheritance'dan daha az bağımlılık oluşturur. Inheritance'da bir alt sınıf, üst sınıftaki değişikliklere bağlıdır. Composition'da ise bir sınıf, kullandığı diğer sınıfların değişikliklerine daha az bağlıdır.
Kod tekrarı: Composition, inheritance'dan daha az kod tekrarına yol açar. Inheritance'da birden fazla alt sınıf aynı özelliği veya davranışı miras alırsa, kod tekrarı oluşur. Composition'da ise bu özellikler veya davranışlar tek bir sınıfta tanımlanıp birden fazla sınıf tarafından kullanılabilir.
Bakım kolaylığı: Composition, inheritance'dan daha kolay bakımı olan kodlar oluşturur. Inheritance'da bir sınıfın değiştirilmesi, diğer alt sınıfları da etkileyebilir. Composition'da ise bir sınıfın değiştirilmesi, sadece o sınıfı ve onu kullanan diğer sınıflara etki eder.
Güvenlik: Composition, inheritance'dan daha güvenli kodlar oluşturabilir. Inheritance'da bir alt sınıf, üst sınıftaki private üyelere erişebilir. Composition'da ise bir sınıf, kullandığı diğer sınıfların private üyelerine erişemez.
Bazı durumlarda inheritance kullanmak gerekli olabilir:
Bir sınıf, bir üst sınıfın tüm özelliklerini ve davranışlarını miras almak istiyorsa.
Bir sınıf, bir üst sınıfın soyut metotlarını implemente etmek istiyorsa.
Ancak, genel olarak composition, inheritance'dan daha tercih edilen bir tekniktir. Composition, daha fazla esneklik, daha az bağımlılık, daha az kod tekrarı, daha kolay bakım ve daha güvenli kodlar oluşturmayı sağlar.
Composition'ın bazı dezavantajları da vardır:
Composition, inheritance'dan daha karmaşık olabilir.
Composition, inheritance'dan daha fazla kod yazmayı gerektirebilir.
Ancak, composition'ın faydaları genellikle dezavantajlarından daha fazladır.
Inheritance ve composition'ın nasıl kullanılacağı, programın gereksinimlerine göre belirlenir.

</details>

<details>

<summary>Java’da upcasting downcasting nasıl yapılır??</summary>

Upcasting (Yukarı Çevirim): Bir alt sınıf nesnesini, üst sınıfın bir nesne türüne atama işlemidir. Otomatik olarak gerçekleşir ve herhangi bir ek işleme gerek yoktur.
Örnek:

public class Animal {

    public void speak() {
        System.out.println("Hayvan ses çıkarıyor.");
    }

}

public class Dog extends Animal {

    @Override
    public void speak() {
        System.out.println("Havlıyor.");
    }

}

public class Main {

    public static void main(String[] args) {
        Dog dog = new Dog();
        Animal animal = dog; // Upcasting

        animal.speak(); // Hayvan ses çıkarıyor. (Dog'un speak metodu değil, Animal'ın speak metodu çalışır.)
    }

}

Downcasting (Aşağı Çevirim): Bir üst sınıf nesnesini, alt sınıfın bir nesne türüne dönüştürme işlemidir. Açıkça yapılmalıdır ve (AltSınıfAdı) şeklinde bir tür dönüşümü kullanılır.
Örnek:
Java
public class Animal {

    public void speak() {
        System.out.println("Hayvan ses çıkarıyor.");
    }

}

public class Dog extends Animal {

    @Override
    public void speak() {
        System.out.println("Havlıyor.");
    }

}

public class Main {

    public static void main(String[] args) {
        Animal animal = new Dog();
        Dog dog = (Dog) animal; // Downcasting

        dog.speak(); // Havlıyor. (Dog'un speak metodu çalışır.)
    }

}

Downcasting'te dikkat edilmesi gerekenler:
Downcasting her zaman güvenli değildir. Dönüştürülen nesne, istenilen alt sınıfın bir örneği değilse, ClassCastException hatası oluşur.
Downcasting'ten önce, nesnenin istenilen alt sınıfın bir örneği olup olmadığını kontrol etmek önemlidir. Bunu instanceof operatörü ile yapabilirsiniz.
Örnek:
Java
public class Animal {

    public void speak() {
        System.out.println("Hayvan ses çıkarıyor.");
    }

}

public class Dog extends Animal {

    @Override
    public void speak() {
        System.out.println("Havlıyor.");
    }

}

public class Main {

    public static void main(String[] args) {
        Animal animal = new Dog();

        if (animal instanceof Dog) {
            Dog dog = (Dog) animal;
            dog.speak(); // Havlıyor.
        } else {
            System.out.println("Nesne bir Dog örneği değil.");
        }
    }

}

</details>

<details>

<summary>Java’da  polymorphism runtime’a mı çalışır compiler time’da mı çalışır??</summary>

Java'da polymorphism hem runtime'da hem de compile time'da çalışır.
Compile time polymorphism:
Overloading, compile time'da gerçekleşir. Compiler, metodun hangi versiyonunun çağrılacağını parametrelere göre belirler.
Inheritance, compile time'da gerçekleşir. Compiler, alt sınıfın hangi özelliklere ve davranışlara sahip olacağını belirler.
Runtime polymorphism:
Overriding, runtime'da gerçekleşir. Metot hangi nesne üzerinde çağrılırsa, o nesnenin metodu çalışır.
Upcasting ve downcasting, runtime'da gerçekleşir. Nesneler runtime'da dönüştürülür.
Özetle:
Overloading ve inheritance hem compile time'da hem de runtime'da çalışır.
Overriding ve upcasting/downcasting sadece runtime'da çalışır.
Polymorphism, Java'da önemli bir programlama tekniğidir. Kodun daha az tekrarlı, daha okunabilir, daha esnek ve daha bakımı kolay olmasını sağlar.

</details>

<details>

<summary>Java’da Dynamic Binding-Late Binding / Static Binding-Early Binding nedir? 
?</summary>

Java'da Dynamic Binding ve Static Binding (Geç Bağlantı ve Erken Bağlantı)
Java'da yöntem çağrımları, iki farklı bağlama mekanizması kullanılarak gerçekleştirilebilir: static binding (erken bağlama) ve dynamic binding (geç bağlama). Bu mekanizmalar, hangi metodun çalıştırılacağının nasıl kararlaştırıldığını etkiler.
Static Binding (Erken Bağlantı):
Compile time'da gerçekleşir.
Compiler, programı derlerken hangi metodun çağrılacağını belirler.
Hangi nesne üzerinde çağrılırsa çağrılsın, aynı isim ve imzalı metot çalışır.
Genellikle private metotlar ve final metotlar için kullanılır.
Örnek:
Java
public class StaticBinding {
public void print() {
System.out.println("Static Binding");
}

    public static void main(String[] args) {
        StaticBinding obj = new StaticBinding();
        obj.print(); // Static Binding metodu çalışır.
    }

}

Dynamic Binding (Geç Bağlantı):
Runtime'da gerçekleşir.
Metot hangi nesne üzerinde çağrılırsa, o nesnenin metodu çalışır.
Inheritance ve polymorphism ile birlikte kullanılır.
Genellikle public metotlar ve non-final metotlar için kullanılır.
Örnek:
Java
public class Animal {
public void speak() {
System.out.println("Animal ses çıkarıyor.");
}
}

public class Dog extends Animal {
@Override
public void speak() {
System.out.println("Havlıyor.");
}
}

public class Main {
public static void main(String[] args) {
Animal animal = new Dog();
animal.speak(); // Havlıyor. (Dog'un speak metodu çalışır.)
}
}

Static binding tercih edildiği durumlar:
Performans önemli olduğunda static binding daha hızlı olabilir.
Güvenlik gerektiğinde static binding daha güvenli olabilir.
Dynamic binding tercih edildiği durumlar:
Polymorphism kullanmak gerektiğinde dynamic binding gereklidir.
Kodun daha esnek ve bakımı kolay olması istendiğinde dynamic binding tercih edilir.
Özetle:
Static binding compile time'da, dynamic binding runtime'da gerçekleşir.
Static bindingde hangi metot çağrılacağı derleme sırasında bellidir, dynamic bindingde runtime'da karar verilir.
Java, inheritance ve polymorphism gibi özellikleri desteklemek için dynamic binding mekanizmasını kullanır.
Hangi bağlama mekanizmasının kullanılacağı, programın gereksinimlerine göre belirlenir.

ek bilgi: static metotlar override edilmezler, derleme zamanı bind edilirler.

</details>

<details>

<summary>Java’da abstrack class’lar hakkında bilgi verir misin?
?</summary>

Abstract class'lar birbirleriyle benzer sınıflar bir çati altinda toplamak için kullanılırlar..
İnterfaceler birbirleriyle benzemeyen, farkli siniflar bir çatı altinda toplamak için kullanılırlar
Abstract class lardan ve interface lerden nesne üretemezler.
Abstract class'larin kendi constructorlari olabilir ama, interface'lerin kendi constructorlari olamaz.
Abstract class'ların kendi fieldlar olabilir, interface Lerin de kendi fieldları olabilir ama final olmak
zorundadır ve başlangıç değerleri olmalıdır. Bu fieldlar ayni zamanda default olarak olarak public ve static tir.
Bir class, bir interface’i ya da bir abstract class ı implement/extend ettiğinde ilgili abstract class in ya da
interface in içi bos metodlar override etmek zorundadır.
Bir class, bir abstract classı extend edebilir ama birden fazla interface'i implements edebilir.
Bir interface baska bir interface'i extend eder. Ve bir interface birden fazla interface'i extend edebilir.

Bir abstract class in içerisinde birden fazla abstract method olabilir / hiç abstract method olmayadabilir.
Bir interface in içerisinde de abstract method olabilir / hiç abstract method olmayadabilir
Java 8'den sonra private-static-default anahtar kelimeleriyle bir interface içerisine içi dolu method yazilabilir.
Bir interface, bir class ı ya da bir abstract class ı extend alamaz. Ama bir abstract class, bir Class'ı extend
edebilir.
Eger bir interface'in sadece bir tane içi boş metodu varsa, bu interface lere Functional İnterface Ler denir. Eger
bir interface in hig bir içi boş metodu yok ise, bu interface lere Marker İnterface Ler denir.

</details>

<details>

<summary>Elimizde bir abstract class var. Bu abstract class'in bütün metodlarını public ve abstract yaparsam ne olur.??</summary>

Teknik olarak basima ne gelir?
Bir abstract class'ın bütün metodlarını public ve abstract olarak yaparsanız, aşağıdaki sonuçlar ortaya çıkar:
Teknik açıdan:
Soyut bir sınıfın tüm metotları public ve abstract olursa, o sınıf bir interface'e dönüşür.
Interface'ler, soyut sınıflara benzer şekilde davranır, ancak sadece soyut metotlar ve sabit değerler içerebilir.
Interface'ler, birden fazla sınıftan miras alınabilir ve bir sınıfta birden fazla interface kullanılabilir.
Kodlama açısından:
Abstract class'ın tüm metotlarını public ve abstract yapmak, kodunuzu daha açık ve okunabilir hale getirir.
Interface'ler, kodunuzu daha modüler ve tekrar kullanılabilir hale getirir.
Interface'ler, kodunuzu daha soyut ve genel hale getirir.
Bazı dezavantajlar:
Abstract class'ın tüm metotlarını public ve abstract yapmak, kodunuzu biraz daha karmaşık hale getirebilir.
Interface'ler, metodun gövdesini içeremez, bu nedenle metodun nasıl uygulanacağını her alt sınıfın kendisinin belirlemesi gerekir.
Özet:
Bir abstract class'ın tüm metotlarını public ve abstract yapmak, o sınıfı bir interface'e dönüştürür. Bu, kodunuzu daha açık, okunabilir, modüler, tekrar kullanılabilir, soyut ve genel hale getirebilir. Ancak, kodunuzu biraz daha karmaşık da hale getirebilir.
Hangi seçeneğin daha iyi olduğu, programınızın gereksinimlerine bağlıdır.
Ek bilgiler:
Abstract class'lar, birden fazla sınıftan miras alınamaz.
Abstract class'lar, somut metotlar da içerebilir.
Interface'ler, sınıflar gibi nesneler oluşturamaz.

</details>

<details>

<summary>Abstract Class ve Interface farkları nelerdir??</summary>

1-) Bir sınıf birden fazla interface’i inherit olarak alabilir ama bir sınıfa bir tane abstract class inherit alınabilir.
2-) Interface içerisinde boş metodlar tanımlanabilir ama abstract class’larda hem boş metodlar tanımlanabilir hemde içi dolu metodlar tanımlabilir.
3-) Abstract classları kullanmak hız açısından avantaj sağlar.
4-) Interface de yeni bir metod yazdığımız zaman bu interfaceden implement ettiğimiz tüm classlarda bu metodun içini tek tek doldurmak gerekiyor ancak abstract classlarda durum farklıdır burada bir metod tanımlayıp içini doldurduğumuzda abstract sınıfımızdan türetilmiş bütün sınıflar bu özelliği kazanmış olur.
5-) Interfaceler çoklu kalıtımı sağlamaya yardımcı abstract classlar ise çoklu kalıtımı desteklemez.
6-) Interface içerisindeki tüm nesnelerin “public” olması gerekirken Abstract classlarda tüm öğelerin “public” olması zorunlu değildir.
7-) Interface yapıcı metotlar(constructor) içermez. Abstract class yapıcı metotlar içerebilir.
8-)Interface metotlar static olamaz. Abstract class soyut olmayan metodlar static olarak tanımlanabilir.

</details>

<details>

<summary>Öyle bir yapı tasarlayın ki interface i implemente eden class ilgili interface in metodunu override etmek zorunda kalmasın.?</summary>

Bir interface'in metodlarını override etmeden kullanmak için iki temel yöntem vardır:

1. Default Metotlar:
   Java 8'den beri, interface'ler default metotlar tanımlayabilir. Bu metotlar, bir gövdeye sahiptir ve alt sınıflar tarafından override edilebilir. Bir alt sınıf, default metodu override etmezse, interface'deki default metot kullanılır.
   Örnek:
   Java
   public interface MyInterface {
   default void myMethod() {
   System.out.println("Default metot");
   }
   }

public class MyClass implements MyInterface {
// myMethod'u override etmiyoruz.
}

public class Main {
public static void main(String[] args) {
MyClass obj = new MyClass();
obj.myMethod(); // "Default metot" yazdırır.
}
}

2. Static Metotlar:
   Java 8'den beri, interface'ler static metotlar da tanımlayabilir. Static metotlar, bir nesneye ihtiyaç duymadan doğrudan interface üzerinden çağrılabilir.
   Örnek:
   Java
   public interface MyInterface {
   static void myStaticMethod() {
   System.out.println("Static metot");
   }
   }

public class MyClass implements MyInterface {
}

public class Main {
public static void main(String[] args) {
MyInterface.myStaticMethod(); // "Static metot" yazdırır.
}
}

Hangi yöntemin kullanılacağı, programınızın gereksinimlerine bağlıdır.
Default metotlar:
Daha fazla esneklik sağlar.
Alt sınıfların, override ederek metodun davranışını değiştirmesine izin verir.
Static metotlar:
Daha az kod yazımı gerektirir.
Nesneye ihtiyaç duymadan doğrudan interface üzerinden kullanılabilir.
Ek bilgiler:
Abstract class'lar da default ve static metotlar tanımlayabilir.
Interface'lerdeki default ve static metotlar, final olarak tanımlanmalıdır.
Umarım bu bilgiler yardımcı olmuştur!

</details>

<details>

<summary>Java’da serializable nedir
?</summary>

Java'da serializable, bir nesnenin byte dizisine dönüştürülüp, dosya veya ağ üzerinden aktarılabilme özelliğidir. Bu sayede nesne, farklı bir JVM'de de yeniden oluşturulabilir.
Serializable arayüzü:
Serializable özelliğini kullanmak için, nesnenin Serializable arayüzünü implemente etmesi gerekir.
Bu arayüz herhangi bir metot içermez, sadece bir marker interface görevi görür.
Nesne serileştirme:
Bir nesneyi serileştirmek için ObjectOutputStream sınıfı kullanılır.
ObjectOutputStream, nesnenin alanlarını ve durumunu byte dizisine dönüştürür.
Nesne deserializasyonu:
Serileştirilmiş bir nesneyi deserialize etmek için ObjectInputStream sınıfı kullanılır.
ObjectInputStream, byte dizisini nesneye dönüştürür.
Serializable'ın faydaları:
Nesnelerin depolanmasını ve taşınmasını kolaylaştırır.
Nesnelerin durumunu kalıcı hale getirir.
Farklı JVM'ler arasında nesne alışverişi yapmayı mümkün kılar.
Serializable'ın dezavantajları:
Güvenlik riskleri oluşturabilir.
Sınıfın uyumluluğunu zorlaştırabilir.
Serializable'ı ne zaman kullanmalıyız:
Nesnelerin depolanması veya taşınması gerekiyorsa.
Nesnelerin durumunun kalıcı hale getirilmesi gerekiyorsa.
Farklı JVM'ler arasında nesne alışverişi yapılması gerekiyorsa.
Serializable'ı ne zaman kullanmamalıyız:
Nesnenin güvenli olması gerekiyorsa.
Sınıfın uyumluluğunun korunması gerekiyorsa.
Serializable'ın alternatifleri:
Externalizable arayüzü
JSON veya XML gibi formatlar
Umarım bu bilgiler yardımcı olmuştur!

</details>

<details>

<summary>Java’da Immutable,?</summary>

bir nesnenin degismezligi anlamina gelir.
Yani herhangi bir şekilde değiştirilemez.
Bir Class'in immutable olmasi için,
final olarak imlenmesi lazim.
Set metotlarının olmamasi lazim.
Deep Copy / Shallow Copy uygulanmasi lazim.

</details>

<details>

<summary>Java'da Map Yapıları?</summary>

Map, anahtar-değer çiftlerini depolamak için kullanılan bir veri yapıdır. Anahtarlar benzersizdir ve her anahtar bir değere eşlenir.
Java'da map oluşturmak için:
HashMap: En yaygın kullanılan map türüdür. Hızlı ve verimlidir.
TreeMap: Anahtarların sıralı olmasını sağlar.
LinkedHashMap: Ekleme sırasını korur.
WeakHashMap: Anahtarların bellekten silinmesine izin verir.
Map'te temel işlemler:
put(key, value): Bir anahtar-değer çifti ekler.
get(key): Bir anahtara bağlı değeri döndürür.
remove(key): Bir anahtara bağlı değeri siler.
containsKey(key): Bir anahtarın map'te olup olmadığını kontrol eder.
isEmpty(): Map'in boş olup olmadığını kontrol eder.
size(): Map'te kaç tane anahtar-değer çifti olduğunu döndürür.
Map'i dolaşmak için:
forEach(): Map'teki her anahtar-değer çifti için bir kod bloğu çalıştırır.
entrySet(): Map'teki tüm girişlerin bir setini döndürür.
keySet(): Map'teki tüm anahtarların bir setini döndürür.
values(): Map'teki tüm değerlerin bir koleksiyonunu döndürür.

Map'i kullanmanın faydaları:
Anahtar-değer çiftlerini depolamak için idealdir.
Hızlı ve verimlidir.
Sıralama ve ekleme sırası gibi özel işlevler sunan farklı map türleri mevcuttur.
Map'i kullanmanın dezavantajları:
Anahtarların benzersiz olması gerekir.
Sıralama ve ekleme sırası gibi özel işlevler, performansı etkileyebilir.
Map'e alternatifler:
List: Anahtar-değer çiftleri sıralı bir şekilde depolanmak istendiğinde kullanılabilir.
Set: Anahtarların benzersiz olması ve sıralı olmaması gerektiğinde kullanılabilir.

</details>

<details>

<summary>Java’da cache nasıl çalışır?
?</summary>

Java'da caching, verileri bellekte saklayarak tekrarlayan erişimleri hızlandırma tekniğidir. Bu, veritabanı sorguları, dosya sistemi işlemleri veya hesaplama yoğun işlemler gibi pahalı işlemler için erişim süresini önemli ölçüde azaltabilir.
Java'da caching'in temel prensibi:
Bir veri ilk defa erişildiğinde, bellekten okunur ve cache'e kopyalanır.
Aynı veriye tekrar erişildiğinde, veritabanından veya dosya sisteminden tekrar okunmak yerine cache'den okunur.
Cache'de yer kalmadığında, en az kullanılan veri silinir ve yeni veri için yer açılır.
Java'da caching'i uygulamak için:
Cache API'si: Java, java.util.concurrent.ConcurrentHashMap gibi önceden hazırlanmış cache API'leri sunar. Bu API'ler, verileri ekleme, alma ve silme gibi temel işlemleri gerçekleştirmek için kullanışlı yöntemler sağlar.
Üçüncü taraf kütüphaneler: Guava ve Ehcache gibi popüler üçüncü taraf kütüphaneler, daha gelişmiş caching işlevleri sunar. Bu kütüphaneler, TTL (time to live) ve LRU (least recently used) gibi cache eviction politikaları belirlemenize ve cache istatistiklerini izlemenize olanak tanır.
Java'da caching'in faydaları:
Performans artışı: Verilere erişim süresini azaltarak uygulamanızın performansını önemli ölçüde artırabilir.
Ölçeklenebilirlik: Veritabanı yükünü azaltarak uygulamanızın daha fazla kullanıcıyı ve iş yükünü kaldırabilmesine yardımcı olabilir.
Kullanılabilirlik: Veritabanı erişimi kesintiye uğrasa bile uygulamanızın çalışmaya devam etmesini sağlayabilir.
Java'da caching'in dezavantajları:
Bellek kullanımı: Cache'de saklanan veriler bellek kullanımı artırır.
Tutarlılık: Veriler güncellendiğinde cache'deki eski veriler tutarsız hale gelebilir.
Karmaşıklık: Cache'i doğru şekilde yapılandırmak ve yönetmek karmaşık olabilir.

</details>

<details>

<summary>+Idempotency Nedir?
?</summary>

Idempotency, bir işlemin birden fazla kez aynı sonucu vermesi anlamına gelir. Yani, bir işlemi bir veya birden fazla kez tekrarlamak, sonucu etkilemez.
Örnek:
Bir banka hesabına para yatırma işlemi idempotenttir. Birden fazla kez para yatırmak, hesaptaki bakiyeyi aynı şekilde artırır.
Bir e-posta gönderme işlemi idempotenttir. Aynı e-postayı birden fazla kez göndermek, alıcının gelen kutusunda birden fazla kopyası oluşmasına neden olur.
Idempotency'nin faydaları:
Hatalara karşı koruma sağlar. Bir işlem idempotent ise, bir hata oluşması durumunda işlem tekrarlanabilir ve aynı sonuca ulaşılabilir.
Performansı artırır. Bir işlem idempotent ise, birden fazla kez tekrarlanmak zorunda kalmaz.
Kullanımı kolaylaştırır. Bir işlem idempotent ise, kullanıcılar işlemin birden fazla kez tekrarlanmasından endişe duymadan kullanabilirler.
Idempotency'nin sağlanması:
İşlemin mantığını dikkatlice tasarlayarak. İşlem, her seferinde aynı sonucu verecek şekilde tasarlanmalıdır.
Doğru veri yapıları ve algoritmalar kullanarak. İşlem, idempotent veri yapıları ve algoritmalar kullanmalıdır.
Tekrarlanan istekleri kontrol ederek. Bir işlem idempotent olsa bile, tekrarlanan istekleri kontrol etmek ve gereksiz işlemleri önlemek önemlidir.
Idempotency'nin kullanıldığı bazı durumlara örnek:
Finansal işlemler
E-ticaret işlemleri
Otomasyon sistemleri
Idempotency, birçok farklı alanda kullanılabilecek önemli bir kavramdır. Bir işlemin idempotent olmasını sağlayarak, hatalara karşı koruma sağlayabilir, performansı artırabilir ve kullanımı kolaylaştırabilirsiniz.

</details>

<details>

<summary>Stateless ve statefull nedir?
?</summary>

Bilgisayar bilimlerinde, "stateless" ve "stateful" terimleri, bir sistemin veya bileşenin işleyiş şeklini tanımlamak için kullanılır. Bunlar arasındaki temel fark, sistemin geçmiş etkileşimleri hakkında bilgi saklama konusundaki yaklaşımlarıdır.
Stateless:
Tanım: Stateless sistemler, her istekte gerekli tüm bilgileri alır ve bu bilgiye dayanarak bir yanıt üretir. Geçmiş etkileşimlerle ilgili herhangi bir bilgiyi saklamaz.
Özellikler:
Her istek bağımsızdır.
Ölçeklenebilirlik kolaydır.
Hata toleransı yüksektir.
Güvenlik açısından daha avantajlıdır.
Kullanıcı oturumları gibi durum bilgisi gerektiren işlemleri gerçekleştiremez.
Örnekler:
Web sunucuları (her HTTP isteği bağımsızdır)
API'ler (her API çağrısı gerekli parametreleri içerir)
DNS sunucuları (her sorgu için IP adresi döner)
Stateful:
Tanım: Stateful sistemler, geçmiş etkileşimlerle ilgili bilgileri saklar ve bir sonraki istekleri işleme koyarken bu bilgileri kullanır.
Özellikler:
Kullanıcı oturumlarını yönetebilir.
Alışveriş sepeti gibi uygulama içi durum bilgilerini saklayabilir.
Daha karmaşık işlemleri gerçekleştirebilir.
Ölçeklenebilirlik daha zordur.
Hata toleransı daha düşüktür.
Güvenlik açısından daha dikkatli yönetilmelidir.
Örnekler:
E-ticaret uygulamaları (alışveriş sepeti tutulur)
Sosyal medya platformları (kullanıcı oturumları)
Online oyunlar (oyun durumu saklanır)
Seçim Kriterleri:
Hangi yaklaşımı kullanacağınız, projenin ihtiyaçlarına bağlıdır. Eğer ölçeklenebilirlik, hata toleransı ve güvenlik sizin için öncelikli ise stateless yaklaşım daha avantajlı olabilir. Ancak kullanıcı oturumları veya durum bilgisi gerektiren işlemler için stateful yaklaşım tercih edilebilir.

</details>

<details>

<summary>Scale Down Yapmak Nedir?
?</summary>

Scale down, bir sistemin veya uygulamanın kapasitesini veya boyutunu küçültmek anlamına gelir. Bu, çeşitli nedenlerle yapılabilir:
Maliyetleri düşürmek: Daha az kaynak kullanarak maliyetleri düşürmek mümkündür.
Verimliliği artırmak: Daha az kaynak kullanarak daha fazla iş yapmak mümkündür.
Güvenilirliği artırmak: Daha az karmaşık bir sistem daha az hata yapma eğilimindedir.
Bakımı kolaylaştırmak: Daha küçük bir sistemin bakımı ve güncellenmesi daha kolaydır.
Scale down yapmanın birkaç yolu vardır:
Daha az kaynak kullanmak: Daha az CPU, RAM veya depolama alanı kullanmak mümkündür.
Daha az karmaşık bir sistem kullanmak: Daha az özellik veya işlev içeren bir sistem kullanmak mümkündür.
Daha az sayıda sunucu kullanmak: Daha az sayıda sunucu çalıştırarak kaynak kullanımını optimize etmek mümkündür.
Scale down yaparken dikkat edilmesi gerekenler:
Sistemin ihtiyaçlarını karşılamak için yeterli kapasiteyi korumak önemlidir.
Scale down işleminin sistemin performansı veya işlevselliği üzerinde olumsuz bir etkisi olmamalıdır.
Scale down işleminin geri döndürülebilir olması önemlidir.
Scale down yapmanın bazı örnekleri:
Bir web sitesinin daha az trafik aldığı zamanlarda sunucu sayısını azaltmak.
Bir uygulamanın daha az özellik içeren bir sürümünü kullanmak.
Bir veritabanının boyutunu küçültmek.
Scale down, bir sistemin veya uygulamanın kapasitesini veya boyutunu optimize etmek için kullanılabilecek bir tekniktir. Doğru şekilde yapıldığında, maliyetleri düşürmeye, verimliliği artırmaya ve güvenilirliği ve bakımı kolaylaştırmaya yardımcı olabilir.

</details>

<details>

<summary>Singleton Class Nedir & Nasıl Oluşturulur?
?</summary>

Singleton class, bir sınıftan sadece bir tane nesne oluşturulmasına ve bu nesnenin tüm uygulamada tek bir erişim noktası olarak kullanılmasına imkan veren bir tasarım desenidir.
Singleton class'ın faydaları:
Bellek tasarrufu sağlar. Bir sınıftan tek bir nesne oluşturulduğundan, bellek kullanımının optimize edilmesi sağlanır.
Tutarlılığı artırır. Tüm uygulamada tek bir nesne kullanıldığından, verilerin tutarlılığı ve bütünlüğü korunur.
Kodun daha kolay okunmasını ve anlaşılmasını sağlar. Bir sınıftan tek bir nesne oluşturulduğundan, kod daha basit ve daha anlaşılır hale gelir.
Singleton class'ın dezavantajları:
Esnekliği azaltır. Bir sınıftan tek bir nesne oluşturulduğundan, kodda değişiklik yapmak daha zor olabilir.
Test edilmesi daha zor olabilir. Bir sınıftan tek bir nesne oluşturulduğundan, singleton class'ı test etmek daha karmaşık olabilir.
Singleton Class Nasıl Oluşturulur?
Singleton class oluşturmak için aşağıdaki adımları takip edebilirsiniz:

1.  Sınıfı private veya protected olarak tanımlayın. Bu sayede, sınıftan nesne oluşturmak sadece sınıfın içinde mümkün olur.
2.  Sınıftan tek bir nesne oluşturan bir statik method oluşturun. Bu method, ilk çağrıldığında nesneyi oluşturmalı ve sonraki çağrılarda bu nesneyi döndürmelidir.
3.  Sınıfın nesnesine erişmek için public bir getter method oluşturun. Bu method, statik method tarafından oluşturulan nesneyi döndürmelidir.
4.  Sınıfın constructor'ını private olarak tanımlayın. Bu sayede, sınıftan nesne oluşturmak constructor üzerinden engellenir.
    Singleton class örneği:
    Python
    class Singleton:

        def __init__(self):
            # ...

        @staticmethod
        def getInstance():
            if not hasattr(Singleton, "_instance"):
                Singleton._instance = Singleton()
            return Singleton._instance

        def getSomeData(self):
            # ...

        def doSomething(self):
            # ...

# ...

singleton = Singleton.getInstance()
data = singleton.getSomeData()
singleton.doSomething()

Bu kodda, Singleton sınıfı bir singleton class olarak tanımlanmıştır. Sınıftan tek bir nesne oluşturmak için getInstance() static methodu kullanılır. Sınıfın nesnesine erişmek için getSomeData() ve doSomething() public methodları kullanılır.
Singleton class'ı oluştururken dikkat edilmesi gereken bazı noktalar şunlardır:
Sınıfı private veya protected olarak tanımlamak önemlidir.
Sınıftan tek bir nesne oluşturan bir statik method oluşturmak önemlidir.
Sınıfın nesnesine erişmek için public bir getter method oluşturmak önemlidir.
Sınıfın constructor'ını private olarak tanımlamak önemlidir.
Singleton class, bir sınıftan sadece bir tane nesne oluşturulması ve bu nesnenin tüm uygulamada tek bir erişim noktası olarak kullanılmasına imkan veren bir tasarım desenidir. Bu desen, bellek tasarrufu sağlar, tutarlılığı artırır ve kodun daha kolay okunmasını ve anlaşılmasını sağlar.

</details>

<details>

<summary>HashSet, LinkedHashSet ve TreeSet arasındaki farkları açıklayınız.
?</summary>

HashSet, LinkedHashSet ve TreeSet, Java'da bulunan ve hashing prensibi ile çalışan üç farklı veri setidir. Hepsi tekil değerler saklar ve hızlı arama işlemleri sunar. Aralarındaki temel farklar şunlardır:

1. Sıra:
   HashSet: Elemanlar rastgele sıralanır.
   LinkedHashSet: Elemanlar eklenme sırasına göre sıralanır.
   TreeSet: Elemanlar doğal sıralamalarına göre sıralanır (compareTo metodu kullanılarak).
2. Performans:
   HashSet: Ekleme ve silme işlemleri en hızlıdır.
   LinkedHashSet: Ekleme ve silme işlemleri HashSet'e göre biraz daha yavaştır.
   TreeSet: Ekleme ve silme işlemleri HashSet ve LinkedHashSet'e göre daha yavaştır.
3. Kullanım Alanları:
   HashSet: Tekil değerleri hızlı bir şekilde saklamak ve aramak için kullanılır.
   LinkedHashSet: Elemanların eklenme sırasını korumak ve hızlı bir şekilde aramak için kullanılır.
   TreeSet: Elemanları doğal sıralamalarına göre saklamak ve aramak için kullanılır.

Özetle:
HashSet: Hızlı ekleme ve silme işlemleri için idealdir.
LinkedHashSet: Elemanların eklenme sırasını korumak için idealdir.
TreeSet: Elemanları doğal sıralamalarına göre saklamak ve aramak için idealdir.
Aşağıdaki tabloda bu üç veri setinin karşılaştırılması daha net bir şekilde gösterilmiştir:

<figure><img src="assets/tables/unnamed (17).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>Javada Stream ve Collection arasındaki farkları açıklayınız.
?</summary>

Stream ve Collection, Java'da verileri işlemek için kullanılan iki farklı API'dir. Aralarında bazı önemli farklar vardır:

1. Veri Kaynağı:
   Stream: Verileri bir kaynaktan (dosya, veritabanı, koleksiyon vb.) alır ve işler.
   Collection: Verileri önceden bellekte tutulan bir koleksiyonda saklar ve işler.
2. İşleme Biçimi:
   Stream: Verileri tek tek işleyen ve işleme sırasında veri kaynağını tüketen fonksiyonel bir API'dir.
   Collection: Verileri bir bütün olarak işleyen ve veri kaynağını tüketmeyen imperatif bir API'dir.
3. Performans:
   Stream: Büyük veri kümeleri üzerinde çalışırken Collection'dan daha performanslı olabilir.
   Collection: Küçük veri kümeleri üzerinde çalışırken Stream'den daha performanslı olabilir.
4. Bellek Kullanımı:
   Stream: Verileri tek tek işlediği için Collection'dan daha az bellek kullanır.
   Collection: Verileri önceden bellekte tuttuğu için Stream'den daha fazla bellek kullanır.
5. Kullanım Alanları:
   Stream: Büyük veri kümeleri üzerinde filtreleme, haritalama, indirgeme gibi işlemleri gerçekleştirmek için idealdir.
   Collection: Küçük veri kümeleri üzerinde işlemler yapmak veya verileri sıralı bir şekilde tutmak için idealdir.
   Özetle:
   Stream: Büyük veri kümeleri üzerinde fonksiyonel bir şekilde işlem yapmak için idealdir.
   Collection: Küçük veri kümeleri üzerinde imperatif bir şekilde işlem yapmak için idealdir.
   Hangi API'yi kullanacağınız, uygulamanızın özel gereksinimlerine bağlıdır. Büyük veri kümeleri üzerinde işlem yapmanız gerekiyorsa Stream ideal bir seçimdir. Küçük veri kümeleri üzerinde işlem yapmanız veya verileri sıralı bir şekilde tutmanız gerekiyorsa Collection ideal bir seçimdir.
   Aşağıdaki tabloda bu iki API'nin karşılaştırılması daha net bir şekilde gösterilmiştir:
   <figure><img src="assets/tables/unnamed (16).png" alt=""><figcaption></figcaption></figure>

   Stream ve Collection'ı birlikte kullanmak da mümkündür. Örneğin, bir Collection'ı bir Stream'e dönüştürebilir ve Stream işlemlerini uyguladıktan sonra sonucu tekrar bir Collection'a dönüştürebilirsiniz.

</details>

<details>

<summary>Java Reflection nedir??</summary>

Java Reflection, bir Java programının çalışma zamanında kendi yapısını ve davranışını inceleyebilmesi ve manipüle edebilmesi için kullanılan bir mekanizmadır. Yani, bir Java kodu parçası çalışma esnasında kendi sınıflarını, metodlarını, alanlarını vb. öğrenebilir ve bunları dinamik olarak kullanabilir. Bu mekanizmanın çeşitli kullanım alanları vardır:

1. Metaprogramlama: Reflection, programın davranışını yazma zamanında değil çalışma zamanında belirlemek için kullanılabilir. Bu, dinamik ve esnek uygulamalar yazılmasına olanak tanır.
2. Frameworkler: Birçok framework, uygulamaların dinamik bir şekilde yüklenip yönetilmesi için Reflection'ı kullanır.
3. Test Araçları: Test araçları genellikle test senaryolarını tanımlamak ve yürütmek için Reflection'ı kullanır.
4. Introspection: Reflection, bir sınıfın yapısını ve özelliklerini incelemek için de kullanılabilir.
   Reflection ile neler yapılabilir?
   Bir sınıfın adını, metodlarını, alanlarını ve bunların erişim düzeylerini vb. bilgilerini almak.
   Metodları dinamik olarak çağırmak.
   Metod parametrelerine değer atamak.
   Alanlara değer okumak ve yazmak.
   Yeni nesneler oluşturmak.
   Sınıfın hiyerarşisini takip etmek.
   Reflection kullanımının dikkat edilmesi gereken noktalar:
   Reflection kullanımı güvenliksiz olabilir. Özel alanlara ve metodlara erişilmesine izin vermemek önemlidir.
   Reflection performansı etkileyebilir. Dinamik olarak yapılan işlemler statik olarak tanımlanmış işlemlerden daha yavaş olabilir.
   Reflection kodu karmaşık olabilir. Reflection kodunu yazmak ve anlamak zor olabilir.

</details>

<details>

<summary>Javada Shallow copy ve deep copy nedir?
?</summary>

Java'da bir nesneyi kopyalama, iki noktada farklılaşan iki yöntemle yapılabilir: Shallow Copy (Yüzeysel Kopyalama) ve Deep Copy (Detaylı Kopyalama). Her ikisi de farklı senaryolarda faydalıdır, ancak birbirlerinden önemli farklılıkları vardır.
Shallow Copy:
Shallow copy, bir nesnenin referanslarına kopyalama yapar. Yani, kopyalanan nesnedeki değerler, asıl nesnenin aynı bellek alanına işaret eder.
Bir örnek ile açıklamak gerekirse, iç içe geçmiş diziler ve nesneler içeren bir Person sınıfınız olduğunu düşünün. Shallow copy ile kopyaladığınız yeni Person nesnesinin, diğer nesne ve dizilere referansları asıl nesneyle aynı olacaktır. Değişiklik yaparsanız, bu değişiklikler her iki nesnede de görünür.
Avantajları: Hızlı ve bellek açısından tasarrufludur.
Dezavantajları: Değişiklikler orijinal nesneyi de etkiler. İç içe geçmiş yapılar kopyalanmadığından, derin yapısal değişiklikler istenmiyorsa uygun değildir.
Deep Copy:
Deep copy, bir nesnenin değerlerini kopyalar. Yani, kopyalanan nesnedeki değerler, asıl nesneden bağımsız yeni bellek alanlarına atanır. İç içe geçmiş diziler ve nesneler de tamamen bağımsız olarak kopyalanır.
Bir örnek ile açıklamak gerekirse, Deep copy ile kopyaladığınız Person nesnesinin diğer nesne ve dizilere referansları asıl nesneden farklı, yeni bellekte oluşturulan kopyalara yönlendirilir. Yani, her iki nesne birbirinden bağımsız olarak değiştirilebilir.
Avantajları: Değişiklikler orijinal nesneyi etkilemez. İç içe geçmiş yapılar da kopyalandığından, derin yapısal değişiklikler istendiğinde uygundur.
Dezavantajları: Hızlı ve bellek açısından daha masraflıdır.
Hangi copy yöntemini kullanmalısınız?
Eğer sadece basit veri tipleri (int, String vb.) içeren bir nesneyi kopyalıyorsanız Shallow Copy yeterlidir.
İç içe geçmiş yapılar içeren bir nesneyi kopyalarken ve her ikisini de birbirinden bağımsız olarak değiştirmek istiyorsanız Deep Copy kullanmalısınız.
Performans ve bellek kullanımı sizin için önemli faktörler ise, Shallow Copy'i tercih edebilirsiniz. Ancak bu durumda değişikliklerin asıl nesneyi de etkileyeceğini unutmayın.

</details>

<details>

<summary>Java Marker Interface - Marker Annotation nedir?
?</summary>

1. Marker Interface:
   Bir marker interface, herhangi bir metot ya da sabit içermeyen boş bir arayüzdür.
   Bir sınıfa uygulanan marker interface, o sınıfa ek bir bilgi eklemek için kullanılır. Bu bilgi daha sonra sınıfın davranışını etkilemek için reflection gibi mekanizmalar ile kullanılabilir.
   Marker interface'lerin kullanım alanları sınırlıdır ve günümüz Java uygulamalarında tercih edilmeyen bir yaklaşımdır. Çünkü bir interface'nin varlığı zaten bir bilgiyi temsil ederken, ekstra bir boş interface eklemek kod karmaşıklığına sebep olabilir.
2. Marker Annotation:
   Marker annotation, Java 5'ten itibaren kullanıma giren bir anotaysyon türüdür.
   Bir annotation, sınıflara, metodlara veya alanlara eklenebilen meta bilgi sağlayan bir yapıdır. Marker annotation ise herhangi bir değer ya da parametre almayan boş bir annotationdur.
   Marker annotation'lar, reflection gibi mekanizmalar ile sınıfın özelliklerini belirlemek için kullanılabilir.
   Günümüz Java uygulamalarında, marker interface yerine daha açıklayıcı ve kod okunurluğu sağlayan marker annotation kullanımı tercih edilir.
   Özetle:
   Marker interface ve marker annotation aynı mantığa dayanarak çalışır ancak farklı syntax kullanılır.
   Marker interface günümüz Java uygulamalarında pek tercih edilmezken, marker annotation daha sıklıkla kullanılır.
   Her ikisi de bir sınıfa ek bilgi eklemek için kullanılır ancak bu bilgiyi ekleme şekilleri farklıdır.

</details>

<details>

<summary>Javada int ve Integer arasındaki farklar nelerdir? Neden ikisine de ihtiyacımız vardır??</summary>

int ve Integer, Java'da tamsayı değerleri temsil etmek için kullanılan iki farklı veri tipidir. Aralarındaki temel farklar şunlardır:

1. Tür:
   int: İlkel bir veri tipidir.
   Integer: Bir sınıftır.
2. Değer Aralığı:
   int: 32 bitlik bir tamsayı değerini temsil eder. Bu, -2.147.483.648 ile 2.147.483.647 arasındaki değerleri kapsar.
   Integer: 32 bitlik bir tamsayı değerini temsil eder. Bu, -2.147.483.648 ile 2.147.483.647 arasındaki değerleri kapsar.
3. Null Değeri:
   int: Null değer alamaz.
   Integer: Null değer alabilir.
4. Bellek Kullanımı:
   int: Daha az bellek kullanır.
   Integer: Daha fazla bellek kullanır.
5. İşlemler:
   int: Temel matematiksel işlemler için doğrudan kullanılabilir.
   Integer: Temel matematiksel işlemler için Integer sınıfının metotlarını kullanmak gerekir.
   Neden ikisine de ihtiyacımız vardır?
   int: İlkel bir veri tipi olduğu için daha hızlı ve daha az bellek kullanır. Bu nedenle, basit tamsayı değerlerini saklamak ve işlemek için idealdir.
   Integer: Bir sınıf olduğu için null değer alabilir ve metotlar gibi ek özellikler sunar. Bu nedenle, daha karmaşık işlemler için ve null değerlerle çalışırken idealdir.
   Özetle:
   int: Hızlı ve basit tamsayı işlemleri için kullanılır.
   Integer: Karmaşık işlemler ve null değerlerle çalışmak için kullanılır.
   Ekstra Bilgi:
   Java'da byte, short, long gibi int'e benzer diğer ilkel veri tipleri de mevcuttur.
   Double, Float gibi Integer'a benzer diğer wrapper sınıfları da mevcuttur.

</details>

<details>

<summary>Javada StringBuilder clasına neden ihtiyaç duyarız??</summary>

1. Veri Katma İşlemleri:
   String sınıfı, metinsel verileri saklamak ve işlemek için kullanılır. Fakat String nesneleri immutable (değiştirilemez)dir. Bir String nesnesine veri eklemek veya değiştirmek isterseniz, yeni bir String nesnesi oluşturmanız gerekir. Bu işlem, özellikle büyük metinler için performans sorunlarına yol açabilir.
   StringBuilder sınıfı ise mutable (değiştirilebilir) bir yapıya sahiptir. Bu sayede, bir StringBuilder nesnesine veri ekleme ve değiştirme işlemleri çok daha hızlı ve verimli bir şekilde yapılabilir.
2. Performans:
   String nesneleri immutable olduğu için, her veri ekleme veya değiştirme işleminde yeni bir nesne oluşturulması gerekir. Bu işlem, bellek kullanımının artmasına ve performansın düşmesine neden olabilir.
   StringBuilder nesneleri mutable olduğu için, veri ekleme ve değiştirme işlemleri mevcut nesne üzerinde gerçekleştirilir. Bu sayede, bellek kullanımı ve performans artışı sağlanır.
3. Thread Güvenliği:
   String nesneleri immutable olduğu için thread-safe (çoklu iş parçacığı güvenli)dir. Birden fazla iş parçacığı aynı String nesnesine erişmeye çalışsa bile, veri tutarsızlığı oluşmaz.
   StringBuilder nesneleri mutable olduğu için thread-safe değildir. Birden fazla iş parçacığı aynı StringBuilder nesnesine erişmeye çalışırsa ve veri ekleme veya değiştirme işlemleri yaparsa, veri tutarsızlığı oluşabilir.
4. Kolay Kullanım:
   StringBuilder sınıfı, metinsel verileri işlemek için çeşitli metotlar sunar. Bu metotlar, veri ekleme, silme, değiştirme ve arama gibi işlemleri kolay ve hızlı bir şekilde yapmamızı sağlar.
   Özetle:
   StringBuilder sınıfı, metinsel verileri işlemek için daha performanslı, verimli ve kullanımı kolay bir çözüm sunar.
   Büyük metinlerle çalışırken, veri ekleme ve değiştirme işlemlerinin sık yapıldığı durumlarda StringBuilder sınıfını kullanmak önemlidir.
   StringBuilder sınıfının kullanımının bazı örnekleri:
   Bir metne metin eklemek
   Bir metinden metin silmek
   Bir metni değiştirmek
   Bir metinde arama yapmak
   Bir metni büyük harfe veya küçük harfe dönüştürmek
   Ekstra Bilgi:
   StringBuilder sınıfına benzer bir sınıf olan StringBuffer sınıfı da mevcuttur. StringBuffer sınıfı thread-safe'dir, ancak StringBuilder sınıfından daha yavaştır.
   Java 9'dan itibaren String sınıfına concat() metodu eklenmiştir. Bu metot, iki String nesnesini birleştirmek için kullanılabilir.
   Umarım bu bilgiler yardımcı olmuştur.

</details>

<details>

<summary>REST API Özellikleri Nelerdir?
?</summary>

REST mimarisi, 6 madde üzerine inşa edilmiştir.
Stateless: Stateless yapısı sayesinde geçmişe yönelik bir tarama yapmanız gerekmez ve her reguest arasında bir kayıt tutmak zorunluluğu yoktur.
Uniform Interface: Bu kısıt, clientve server arasındaki iletişim için belirlenmiş prensiplerle sağlanır.
Cacheable: Client, gönderilen bilgilere göre bir cache mekanizması oluşturabilir.
Client-Server: Bu kısıta göre client, server’ın sorumluluğundaki depolama işlemleri vb. şeylerle ilgilenmez.
Layered System: Client-server mimarisi her zaman client’in direkt bir server’a istek göndermesi ve ondan cevap alması şeklinde değildir. Bu aşamada aralarda güvenlik katmanı, cache katmanı gibi katmanlar olabilir.
Code on Demand: Code on demand kısıt, server’ın client’a belli durumlarda executable script’ler ve applet’ler gönderebilmesini kapsar.

</details>

<details>

<summary>Agregatör?</summary>

Agregatör, birden fazla servisin verilerini toplayıp birleştiren bir servistir. Bu, birden fazla servisin verisini tek bir yere toplamak ve üzerinde işlem yapmak gerektiğinde kullanılır.

</details>

<details>

<summary>Proxy?</summary>

Proxy, bir servisin yerine geçen bir aracıdır. Proxy, istekleri gerçek servise yönlendirir ve servisin davranışını değiştirebilir. Örneğin, bir authorization proxy'si, istekleri yetkilendirebilir veya bir caching proxy, sıkça erişilen verileri önbellekte tutabilir.

</details>

<details>

<summary>Pipeline?</summary>

Pipeline, birden fazla servisin seri olarak çalıştırıldığı bir tasarımdır. Her servis, bir sonraki servis için veri üretir. Bu yaklaşım, bir dizi adım gerektiren işlemleri gerçekleştirmek için idealdir.

</details>

<details>

<summary>shared resources?</summary>

Paylaşılan kaynaklar, birden fazla servis tarafından kullanılan veriler veya diğer kaynaklardır. Bu kaynaklar, servislerin birbirleriyle koordineli bir şekilde çalışmasını sağlar. Paylaşılan kaynakların yönetimi ve güvenliği dikkatle ele alınmalıdır.

</details>

<details>

<summary>Asenkron Mesajlaşma?</summary>

Asenkron mesajlaşma, servisler arasında iletişim kurmak için kullanılan bir yöntemdir. Bu yöntemde, bir servis bir mesaj gönderir ve daha sonra bir yanıt bekler yerine, mesajı bir kuyruğa gönderir ve devam eder. Bu, servislerin birbirini beklemeden çalışmasına ve performansı artırmaya yardımcı olur.

</details>

<details>

<summary>Serializing Nedir?
?</summary>

Serializing, bir nesnenin veya veri yapısının, depolanabilecek veya ağ üzerinden aktarılabilecek ve daha sonra geri yüklenebilecek bir formata dönüştürülmesi işlemidir. Bu işlem, nesnenin durumunu (değişkenlerinin değerleri) bir dizi byte'a dönüştürerek gerçekleştirilir.
Serializing'in Avantajları:
Veri saklama: Nesneleri dosyalarda veya veritabanlarında saklamak için kullanılabilir.
Ağ iletişimi: Nesneleri ağ üzerinden bir sistemden diğerine aktarmak için kullanılabilir.
Bellek kopyalama: Nesnelerin bellekteki kopyalarını oluşturmak için kullanılabilir.
Nesnelerin kopyalanması: Nesnelerin kopyalarını oluşturmak için kullanılabilir.
Serializing Çeşitleri:
Java Serialization: Java'da nesneleri serileştirmek için kullanılan standart bir mekanizmadır.
XML Serialization: Nesneleri XML formatına dönüştürmek için kullanılır.
JSON Serialization: Nesneleri JSON formatına dönüştürmek için kullanılır.
Serializing İşlemi:
Serializing işlemi iki aşamadan oluşur:
Yazma: Nesnenin durumu byte'lara dönüştürülür ve bir çıktı akışına yazılır.
Okuma: Byte'lar bir giriş akışından okunur ve nesnenin durumu geri yüklenir.
Serializing ile Dikkat Edilmesi Gerekenler:
Güvenlik: Serialized nesneler, güvenli olmayan bir şekilde depolanırsa veya aktarılırsa güvenlik riskleri oluşturabilir.
Performans: Serializing işlemi, büyük ve karmaşık nesneler için zaman alıcı olabilir.
Uyumluluk: Serialized nesneler, farklı platformlarda veya farklı Java sürümlerinde geri yüklenebilmeleri için uyumlu bir şekilde serileştirilmelidir.
Serializing, nesneleri saklamak, aktarmak ve kopyalamak için kullanılabilecek güçlü bir araçtır. Serializing'in avantajlarından ve dezavantajlarından haberdar olmak ve onu doğru şekilde kullanmak önemlidir.

</details>

<details>

<summary>Volatile Nedir?
?</summary>

Volatile, bir değişkenin değerinin programın akışı dışında değişebileceğini gösteren bir anahtar kelimedir. Bu, genellikle birden fazla iş parçacığı veya donanım kesmesi tarafından erişilen değişkenler için kullanılır.
Volatile'in Özellikleri:
Değişkenin belleğe her erişiminde güncel değer okunur.
Değişkenin belleğe her yazılmasında güncel değer yazılır.
Farklı iş parçacıkları tarafından yapılan değişiklikler anında görünür hale gelir.
Volatile'in Kullanım Alanları:
Çoklu iş parçacığı programlama: Birden fazla iş parçacığı tarafından paylaşılan değişkenleri korumak için kullanılır.
Donanım kesmeleri: Donanım kesmeleri tarafından erişilen değişkenleri korumak için kullanılır.
Bellek sırası: Bellek sırası ile ilgili problemleri önlemek için kullanılır.
Volatile'in Avantajları:
Veri tutarlılığını sağlar.
İş parçacıkları arasında veri yarışını önler.
Donanım kesmeleri ile ilgili problemleri önler.
Volatile'in Dezavantajları:
Performansı düşürebilir.
Kod karmaşıklığını artırabilir.
Volatile'in Örnek Kullanımı:

```java
public class VolatileExample {

    private volatile int counter = 0;

    public void incrementCounter() {
        counter++;
    }

    public int getCounter() {
        return counter;
    }

}
```

Bu örnekte, counter değişkeni volatile olarak tanımlanmıştır. Bu, birden fazla iş parçacığı tarafından erişilmesine izin vererek, her iş parçacığının her zaman counter'ın güncel değerini görmesini sağlar.
Volatile, çoklu iş parçacığı programlamada ve donanım kesmeleri ile çalışırken önemli bir kavramdır. Doğru şekilde kullanıldığında, veri tutarlılığını sağlayabilir ve iş parçacıkları arasında veri yarışını önleyebilir.

</details>

<details>

<summary>Java’da Delegate Nedir?
?</summary>

Delegate, bir nesnenin bir görevi veya sorumluluğu başka bir nesneye devretmesine olanak tanıyan bir tasarım desenidir. Bu, kodun yeniden kullanılabilirliğini ve modülerliğini artırabilir ve karmaşıklığı azaltabilir.
Delegate'in temel prensibi:
Görev arayüzü: Delegate, devredilecek görevi tanımlayan bir arayüzdür.
Gönderen nesne: Gönderen nesne, görevi devretmek isteyen nesnedir.
Alıcı nesne: Alıcı nesne, görevi devralan nesnedir.
Görev devri: Gönderen nesne, delegate arayüzü aracılığıyla alıcı nesneye bir referans verir.
Görev yürütme: Alıcı nesne, delegate arayüzündeki yöntemi implement ederek görevi yürütür.
Java'da delegate'i uygulamak için:
Görev arayüzü: Bir interface oluşturarak devredilecek görevi tanımlayın.
Gönderen nesne: Delegate arayüzü tipinde bir field veya variable tanımlayın.
Alıcı nesne: Görev arayüzünü implement edin.
Görev devri: Gönderen nesne, alıcı nesnenin referansını delegate field veya variable'a atayın.
Görev yürütme: Gönderen nesne, delegate arayüzündeki yöntemi çağırarak alıcı nesneden görevi yürütmesini ister.
Delegate'in faydaları:
Kodun yeniden kullanılabilirliği: Bir görevi birden fazla nesneye devredebilirsiniz.
Modülerlik: Kodunuzu daha küçük ve daha yönetilebilir parçalara ayırabilirsiniz.
Karmaşıklık azaltma: Kodunuzun daha okunabilir ve anlaşılır olmasını sağlayabilirsiniz.
Delegate'in dezavantajları:
Bağımlılıklar: Gönderen ve alıcı nesneler arasında bir bağımlılık oluşturur.
Performans: Delegate kullanımı, performans üzerinde bir ek yük oluşturabilir.
Delegate'i kullanmanın uygun olduğu durumlar:
Bir görevi birden fazla nesneye devretmek istediğinizde.
Kodunuzu daha modüler ve yeniden kullanılabilir hale getirmek istediğinizde.
Karmaşıklığı azaltmak ve kodun okunabilirliğini artırmak istediğinizde.
Java'da delegate'i kullanmak için bazı örnekler:
Event handling: Bir nesnenin bir olayı başka bir nesneye bildirmesi için.
Callback: Bir işlem tamamlandıktan sonra başka bir nesneyi bilgilendirmek için.
Logging: Bir nesnenin log mesajlarını başka bir nesneye göndermesi için.

</details>

<details>

<summary>Event-Driven Nedir?
?</summary>

Event-driven, olay odaklı bir programlama ve mimari paradigmasıdır. Bu paradigma, programın akışının olaylar tarafından yönlendirildiği fikrine dayanır. Olaylar, sistemde meydana gelen önemli anlar veya değişikliklerdir. Örneğin, bir kullanıcının bir düğmeye tıklaması veya bir veri kaynağında bir değişiklik olması bir olay olabilir.
Event-Driven'ın Özellikleri:
Olaylar programın akışını yönlendirir.
Olaylar, sistemdeki değişiklikleri temsil eder.
Olaylar, birden fazla bileşeni etkileyebilir.
Olaylar asenkron olarak işlenebilir.
Event-Driven'ın Kullanım Alanları:
Kullanıcı Arabirimi Programlama (GUI): Kullanıcı arabirimi olaylarına (örneğin, bir düğmeye tıklama) yanıt vermek için kullanılabilir.
Gerçek Zamanlı Sistemler: Gerçek zamanlı olaylara (örneğin, bir sensörden gelen veri) yanıt vermek için kullanılabilir.
Dağıtılmış Sistemler: Farklı sistemler arasında iletişim kurmak için kullanılabilir.
Event-Driven'ın Avantajları:
Esneklik: Olaylara kolayca yeni tepkiler eklenebilir veya mevcut tepkiler değiştirilebilir.
Ölçeklenebilirlik: Olaylar asenkron olarak işlenebildiği için sistem kolayca ölçeklendirilebilir.
Bakımı Kolay: Olay odaklı kod, modüler ve bakımı kolay olma eğilimindedir.
Event-Driven'ın Dezavantajları:
Karmaşıklık: Olay odaklı sistemler, geleneksel sistemlere kıyasla daha karmaşık olabilir.
Hata Ayıklama: Olay odaklı sistemlerde hataları bulmak ve düzeltmek zor olabilir.
Event-Driven, birçok farklı programlama dilinde ve platformda uygulanabilen güçlü bir paradigmadır.
Event-Driven'ın Örnek Kullanımı:
Python
def on_button_click(event):
print("Düğmeye tıklandı!")

# Bir düğmeye tıklandığında on_button_click fonksiyonu çağrılacak

button.on_click(on_button_click)

Bu örnekte, bir düğmeye tıklandığında on_button_click fonksiyonunun çağrılmasını sağlayan bir event-driven programın basit bir örneği gösterilmiştir.
Event-Driven, programların daha esnek, ölçeklenebilir ve bakımı kolay olmasını sağlayabilecek güçlü bir paradigmadır.

</details>

<details>

<summary>Race Condition
?</summary>

Race condition, birden fazla iş parçacığının veya thread'in paylaşılan bir kaynağa aynı anda erişmeye çalıştığı ve bu işlemlerin sırasına bağlı olarak beklenmeyen sonuçlar ortaya çıkabileceği bir yazılım hata durumudur.
Nasıl Çalışır:
Paylaşılan Kaynak: Örneğin, bir sayaç gibi programın devamı için kritik değere sahip bir değişken.
Çoklu Erişim: Aynı anda birden fazla iş parçacığı bu kaynağa erişmeye çalışır.
Sıra Bağımlılığı: Hangi iş parçacığının önce okuyup yazacağından emin olunmaz.
Beklenmeyen Sonuç: İşlem sırasına göre doğru değer değişebilir veya kaybolabilir.
Örnek:
Java
int counter = 0;

public void incrementCounter() {
counter++;
}

public int getCounter() {
return counter;
}

// Ana Thread
// ... Diğer işlemler
for (int i = 0; i < 1000; i) {
new Thread(this::incrementCounter).start();
}

// ... Diğer işlemler
// Beklenen Değer: 1000
System.out.println("Sayaç Değeri: " + getCounter());

Bu kodda, bir sayaç değeri her iş parçacığında artırılır. Fakat hangi iş parçacığının önce başlayacağı bilinmediğinden, sayaç değeri beklenen 1000 yerine daha düşük bir değer alabilir.
Sonuçlar:
Yanlış veriler
Program çökmesi
Beklenmeyen davranışlar
Veri tutarsızlığı
Önleme Yöntemleri:
Senkronizasyon: Lock, Mutex gibi mekanizmalar ile paylaşılan kaynağa aynı anda sadece bir iş parçacığı erişebilir.
Atomik İşlemler: İşlemi bölünemeyecek bir birim olarak ele alarak aynı anda başka bir iş parçacığı müdahale edemez.
Thread-Safe Veri Yapıları: Paylaşılan verileri iş parçacığı güvenli hale getirilmiş veri yapıları ile kullanmak.

</details>

<details>

<summary>Encoding Nedir?
?</summary>

Encoding, bir karakter kümesinin veya metnin, bilgisayarlar tarafından işlenebilecek bir formata dönüştürülmesi işlemidir. Bu işlemde, her karaktere bir sayı veya bit dizisi atanır. Encoding işlemi, farklı karakter kümeleri ve diller arasında veri alışverişi yapmayı ve farklı sistemlerde metni doğru şekilde görüntülemenizi sağlar.
Encoding Türleri:
ASCII: 7 bitlik bir kodlama sistemidir. İngilizce alfabesi, sayılar ve bazı özel karakterleri kapsar.
Unicode: 16 bitlik bir kodlama sistemidir. ASCII'de yer alan karakterlerin yanı sıra, birçok farklı dil ve alfabedeki karakterleri de kapsar.
UTF-8: Unicode karakter kümesini 8 bitlik byte'lara dönüştüren bir kodlama sistemidir. En yaygın kullanılan encoding türlerinden biridir.
Encoding Seçimi:
Encoding seçimi, kullanacağınız metnin içeriğine ve hangi sistemlerde kullanılacağına bağlıdır. Örneğin, Türkçe metinler için UTF-8 kodlama sistemi tercih edilir.
Encoding Problemleri:
Farklı encoding sistemleri kullanıldığında, metinlerde istenmeyen değişiklikler oluşabilir. Örneğin, bir metin ASCII kodlama ile kaydedilip UTF-8 kodlama ile açılırsa, Türkçe karakterler hatalı görünebilir.
Encoding Örnekleri:
Bir metin dosyasını UTF-8 kodlama ile kaydetmek.
Bir web sayfasının kodlama sistemini belirlemek.
Veritabanında bir metin sütununu belirli bir kodlama sistemi ile saklamak.
Encoding, metinlerle çalışırken önemli bir kavramdır. Doğru encoding seçimi ve kullanımı, metinlerin doğru şekilde işlenmesini ve görüntülenmesini sağlar.

</details>

<details>

<summary>Code Coverage
?</summary>

Code coverage, yazılım geliştirmede yazılan kodun ne kadarının testlerle kapsanıp çalıştırıldığına dair bir ölçüdür. Daha basitçe, kodunuzun ne kadarının test senaryoları ile çalıştırılıp kontrol edildiğini gösterir.
Ne İşe Yarar:
Testlerin kapsamlılığını ölçmek: Yüksek code coverage oranı, kodun daha fazla test ile kapsanıp hataları tespit etme ihtimalini artırır.
Hata yakalama olasılığını artırmak: Daha fazla kod test edildiği için hataların bulunma ve düzeltilme olasılığı yükselir.
Kod kalitesini değerlendirmek: Yüksek code coverage, kodun daha iyi yazıldığına dair bir gösterge olabilir.
Sürekli Entegrasyon (CI) ve Sürekli Dağıtım (CD) süreçlerinde kullanmak: CI/CD süreçlerinde belirli bir code coverage oranının sağlanması gerekli olabilir.
Nasıl Hesaplanır:
Code coverage, genellikle satır bazında hesaplanır. Yani, kodunuzdaki satırların kaçınının testler tarafından çalıştırıldığına bakılır. Diğer hesaplama yöntemleri de mevcuttur, örneğin:
Dal (Branch) coverage: Dallanma noktalarının ne kadar kapsandığına bakar.
Fonksiyon coverage: Fonksiyonların ne kadarının test edildiğine bakar.
Hangi Oran İyi Sayılır:
Yüksek code coverage oranı her zaman iyi değildir. Çok yüksek oranlar aşırı test yazılmasına ve gereksiz zaman harcanmasına neden olabilir. Genel olarak %80-90 civarı bir oran ideal kabul edilir, ancak bu oran proje türüne ve risk seviyesine göre değişebilir.
Ne Zaman Önemlidir:
Kritik ve güvenlik açısından önemli yazılımlar
Karmaşık algoritmalar içeren kodlar
Hata oranının düşük olması gereken sistemler
Unutmayın:
Code coverage tek başına bir kalite ölçütü değildir. İyi yazılım için test kapsamlılığının yanı sıra kodun temizliği, okunabilirliği, performansı gibi faktörler de önemlidir.
Testler, code coverage'ı artırsa da her zaman doğru ve etkili olmayabilir. Kaliteli test yazmak önemlidir.

</details>

<details>

<summary>Warning Threshold
?</summary>

Warning Threshold, farklı bağlamlarda kullanılabilen, ancak temel olarak bir uyarı eşiğini ifade eden bir terimdir.
Warning Threshold, bir sistemin normal çalışma durumunu tanımlayan sınır değerlerdir. Bu sınırlar aşıldığında, potansiyel bir sorun olduğunu anlamak için bir uyarı verilir.
Warning Threshold'un hangi seviyede olması gerektiği, sistemin amacına, risk tolere edilebilirliğine ve alınacak aksiyonlara göre değişir.
Efektif uyarı eşiği belirlemek, sorun tespitini hızlandırır, gereksiz uyarıları azaltır ve istenmeyen durumlara önlem alınmasını sağlar.

</details>

<details>

<summary>Monitoring
?</summary>

Monitoring, bir sistemin veya uygulamanın performansını, işlevselliğini ve güvenliğini izleme ve analiz etme işlemidir. Bu işlem, çeşitli araçlar ve teknikler kullanılarak gerçekleştirilir ve aşağıdakileri kapsar:
Veri Toplama: Sistemin çeşitli kaynaklarından (örneğin, CPU, bellek, disk, ağ) performans ve durum verileri toplanır.
Veri Analizi: Toplanan veriler, anormallikleri, trendleri ve potansiyel sorunları belirlemek için analiz edilir.
Uyarı ve Bildirim: Belirli sınırlar aşıldığında veya belirli olaylar gerçekleştiğinde, otomatik uyarılar ve bildirimler gönderilir.
Görselleştirme: Veriler, trendleri ve sorunları görsel olarak göstermek için grafikler, gösterge tabloları ve diğer görselleştirme teknikleri kullanılır.
Teşhis ve Sorun Giderme: Sorunlar belirlendikten sonra, temel nedenleri teşhis edilir ve çözümler bulunur.
Raporlama: Performans ve durum hakkında düzenli raporlar oluşturulur ve ilgili paydaşlara sunulur.
Monitoring'in Faydaları:
Sistem ve uygulama performansını optimize eder.
Sorunları önceden tespit ederek önlem almanızı sağlar.
Güvenlik açıklarını ve riskleri belirler.
Verilerin kullanılabilirliğini ve bütünlüğünü sağlar.
Uyumluluk gereksinimlerini karşılamanıza yardımcı olur.
Maliyetleri düşürür ve üretkenliği artırır.
Monitoring Türleri:
Sistem Monitoring: İşletim sistemi, ağ, donanım ve diğer sistem bileşenlerinin performansını izler.
Uygulama Monitoring: Yazılım uygulamalarının performansını ve işlevselliğini izler.
Ağ Monitoring: Ağ trafiğini, cihazları ve performansı izler.
Güvenlik Monitoring: Güvenlik açıklarını, saldırıları ve izinsiz girişleri izler.
Performans Monitoring: Sistemin genel performansını ve darboğazları izler.
Monitoring Araçları:
Nagios: Açık kaynaklı bir sistem ve ağ izleme aracıdır.
Zabbix: Kapsamlı bir izleme çözümü sunan, açık kaynaklı bir platformdur.
SolarWinds Orion: Ağ, sistem ve uygulama izleme için ticari bir çözümdür.
Microsoft System Center Operations Manager: Microsoft tarafından geliştirilen bir sistem ve uygulama izleme platformudur.

</details>

<details>

<summary>Custom Telemetry/Metrik
?</summary>

Özel telemetri/metrik, belirli bir sistemin veya uygulamanın işlevselliği ve performansı hakkında bilgi edinmek için toplanan özel verilerdir. Bu veriler, standart telemetri/metrik araçları tarafından toplanan verilerden ayrıdır ve genellikle daha ayrıntılı ve özel bilgiler içerir.
Özel Telemetri/Metrik Kullanmanın Avantajları:
Daha ayrıntılı bilgi: Standart telemetri/metrik araçları, genel bir bakış sunarken, özel telemetri/metrik belirli bir sistemin veya uygulamanın belirli yönleri hakkında daha ayrıntılı bilgi sağlayabilir.
Sorunları daha hızlı tespit etme: Özel telemetri/metrik, standart telemetri/metrik araçları tarafından tespit edilemeyen sorunları daha hızlı tespit etmeye yardımcı olabilir.
Performansı optimize etme: Özel telemetri/metrik, sistemin veya uygulamanın performansını optimize etmek için kullanılabilir.
Güvenliği iyileştirme: Özel telemetri/metrik, sistemin veya uygulamanın güvenliğini iyileştirmek için kullanılabilir.
Özel Telemetri/Metrik Toplama Yöntemleri:
Kodlama: Özel telemetri/metrik verilerini toplamak için uygulama koduna özel kod ekleyebilirsiniz.
Araçlar: Özel telemetri/metrik verilerini toplamak için üçüncü taraf araçlar kullanabilirsiniz.
API'ler: Özel telemetri/metrik verilerini toplamak için sistemin veya uygulamanın API'lerini kullanabilirsiniz.
Özel Telemetri/Metrik Verilerini Kullanma:
Veri analizi: Özel telemetri/metrik verilerini analiz ederek trendleri, modelleri ve anormallikleri belirleyebilirsiniz.
Görselleştirme: Özel telemetri/metrik verilerini görselleştirerek verilerden daha kolay anlamlı bilgiler elde edebilirsiniz.
Uyarılar: Belirli sınırlar aşıldığında veya belirli olaylar gerçekleştiğinde otomatik uyarılar oluşturabilirsiniz.
Özel Telemetri/Metrik, sistemler ve uygulamalar hakkında daha ayrıntılı bilgi edinmek ve performansı ve güvenliği optimize etmek için güçlü bir araçtır.
Özel Telemetri/Metrik Örnekleri:
Bir web uygulamasının API'sine yapılan isteklerin sayısı ve süresi
Bir mobil uygulamanın kullandığı bellek ve CPU miktarı
Bir veritabanındaki sorguların yürütme süresi
Bir ağdaki paket kaybı ve gecikme süresi
Özel Telemetri/Metrik, her bir sistemin veya uygulamanın özel gereksinimlerine göre özelleştirilebilir.

</details>

<details>

<summary>Blog Storage
?</summary>

"Blog storage" terimi aslında net bir şekilde tanımlanmış bir teknoloji veya konsept değildir. Ancak web sitelerinde ve blog yazarlığı ile ilgili olarak iki farklı şekilde yorumlanabilir:

1. Blog platformlarının depolama seçenekleri:
   Burada "blog storage" blog platformlarının sunduğu depolama çözümlerini ifade eder. Örneğin, WordPress.com, Blogger gibi ücretsiz platformlar sınırlı bir depolama alanı sunarlar. Blog yazarları daha fazla depolama ihtiyacı olduğunda ise ücretli planlara geçebilirler. Diğer yandan Wix, Squarespace gibi platformlar ödenen planlarla birlikte çeşitli depolama kapasiteleri sunarlar. Bunlara ek olarak, kendi web sunucunuzu kullanarak bir blog kurduğunuzda depolama için sunucu sağlayıcının sunacağı disk alanından faydalanırsınız.
2. Blog içeriğinin depolandığı yerler:
   Bu yorumda ise "blog storage" blog içeriklerinin (metin, resimler, videolar) fiziksel olarak saklandığı yerlere işaret eder. Bu da yine birkaç olasılığı barındırır:
   Merkezi sunucular: Çoğu blog platformu içeriği kendi sunucularında depolar. Bu sunucular genellikle güvenli ve bakımı yapılmış verimerkezlerinde bulunur.
   CDN (Content Delivery Network): Bazı platformlar veya blog yazarları içeriği daha hızlı yüklemek için CDN hizmetlerinden yararlanır. CDN, dünyanın farklı yerlerinde bulunan sunucularda web sitesi içeriğini önbelleğe alır. Böylece ziyaretçi içeriğe en yakın sunucudan erişerek daha hızlı yükleme elde eder.
   Yerel depolama: Eğer WordPress gibi kendi kod tabanınızı barındıran bir platform kullanıyorsanız, blog içeriği web sunucunuzun disk alanında depolanır.
   "Blog storage" hakkında ek bilgilendirme isterseniz, şu konuları belirterek sorunuzu detaylandırabilirsiniz:
   Hangi bağlamda "blog storage" terimini duyduğunuz?
   Siz ne tür bir bilgi arıyorsunuz?
   Umarım bu açıklamalar size yardımcı olur.

</details>

<details>

<summary>Reverse Proxy ve Forward Proxy
?</summary>

Hem Forward Proxy hem de Reverse Proxy, ağ trafiğini yönlendirmek için kullanılan aracı sunuculardır. Ancak aralarında önemli farklılıklar mevcuttur:
Forward Proxy:
Konum: İstemci ve internet arasında bulunur.
Hedef: İstemcinin internet erişimini kontrol etmek, filtrelemek veya anonimleştirmek için kullanılır.
Kullanım Örnekleri:
İşyeri ağlarında internet erişimini kısıtlamak için
Kamu Wi-Fi'de anonim kalmak için
Coğrafi kısıtlamaları aşmak için
Reverse Proxy:
Konum: İnternet ve sunucu (web sunucusu, uygulamalar vb.) arasında bulunur.
Hedef: Sunucuları korumak, yük dengelemek, performansı artırmak ve güvenliği geliştirmek için kullanılır.
Kullanım Örnekleri:
Web sunucularını DDoS saldırılarından korumak için
Birden fazla sunucuya gelen trafiği dağıtmak için
SSL/TLS sertifikalarını merkezi olarak yönetmek için
Forward Proxy ile Reverse Proxy arasındaki farklar:

<figure><img src="assets/tables/unnamed (19).png" alt=""><figcaption></figcaption></figure>

Ek Bilgi:
Her iki proxy türü de güvenlik riskleri oluşturabilir. Forward Proxy kullanırken gizliliğinizin korunduğundan emin olmak önemlidir. Reverse Proxy, web sunucularınızı ve uygulamalarınızı daha güvenli hale getirmeye yardımcı olabilir, ancak doğru yapılandırılmadığında güvenlik açıkları oluşturabilir.
CDN (Content Delivery Network) hizmetleri genellikle Reverse Proxy teknolojisini kullanır.

</details>

<details>

<summary>Data Consistency Nedir?
?</summary>

Data consistency (veri tutarlılığı), bir sistemdeki verilerin birbiriyle ve kurallarla tutarlı olma durumunu ifade eder. Başka bir deyişle, aynı bilgi farklı yerlerde tutulduğunda hepsinin aynı ve doğru olması anlamına gelir.
Tutarlı olmayan veriler, bilgi analizindeki hatalara, karar yanlışlarına ve güvenlik sorunlarına yol açabileceğinden son derece önemlidir.
Data Consistency Çeşitleri
Veri tutarlılığı birkaç farklı seviyede düşünülebilir:
Satır Bazlı Tutarlılık: Aynı tablodaki farklı satırlarda aynı verilere atıfta bulunulurken tutarlılık. Örneğin, bir müşterinin adı tüm kayıtlarında aynı olmalıdır.
Sütun Bazlı Tutarlılık: Aynı tablodaki farklı sütunlar arasındaki ilişkilerde tutarlılık. Örneğin, bir siparişin tutarı, ürünlerin fiyatlarının toplamına eşit olmalıdır.
Uygulama Tutarlılığı: Farklı uygulamalar arasında aynı bilgi tutarlı bir şekilde temsil edilir. Örneğin, bir müşteri bilgisi web sitesinde ve satış sisteminde aynı olmalıdır.
Veritabanı Tutarlılığı: Farklı veritabanları arasında tutarlılık, özellikle dağıtılmış sistemlerde önemlidir.
Data Consistency Neden Önemlidir?
Doğru Kararlar: Doğru ve tutarlı verilere sahip olmak, daha iyi bilgi analizi, raporlama ve dolayısıyla daha doğru kararlar alınmasını sağlar.
Güvenilir Operasyonlar: Tutarlı veri, sistem hatalarını azaltır ve iş süreçlerinin sorunsuz çalışmasını sağlar.
Veri Güvenliği: Tutarlılık, verilerin manipüle edilmesini veya yanlış yorumlanmasını zorlaştırır, güvenliği arttırır.
Yasal Uyum: Bazı endüstrilerde veri tutarlılığı, yasalara ve düzenlemelere uymak için gereklidir.
Data Consistency Nasıl Sağlanır?
Veri tutarlılığı sağlamak için çeşitli yöntemler kullanılabilir:
Veri Doğrulama: Verinin girişi sırasında kontroller uygulanarak doğruluğunun sağlanması.
Veri Temizleme: Var olan verilerdeki tutarsızlıkları düzeltmek için işlemler yapılması.
Veri İlişkileri: Farklı veriler arasındaki ilişkileri tanımlayan kuralların yazılması.
Veri İşlemleri: Veri değişikliklerini bir bütün olarak işleyen mekanizmalar kullanılması (örneğin, transactionlar).
Veri Yönetim Araçları: Veri tutarlılığını izleyen ve enforse eden yazılımlar kullanaılması.
Data consistency farklı sistemler ve uygulamalarda karmaşık olabileceğinden, sürekli takip ve iyileştirme gerektirir. Veri mimarisi, güvenlik ilkeleri ve iş kurallarıyla uyumlu bir yaklaşım izlenmelidir.

</details>

<details>

<summary>system/process documentation
?</summary>

Sistem/süreç dokümantasyonu, bir sistemin veya sürecin nasıl çalıştığını, bileşenlerini ve işlevlerini ayrıntılı olarak açıklayan yazılı bir materyaldır. Bu dokümantasyon, sistemin geliştirilmesi, anlaşılması, işletilmesi ve bakımı için kritik önem taşır.
Sistem/süreç dokümantasyonu şunları içerebilir:
Sistem/süreç tanımı: Sistemin/sürecin ne yaptığı, ne amaçla kullanıldığı ve hangi işlevleri yerine getirdiği açıklanır.
Bileşenler: Sistemin/sürecin ana bileşenleri, bunların rolleri ve aralarındaki ilişkiler tanımlanır.
İş akışları: Sistem/süreç adım adım nasıl çalışır, hangi aşamalardan ve karar noktalarından oluşur açıklanır.
Veriler: Sistem/süreç hangi verileri kullanır, bu verilerin nasıl işlendiği ve depolandığı belirtilir.
Prosedürler: Sistemin/sürecin kullanımı için adım adım prosedürler ve talimatlar sunulur.
Hatalar ve sorun giderme: Sistemle ilgili olası hatalar ve bunların çözümleri açıklanır.
Bakım ve güncelleme: Sistemin bakımı ve güncellenmesi için gerekli işlemler tanımlanır.
Sistem/süreç dokümantasyonunun faydaları şunlardır:
Daha iyi anlaşılma: Sistemin/sürecin nasıl çalıştığını anlamak için net bir referans noktası sağlar.
Eğitim amaçlı: Yeni personelin eğitiminde ve mevcut personelin bilgi tazelemesinde kullanılır.
Sorun giderme: Sorunları teşhis etmeyi ve çözmeyi kolaylaştırır.
Sürekli iyileştirme: Sistemi/süreçi iyileştirmek için fikirlerin ortaya atılmasını ve uygulanmasını sağlar.
Yasal uyumluluk: Bazı sektörlerde yasalara ve düzenlemelere uymak için dokümantasyon gereklidir.
Risk yönetimi: Sistemdeki potansiyel risklerin belirlenmesine ve azaltılmasına yardımcı olur.
Sistem/süreç dokümantasyonu farklı şekillerde oluşturulabilir:
Yazılı belgeler: Geleneksel ve en yaygın yöntemdir. Metin, çizelge ve diyagramlar kullanılarak oluşturulur.
Video kayıtları: Karmaşık süreçleri görsel olarak göstermek için kullanılabilir.
Web tabanlı dokümantasyon: Erişim kolaylığı ve güncel tutulabilirlik sağlar.
İş akışı yönetimi yazılımları: Süreçleri modellemek ve dokümantasyon oluşturmak için özel yazılımlar kullanılabilir.
Sistem/süreç dokümantasyonu oluştururken önemli hususlar şunlardır:
Hedef kitleyi belirleyin: Dokümantasyonu kimin okuyacağı ve ne tür bilgiye ihtiyaç duyacaklarını anlayın.
Açık ve özlü dil kullanın: Teknik jargonu minimumda tutun ve herkesin anlayabileceği şekilde yazın.
Güncel tutun: Sistem/süreç değiştikçe dokümantasyonu güncelleyin.
Erişilebilir olun: Dokümantasyona kolayca erişilebilir olduğundan emin olun.
Sonuç olarak, sistem/süreç dokümantasyonu, sistemlerin ve süreçlerin verimli ve etkili bir şekilde çalışmasını sağlayan önemli bir araçtır. İyi hazırlanmış dokümantasyon, sistemin anlaşılmasını, kullanımını, bakımını ve iyileştirilmesini kolaylaştırır.

</details>

<details>

<summary>Typecasting Nedir?
?</summary>

Typecasting, bir veri tipini başka bir veri tipine dönüştürme işlemidir. Java'da iki tür typecasting vardır:

1. Implicit Typecasting (Otomatik Dönüştürme)
   Java, bazı durumlarda veri tiplerini otomatik olarak dönüştürür. Örneğin, bir byte veri tipindeki değer bir int veri tipine atanabilir. Bu işlem veri kaybına neden olmaz.
   Örnek:
   Java
   byte b = 10;
   int i = b; // Otomatik dönüştürme

2. Explicit Typecasting (Açık Dönüştürme)
   Bazı durumlarda, veri tipini açıkça dönüştürmeniz gerekir. Bunu, dönüştürmek istediğiniz veri tipinin adını parantez içinde yazarak yapabilirsiniz. Explicit typecasting veri kaybına neden olabilir.
   Örnek:
   Java
   int i = 10;
   byte b = (byte) i; // Açık dönüştürme

// Bu kod veri kaybına neden olabilir

Typecasting'in Kullanım Alanları:
Farklı veri tiplerindeki değerleri karşılaştırmak için.
Farklı veri tiplerindeki değerleri işlemek için.
Farklı veri tiplerindeki değerleri bir araya getirmek için.
Typecasting Kullanırken Dikkat Edilmesi Gerekenler:
Explicit typecasting kullanırken veri kaybına neden olabileceğini unutmayın.
Dönüştürmek istediğiniz veri tipinin aralığını kontrol edin.
Typecasting'i gereksiz yere kullanmaktan kaçının.
Java'da sonsuz döngü (infinite loop) nedir?
Java’da sonsuz döngü (infinite loop), bir döngü veya koşulun sürekli olarak doğru kalması nedeniyle döngünün hiçbir zaman sonlanmaması durumudur. Yani döngü, sürekli olarak tekrar eder.

</details>

<details>

<summary>Java String Pool (Dize Havuzu) nedir?
?</summary>

Java String Havuzu (String Pool) Nedir?
Java String havuzu, Java Heap belleğinde saklanan bir alandır. Flyweight Tasarım Şablonu örneğidir. String immutable (değişmez) olduğu için ve String intern kavramı uygulanabildiği için Java'da String Pool mümkündür.
String Havuzu Nasıl Çalışır?
Yeni bir String nesnesi oluşturulduğunda, String havuzu önce nesnenin havuzda olup olmadığını kontrol eder.
String havuzda varsa, aynı referans değişkene döndürülür.
String havuzda yoksa, nesne havuza eklenir ve referans değişkeni döndürülür.
String Havuzunun Faydaları:
Hafıza tasarrufu sağlar: Aynı String nesnesinin birden fazla kopyası oluşturulmaz.
Performansı artırır: String nesnelerine erişim daha hızlı hale gelir.
Kodun okunabilirliğini artırır: Aynı String nesnesinin birden fazla kopyası ile uğraşmaya gerek kalmaz.
String Havuzunu Kullanmak:
String nesnelerini new String ile oluşturmak yerine, String.intern() metodu kullanılabilir.
String.intern() metodu, String nesnesini String havuzda arar ve varsa aynı referans değişkenini döndürür.
String Havuzunun Dezavantajları:
String nesneleri değiştirilemez.
String havuzunun boyutu sınırlıdır.
String Havuzuna İlişkin Örnekler:
Java
String str1 = "Merhaba";
String str2 = "Merhaba";

// str1 ve str2 aynı String nesnesine referans verir.
System.out.println(str1 == str2); // true

String str3 = new String("Merhaba");

// str3 farklı bir String nesnesine referans verir.
System.out.println(str1 == str3); // false

String str4 = "Merhaba".intern();

// str4 ve str1 aynı String nesnesine referans verir.
System.out.println(str1 == str4); // true

</details>

<details>

<summary>Autoboxing boxing nedir?
?</summary>

Wrapper'lar primative 8 değişkenin (byte,short,int,long,float,double,boolean,char) class halleridir. Autoboxing primative bir değişkenin wrapper sınıf tipine otomatik olarak dönüştürme işlemine denir. Boxing ise yine aynı wrapper sınıfına dönüştürme işlemidir ancak new ile üretilip constructor içerisinde bir initialization yapılır.
Process ve Thread arasındaki farklar nelerdir?
Günümüzde bir bilgisayar sisteminde tek bir işlem birimi olsa dahi, bu tek işlem birimi(işlemci) işletim sisteminin kaynak kullanım stratejisine göre her birine belli bir zaman ayırma esasına göre işlem yapmaktadır. Dolayısıyla bilgisayarda aynı anda çok sayıda thread ve process bulunmaktadır. Process kendisine ait kaynakları olan işlem birimidir. Örneğin her process kendisine ait hafıza alanına sahiptir. Theadler de processler gibi işlem birimleridir ve hafif siklet processler (lightweight processes) olarak adlandırılır. Theadler daha az kaynağa ihtiyaç duymaktadır. Theadler bir process içinde yer almaktadır yani her Thead mutlaka bir processe sahiptir ve onun kaynaklarından faydalanır. Theadler de processler gibi uygulamalarda paralelllik elde etmek için kullanılır. Ancak processler daha bağımsız işletim birimleridir kendilerine ait durum bilgileri, kendilerine ait adres alanları varodr. Bir process içerisinde birçok thread barındırabilir ve herbir thread mutlaka bir process içinde yer almaktadır. Aynı process içindeki tüm Theadler aynı hafıza ve aynı durumu paylaşır birbirleriyle direkt olarak haberleşebilirler çünkü aynı alanı paylaşırlar.

</details>

<details>

<summary>Coupling nedir?
?</summary>

iki sınıfın birbirine olan bağımlılığı diyebiliriz. OOP'de nesnelerin birbirleriyle az bağımlı olması benimsenir. (Low coupling) Örnek olarak A sınıfı B sınıfına ne kadar bağımlıysa coupling bir o kadar artar. Bu da projenin bakımını ve genişletilebilirliğini azaltır. Low coupling için çeşitli prensipler uygulanır. Interface kullanımı, design patternler gibi.
Stored Procedure Nedir?
Procedure belli bir işi yapan kod parçasıdır. Stored Procedure Database server ında tutulan ve ilk derlemeden sonra bir daha derlenmeye ihtiyaç duyulmayan SQL ifadeleridir.
Trigger Nedir?
Trigger yani tetikleyici, ilişkisel veri tabanı yönetim sistemlerinde bir tabloda belirli olaylar meydana geldiği zaman yani ekleme, güncelleme, silme işlemlerinden biri gerçekleşmeden önce veya sonra çalışan ve belirli işlemleri kodlandığı şekilde yerine getiren yordamdır.
Factory design pattern nedir?
Bir sınıf oluşturup arada bir interface kullanarak, kullanılacak sınıflar kümelenebilir, bununla birlikte araya bir factory (fabrika) sınıfı eklenere soyut bir biçimde daha anlaşılabilir bir biçimde yazılmasına factory design pattern denir.
JPA / Hibernate arasındaki fark nedir?
JPA bir spesifikasyondur, yani kurallar bütünüdür. Java EE ve Java SE uygulamalarında kullanılır. Java Persistence API kendi başına bir şey yapamaz, bir implementation'a yani uygulamak için bir araca ihtiyaç duyar.Hibernate, Java geliştiricileri için geliştirilmiş bir ORM kütüphanesidir. Nesne yönelimli modellere göre veritabanı ile olan ilişkiyi sağlayarak, veritabanı üzerinde yapılan işlemleri kolaylaştırır.JPA sadece bir spesifikasyon, yani bir implementasyonu yok. JPA'yı izlenmesi gereken yönergeler veya bir arabirim olarak düşünürken, Hibernate JPA uygulaması, JPA tarafından tanımlanan API altında işlevsellik sağlayan koddur.

</details>

<details>

<summary>Thead yaratmanın iki yolu nedir?
?</summary>

1-Runnable interface'ini implemente ederek.
2-Thread sınıfını extend ederek.

</details>

<details>

<summary>Java’da Fetch Stratejileri nelerdir?
?</summary>

nedir abi

</details>

<details>

<summary>DDL Komutları Nelerdir?
?</summary>

DDL (Data Definition Language): Veri Tanımlama Dili (DDL) deyimleri tabloları, veritabanı yapısı veya şema tanımlamak için kullanılır.
CREATE — Veritabanındaki nesneleri oluşturmak için kullanılır.
ALTER — Veritabanı nesnelerinin yapısını değiştirmek için kullanılır.
DROP — Veritabanındaki nesneleri silmek ya da başka bir ifadeyle ilgili nesneleri bütünüyle kaldırmak için kullanılır.
TRUNCATE — Kayıtlar için ayrılan tüm boşluklar dahil, bir tablodaki tüm kayıtları kaldırılır
COMMENT — Veri sözlüğüne yorum eklemek için kullanılır.
RENAME — Bir nesneyi yeniden adlandırmak için kullanılır.

</details>

<details>

<summary>DML Komutları Nelerdir?
?</summary>

DML (Data Manipulation Language): Veri İşleme Dili (DML) deyimleri tablo ya da şema nesneleri içindeki verileri yönetmek için kullanılır.
SELECT — Veritabanından kayıt çekmek için kullanılır.
INSERT — Tabloya kayıt ya da kayıtları eklemek için kullanılır.
UPDATE — Tablodaki kayıt ya da kayıtları güncellemek için kullanılır.
DELETE — Tablodan kayıt ya da kayıtları silmek için kullanılır (Veriler silinse de ancak kapladığı alan kalır)
MERGE — UPSERT işlemi (ekleme veya güncelleme), başka bir ifadeyle birleştirme yapar.
CALL — PL/SQL veya Java alt programını çalıştırır.
EXPLAIN PLAN — Verilere erişim yolunun detaylarını açıklamak için kullanılır.
LOCK TABLE — Kontrolü eş zamanlılığı sağlamak için kullanılır.

</details>

<details>

<summary>DCL KOMUTLARI NELERDİR?
?</summary>

DCL (Data Control Language): Veri Kontrol Dili (DCL) deyimleri yetkilendirme ya da ayrıcalıkları belirlemek için kullanılır.
GRANT — Belirli bir kullanıcı ya da gruba veritabanının belirtilen nesnelerine erişim ayrıcalıklarını verir.
REVOKE — GRANT komutu ile verilen ayrıcalıkların bir kısmını ya da tümünü geri almak için kullanılır.
TCL KOMUTLARI NELERDİR?
TCL (Transaction Control): İşlem Kontrol (TCL) deyimleri DML ifadeleri tarafından yapılan değişiklikleri yönetmek için kullanılır.
COMMIT — Yapılanları kalıcı hale getirir. İşin tamamlanmasını sağlar.
SAVEPOINT — Daha sonra geri dönülecek bir dönüş noktası belirler.
ROLLBACK — Son COMMIT’e kadar olan yeri geri alır.
Stored procedure nedir?
Database sunucusunda tutulan ve ilk derlemeden sonra bir daha derlemeye ihtiyaç duyulmayan TSQL ifadelerdir.
Belirli bir görevi yerine getirmek amacıyla program içinden çağırarak kullanırız.
İlk çalışmadan sonra derlenmedikleri için çalışmalara hız kazandırırlar.
Network trafiğini azaltırlar.
Sql ifadelerinin geçtiği yerlerdeki parametreleri tek tek değiştirmek yerine store procedure içindeki parametre yada kuralları değiştirirerek istediğimizi yapabiliriz.
Sıklıkla kullanılan işlemler için 1 defa yazıp birden fazla kullanabiliriz.

</details>

<details>

<summary>UnIt test nedir?
?</summary>

Birim testi geliştirmiş olduğumuz kodu test etmek için yazmış olduğumuz koddur.
Kodun veya fonksiyonun belirli bir biriminin davranışını kontrol eder.
Unit test kodlarımızı kullanacak diğer developerlar açısından da önemlidir,diğer developerlar kodun nasıl çalıştığını anlamak için unit testi çalıştırırlar.

</details>

<details>

<summary>Aspect-Oriented Programming nedir?
?</summary>

Aspect-Oriented Programming (AOP), geleneksel programlama paradigmalarında olduğu gibi fonksiyonlar ve nesneler yerine "cross-cutting concern"leri odaklanan bir programlama paradigmasıdır. "Cross-cutting concern"ler, uygulamanın her yerinde tekrar eden ve dağınık bir şekilde yerleştirilebilen iş mantığı parçalarıdır. Örneğin, logging, güvenlik, transaction yönetimi, performans ölçümü gibi işlemler bu kategoriye girer.

AOP, bu tarz tekrarlayan işlemleri tek bir yerde tanımlamayı ve bunları program koduna dağıtmadan uygulamanızın farklı noktalarında uygulanmasını sağlar. Bu sayede kodun okunabilirliği, bakımı ve modülerliği artar.
AOP temel konseptleri:
Aspect: Cross-cutting concern'ü temsil eden bir modül. İşlevsellik tanımlaması ve ne zaman, nerede uygulanacağı gibi kurallar içerir.
Join point: Aspect'in uygulanacağı program akışındaki belirli noktalar. Örneğin, bir metodun çağrılması, bir field'a erişim gibi.
Advice: Aspect'in join point'lerde uygulanacak işlevselliktir. Örneğin, logging için yazının kaydedilmesi, güvenlik için yetki kontrolü yapılması gibi.
Pointcut: Hangi join point'lerde hangi aspect'lerin uygulanacağını belirleyen filtredir.
AOP'nin faydaları:
Kod tekrarını azaltır.
Kodun okunabilirliğini ve anlaşılırlığını artırır.
Bakım ve hata düzeltmeyi kolaylaştırır.
Kodun modülerliğini ve yeniden kullanılabilirliğini artırır.
Logging, güvenlik, transaction yönetimi gibi işlemleri koddan ayırır ve kolayca yönetilebilir hale getirir.
AOP'nin dezavantajları:
Öğrenme ve uygulama eğrisi diğer paradigmalara göre daha zor olabilir.
Bazı durumlarda performans üzerinde hafif bir ek yük oluşturabilir.
Aşırı kullanım kodun anlaşılırlığını azaltabilir.
AOP kullanım alanları:
Logging
Güvenlik
Transaction yönetimi
Performans ölçümü
Hata yönetimi
Caching
Yetkilendirme
Aspect'ler arası iletişim
Örnek:
@Aspect
public class LoggingAspect {

    @Before("execution(* com.example.demo.service.*.*(..))")
    public void logBefore(JoinPoint joinPoint) {
        System.out.println("Metodun Adı: " + joinPoint.getSignature().getName());
        System.out.println("Parametreler: " + Arrays.toString(joinPoint.getArgs()));
    }

    @After("execution(* com.example.demo.service.*.*(..))")
    public void logAfter(JoinPoint joinPoint) {
        System.out.println("Metot bitti!");
    }

}
Logging aspect'i ile bir uygulamadaki tüm metoda giriş ve çıkışlarını loglamak isteyebilirsiniz. Aspect'inizde metodun adını, parametrelerini ve dönüş değerini kayıt eden fonksiyon yer alır. Pointcut ile hangi metodlara uygulanacağını belirleyebilirsiniz. Bu sayede logging kodunu her metoda ayrı ayrı yazmak yerine tek bir yerde yönetebilirsiniz.
Sonuç olarak:
Aspect-Oriented Programming, cross-cutting concern'leri etkili bir şekilde yönetmeye ve kod tekrarını azaltmaya yardımcı olan güçlü bir programlama paradigmasıdır. Ancak öğrenme ve uygulama eğrisi daha zor olabilir ve yanlış kullanıldığında kodun anlaşılırlığını azaltabilir. Uygun durumlarda kullanıldığında kodun okunabilirliğini, bakımı ve modülerliğini artırarak yazılım geliştirme sürecini kolaylaştırabilir.

</details>

<details>

<summary>Jdbc (Java Database Connectivity)nedir?
?</summary>

JDBC (Java Database Connectivity), Java uygulamalarının çeşitli veritabanlarına bağlanıp etkileşim kurmasını sağlayan bir Java API'sidir. Bu sayede Java geliştiricileri veritabanlarında veri ekleme, silme, güncelleme ve sorgulama işlemlerini gerçekleştirebilirler.
JDBC'nin temel özellikleri:
Veritabanı Bağlantısı: JDBC, farklı veritabanlarına (MySQL, Oracle, PostgreSQL, vb.) bağlanmak için JDBC sürücüleri aracılığıyla bir bağlantı mekanizması sağlar.
SQL Sorgu Çalıştırma: JDBC, SQL sorgularını veritabanına gönderip sonuçları alma imkanı sunar.
Veri İşlemleri: JDBC, veritabanlarında veri ekleme, silme, güncelleme gibi işlemleri gerçekleştirmek için çeşitli metotlar sunar.
ResultSet: Veritabanından gelen sorgu sonuçları, okunabilir bir formatta saklanan ResultSet nesneleri ile yönetilir.
Transaction Yönetimi: JDBC, veritabanı işlemlerini bir bütün olarak ele alıp geri almak veya tamamlamak için transaction yönetimi mekanizması sunar.
JDBC'nin faydaları:
Platform Bağımsız: Java platform bağımsız olduğundan JDBC de farklı işletim sistemlerinde veritabanlarına bağlanmak için kullanılabilir.
Esneklik: Farklı veritabanı yönetim sistemlerine farklı sürücüler ile bağlanabilir.
Standart API: Java uygulamaları için standart bir veritabanı erişim arayüzü sunar.
Performans: Veritabanı işlemlerini optimize etmek için çeşitli özellikler sunar.
JDBC'nin dezavantajları:
Karmaşıklık: Veritabanı işlemlerini karmaşık kod yazımı olmadan gerçekleştirmek biraz zor olabilir.
Performans: Bazı durumlarda, diğer veritabanı erişim teknolojilerine göre performans eksikliği yaşanabilir.
Güvenlik: Veritabanı bağlantı bilgilerinin güvenli bir şekilde saklanması ve yönetilmesi gerekir.
JDBC kullanım alanları:
Web uygulamaları
Masaüstü uygulamaları
Veri analizi ve raporlama uygulamaları
ETL (Extract, Transform, Load) uygulamaları
Java'da JDBC kullanımı:
JDBC ile veritabanına bağlanmak ve işlem yapmak için aşağıdaki adımları izleyebilirsiniz:
Veritabanı Sürücüsünü Yükleyin: Uygun JDBC sürücüsünü projenize ekleyin.
Bağlantı Oluşturun: Bir Connection nesnesi oluşturarak veritabanına bağlanın.
Statement veya PreparedStatement Oluşturun: Sorguları çalıştırmak için bir Statement veya PreparedStatement nesnesi oluşturun.
SQL Sorgusunu Yazın: İstediğiniz SQL sorgusunu yazın.
Sorguyu Çalıştırın: Statement veya PreparedStatement nesnesini kullanarak sorguyu veritabanına gönderin.
Sonuçları İşleyin: Veritabanından gelen sonuçları ResultSet nesnesi üzerinden işleyin.
Bağlantıyı Kapatın: İşlem bittiğinde bağlantıyı kapatın.
Sonuç olarak, JDBC, Java uygulamalarının çeşitli veritabanlarına bağlanıp etkileşim kurmasını sağlayan önemli bir araçtır. JDBC'nin doğru şekilde kullanılmasıyla hızlı, güvenilir ve verimli veritabanı uygulamaları geliştirilebilir.

</details>

<details>

<summary>
Acid prensipleri nelerdir?
</summary>

ACID Prensipleri
ACID, veritabanı işlemlerinin güvenilirliğini ve tutarlılığını sağlamak için kullanılan dört temel prensipten oluşur. Bu prensipler şunlardır:

1. Atomicity (Bütünlük): Bir işlemdeki tüm işlemler ya tamamıyla gerçekleşir ya da hiç gerçekleşmez. Bir işlem sırasında bir hata oluşursa, işlem geri alınır ve veritabanı başlangıçtaki haline döner.
2. Consistency (Tutarlılık): Bir işlem veritabanını her zaman tutarlı bir durumda bırakır. Bir işlemden önce veritabanı tutarlıysa, işlemden sonra da tutarlı kalacaktır.
3. Isolation (Yalıtım): Aynı anda birden fazla işlem çalışırken, birbirlerinden etkilenmezler. Her işlem kendi özel bir ortamda çalışıyormuş gibi davranır.
4. Durability (Dayanıklılık): Bir işlem tamamlandıktan sonra, veritabanındaki değişiklikler kalıcı hale gelir. Bir sistem arızası veya güç kesintisi olsa bile, veriler kaybolmaz.
   ACID prensiplerinin faydaları:
   Veritabanı tutarlılığını ve güvenilirliğini sağlar.
   Veri kaybını ve hatalı verileri önler.
   İşlemlerin güvenli ve doğru bir şekilde gerçekleşmesini sağlar.
   ACID prensiplerinin dezavantajları:
   Performansı etkileyebilir.
   Karmaşıklığı artırabilir.
   ACID prensiplerinin kullanımı:
   ACID prensipleri, veritabanı işlemlerinin güvenilirliği ve tutarlılığı kritik önem taşıyan uygulamalarda kullanılır. Örneğin, banka uygulamaları, finansal uygulamalar ve sağlık uygulamaları gibi.
   ACID prensiplerine örnek:
   Bir banka havalesi işleminde, paradan gönderenin hesabından alıcının hesabına aktarılması tek bir işlem olarak gerçekleşir. İşlem sırasında bir hata oluşursa, para transferi gerçekleşmez ve her iki hesap da başlangıçtaki bakiyelerinde kalır.
   Bir e-ticaret sitesinde bir ürün satın alırken, sipariş işlemi ve ödeme işlemi tek bir işlem olarak gerçekleşir. İşlem sırasında bir hata oluşursa, sipariş tamamlanmaz ve ödeme gerçekleşmez.
   Sonuç olarak, ACID prensipleri, veritabanı işlemlerinin güvenilirliğini ve tutarlılığını sağlamak için kullanılan temel prensiplerdir. Bu prensiplerin doğru şekilde kullanılmasıyla güvenli, tutarlı ve hatasız veritabanı uygulamaları geliştirilebilir.

</details>

<details>

<summary>Hard parse ve soft paresnedir?
?</summary>

Hard Parse ve Soft Parse Nedir?
Bu terimler genellikle veritabanı yönetim sistemlerinde (DBMS) karşılaşılan kavramlardır, özellikle Oracle gibi SQL tabanlı sistemlerde. İkisi arasında temel fark, bir SQL sorgusunun işlenme şekliyle ilgilidir.
Hard Parse:
Hard parse (zor ayrıştırma), bir SQL sorgusunun ilk kez çalıştırıldığında veya sorguda bazı önemli değişiklikler yapıldığında meydana gelir.
DBMS, sorguyu tamamen analiz eder, doğrulamasını yapar ve yürütme planı oluşturur.
Bu plan, sorgunun veritabanı tablolarına ve indekslerine nasıl erişeceğini ve verileri nasıl işleme koyacağını belirtir.
Hard parse işlem yoğun olabilir ve performansı etkileyebilir.
Soft Parse:
Soft parse (kolay ayrıştırma), önceden ayrıştırılmış ve önbelleğe alınmış bir sorgu yeniden kullanıldığında gerçekleşir.
DBMS, önbellekte sorgu planını arar ve bulabilirse, yürütme için doğrudan bu planı kullanır.
Soft parse çok daha hızlıdır ve genellikle hard parse'a tercih edilir.
Ancak, sorgu önceden çalıştırılmamışsa veya önbellekteki plan geçerli değilse, bir hard parse gerekebilir.
Soft Parse'ın Avantajları:
Performans artışı: Sorgu planı önceden hazırlandığı için yürütme daha hızlı gerçekleşir.
Kaynak verimliliği: Veritabanı kaynakları, her seferinde yeni bir plan oluşturmak yerine önbelleğe alınmış planları kullanarak korunur.
Ölçeklenebilirlik: Daha fazla kullanıcı aynı sorguları çalıştırdığında, sistem önbelleğe alınmış planları tekrar kullanarak iyi bir performans sergileyebilir.
Hard Parse'ın Ne Zaman Olur:
Sorgu ilk kez çalıştırıldığında.
Sorguda parametre değişikliği yapıldığında.
Veritabanı yapılandırması değiştiğinde.
Önbellekteki plan süresi dolduğunda.
Sonuç olarak:
Hard parse ve soft parse, SQL sorgularının veritabanında işlenmesine ilişkin iki ayrıştırma yöntemidir. Soft parse performans açısından tercih edilir, ancak bir sorgu ilk kez veya önbellekteki plan geçerli değilse hard parse gerekir.

</details>

<details>

<summary>Statement nesnesi ne işe yarar?
?</summary>

Statement Nesnesi Ne İşe Yarar?
Statement nesnesi, JDBC'de SQL sorgularını çalıştırmak için kullanılır. Temel SQL ifadelerini (SELECT, INSERT, UPDATE, DELETE) çalıştırır ve bu ifadelerin değer döndürme özelliğine sahiptir.
Statement Nesnesinin Özellikleri:
SQL Sorgularını Çalıştırır: Statement nesnesi, executeQuery() ve executeUpdate() gibi metotlar aracılığıyla SQL sorgularını veritabanına gönderir ve sonuçları alır.
Değer Döndürme: SELECT sorguları için, Statement nesnesi ResultSet nesnesi aracılığıyla verileri döndürür.
Parametreler: Statement nesnesi, sorgularda parametre kullanımı için setString() ve setInt() gibi metotlar sunar.
DML (Data Manipulation Language) İşlemleri: INSERT, UPDATE ve DELETE gibi DML işlemleri için Statement nesnesi kullanılabilir.
Statement Nesnesi Kullanımı:
Java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.ResultSet;
import java.sql.Statement;

public class Main {

    public static void main(String[] args) throws Exception {
        // Veritabanına bağlantı kurma
        Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/database", "username", "password");

        // Statement nesnesi oluşturma
        Statement statement = connection.createStatement();

        // SELECT sorgusu çalıştırma
        ResultSet resultSet = statement.executeQuery("SELECT * FROM users");

        // Verileri işleme
        while (resultSet.next()) {
            System.out.println(resultSet.getString("name"));
        }

        // INSERT sorgusu çalıştırma
        statement.executeUpdate("INSERT INTO users (name, age) VALUES ('John Doe', 30)");

        // Bağlantıyı kapatma
        connection.close();
    }

}

Bu örnekte, Statement nesnesi bir SELECT sorgusu çalıştırmak ve sonuçları yazdırmak için kullanılır. Ayrıca, bir INSERT sorgusu çalıştırmak için de kullanılır.
Statement Nesnesi Türleri:
Statement: Temel SQL ifadelerini çalıştırmak için kullanılır.
PreparedStatement: Parametreli sorguları çalıştırmak için kullanılır ve performansı optimize eder.
CallableStatement: Stored procedure'ları (saklı prosedürler) çalıştırmak için kullanılır.

</details>

<details>

<summary>PreparedStatement nasıl çalışır?
?</summary>

PreparedStatement Nasıl Çalışır?
PreparedStatement, JDBC'de parametreli SQL sorgularını çalıştırmak için kullanılan bir nesnedir. Statement nesnesine kıyasla performans optimizasyonu ve SQL enjeksiyonu gibi güvenlik açıklarına karşı koruma sağlar.
PreparedStatement Çalışma Prensibi:
Sorgunun Hazırlanması:
PreparedStatement nesnesi oluşturulur ve SQL sorgusu parametreleri ile birlikte bu nesneye gönderilir.
Veritabanı, sorgunun syntax'ını kontrol eder ve yürütme planı oluşturur.
Sorgu planı önbelleğe alınır ve daha sonra tekrar kullanılabilir.
Parametrelerin Değerlendirilmesi:
Sorgudaki parametrelere değerler set metotları ile atanır.
Veritabanı, parametre değerlerini sorguda yerleştirir.
Sorgunun Çalıştırılması:
executeUpdate() veya executeQuery() metotları ile sorgu çalıştırılır.
Veritabanı, önceden hazırlanmış planı kullanarak sorguyu işler.
PreparedStatement'ın Avantajları:
Performans Optimizasyonu: Sorgu planı önceden hazırlandığı için her seferinde yeniden oluşturulmaz ve bu da performansı artırır.
Güvenlik: SQL enjeksiyonu gibi güvenlik açıklarına karşı koruma sağlar. Parametre değerleri sorgudan ayrı olarak değerlendirilir.
Tekrar Kullanılabilirlik: Aynı sorgu farklı parametrelerle tekrar tekrar çalıştırılabilir.
PreparedStatement'ın Dezavantajları:
Statement'a Göre Karmaşık: PreparedStatement nesnesi oluşturmak ve parametreleri atamak Statement nesnesine göre daha karmaşıktır.
PreparedStatement Kullanım Örneği:
Java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.PreparedStatement;
import java.sql.ResultSet;

public class Main {

    public static void main(String[] args) throws Exception {
        // Veritabanına bağlantı kurma
        Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/database", "username", "password");

        // PreparedStatement nesnesi oluşturma
        PreparedStatement statement = connection.prepareStatement("SELECT * FROM users WHERE name = ? AND age = ?");

        // Parametrelere değer atama
        statement.setString(1, "John Doe");
        statement.setInt(2, 30);

        // SELECT sorgusu çalıştırma
        ResultSet resultSet = statement.executeQuery();

        // Verileri işleme
        while (resultSet.next()) {
            System.out.println(resultSet.getString("name"));
        }

        // Bağlantıyı kapatma
        connection.close();
    }

}

</details>

<details>

<summary>Normalizasyon nedir?
?</summary>

Normalizasyon Nedir?
Normalizasyon, veritabanındaki tabloların içeriğini organize etme tekniğidir. Verileri farklı tablolara ayırarak aşağıdaki sorunları ortadan kaldırmak veya azaltmak için kullanılır:
Veri Tekrarı: Aynı bilginin birden fazla tabloda yer alması.
Eksik Veri: Bir tablodaki bazı bilgilere diğer tablodan erişilmesi gerektiği durum.
Anomali: Veritabanındaki bir değişikliğin birden fazla tabloda tutarsızlık yaratması.
Normalizasyon Seviyeleri:
Normalizasyon, çeşitli seviyelerde uygulanabilir. Her seviye, veri tekrarını ve tutarsızlığı azaltmaya yardımcı olur. En yaygın normalizasyon seviyeleri şunlardır:

1. Normal Form (1NF): Her satırın benzersiz bir anahtara sahip olması ve her sütunun atomik olması (ayrıştırılamaz) gerekir.
2. Normal Form (2NF): 1NF'i sağlamanın yanı sıra, her sütunun birincil anahtara tam bağımlı olması gerekir.
3. Normal Form (3NF): 2NF'i sağlamanın yanı sıra, her sütunun geçişsiz bağımlılık olması gerekir.
   Normalizasyon Teknikleri:
   Normalizasyon, aşağıdaki teknikler kullanılarak uygulanabilir:
   Ayrıştırma: Bir tabloyu birden fazla tabloya bölme işlemi.
   Fonksiyonel Bağımlılık Analizi: Hangi sütunların hangi sütunlara bağımlı olduğunu belirleme işlemi.
   Asıl Anahtar Belirleme: Her satırı benzersiz şekilde tanımlayan bir sütun veya sütun grubu seçme işlemi.
   Normalizasyonun Avantajları:
   Veri Tutarlılığı: Veritabanındaki tutarsızlıkları ve hataları azaltır.
   Veri Erişimi: Verilere erişimi kolaylaştırır ve hızlandırır.
   Veri İşlemleri: Veri ekleme, silme ve güncelleme işlemlerini kolaylaştırır.
   Depolama Alanı: Veri tekrarını azaltarak depolama alanından tasarruf sağlar.
   Normalizasyonun Dezavantajları:
   Karmaşıklık: Veritabanı tasarımını ve uygulamasını karmaşıklaştırabilir.
   Performans: Bazı durumlarda, sorguların performansını olumsuz etkileyebilir.
   Sonuç olarak:
   Normalizasyon, veritabanındaki veri tutarlılığı, erişimi ve işlenmesini optimize etmek için kullanılan önemli bir tekniktir. Doğru şekilde uygulandığında, veritabanı performansını ve güvenilirliğini artırır.

</details>

<details>

<summary>Normal formlar nelerdir?1nf ye örnek veriniz
?</summary>

Normal Formlar ve 1NF Örneği
Normal Formlar:
Normalizasyon, veritabanındaki tabloların içeriğini organize etme tekniğidir. Verileri farklı tablolara ayırarak veri tekrarı, eksik veri ve anomali gibi problemleri ortadan kaldırmak veya azaltmak için kullanılır. Normalizasyonun farklı seviyeleri vardır ve her seviye bir önceki seviyenin üzerine inşa edilir.
En yaygın normal formlar şunlardır:

1. Normal Form (1NF): Her satırın benzersiz bir anahtara sahip olması ve her sütunun atomik olması (ayrıştırılamaz) gerekir.
2. Normal Form (2NF): 1NF'i sağlamanın yanı sıra, her sütunun birincil anahtara tam bağımlı olması gerekir.
3. Normal Form (3NF): 2NF'i sağlamanın yanı sıra, her sütunun geçişsiz bağımlılık olması gerekir.
   1NF Örneği:
   Öğrenci tablosu:
   <figure><img src="assets/tables/unnamed (21).png" alt=""><figcaption></figcaption></figure>

   Bu tablo 1NF'dedir çünkü:
   Her satırın benzersiz bir anahtarı vardır (Öğrenci No).
   Her sütun atomiktir (ayrıştırılamaz).
   Ancak, bu tabloda veri tekrarı vardır. Bölüm bilgisi her satırda tekrarlanmaktadır. Bu veri tekrarını ortadan kaldırmak için Bölüm adında ayrı bir tablo oluşturabiliriz:
   Bölüm tablosu:
   <figure><img src="assets/tables/unnamed (22).png" alt=""><figcaption></figcaption></figure>

   Öğrenci tablosu:
   <figure><img src="assets/tables/unnamed (23).png" alt=""><figcaption></figcaption></figure>

   Bu şekilde, Bölüm bilgisi tek bir yerde tutulur ve veri tekrarı ortadan kalkar.
   1NF'de olması gereken diğer özellikler:
   Her satırda null değer olmamalıdır.
   Birincil anahtar birden fazla sütundan oluşabilir.
   İki farklı satırda aynı değerler tekrarlanamaz.

</details>

<details>

<summary>NoSQL Nedir ?
?</summary>

NoSQL, "Not Only SQL" veya "No Structured Query Language" anlamına gelir. Geleneksel ilişkisel veritabanlarına (RDBMS) alternatif olarak ortaya çıkan bir veritabanı yönetim sistemleri (DBMS) ailesidir.
NoSQL'in Özellikleri:
Şema Esnekliği: NoSQL veritabanları, önceden tanımlanmış bir şemaya ihtiyaç duymaz. Veriler, JSON, XML veya NoSQL'e özgü formatlar gibi farklı formatlarda depolanabilir.
Yatay Ölçeklenebilirlik: NoSQL veritabanları, yatay olarak ölçeklenebilir şekilde tasarlanmıştır. Bu, veri yükü arttıkça daha fazla sunucu ekleyerek veritabanının kapasitesini kolayca artırabileceğiniz anlamına gelir.
Hızlı Performans: NoSQL veritabanları, belirli veri modelleri için optimize edilmiştir ve bu nedenle RDBMS'den daha hızlı performans sunabilir.
NoSQL Veritabanı Türleri:
Anahtar-Değer Mağazaları: Anahtar-değer mağazaları, anahtar-değer çiftlerini depolayan basit bir NoSQL veritabanı türüdür. Redis ve Memcached bu türün popüler örnekleridir.
Belge Veritabanları: Belge veritabanları, JSON gibi yarı yapılandırılmış verileri depolayan NoSQL veritabanı türüdür. MongoDB ve CouchDB bu türün popüler örnekleridir.
Sütun Aileleri: Sütun aileleri, satır ve sütunlardan oluşan tablolar gibi bir yapıya sahip NoSQL veritabanı türüdür. Cassandra ve HBase bu türün popüler örnekleridir.
Grafik Veritabanları: Grafik veritabanları, nesneler ve bunlar arasındaki ilişkileri depolayan NoSQL veritabanı türüdür. Neo4j ve Titan bu türün popüler örnekleridir.
NoSQL'in Kullanım Alanları:
Sosyal Medya: Sosyal medya platformları, büyük miktarda kullanıcı verisi ve etkileşimi depolamak için NoSQL veritabanlarını kullanır.
E-ticaret: E-ticaret platformları, ürün katalogları ve müşteri siparişleri gibi verileri depolamak için NoSQL veritabanlarını kullanır.
IoT: IoT cihazları tarafından üretilen büyük miktarda veriyi depolamak için NoSQL veritabanları kullanılır.
NoSQL'in Avantajları:
Esneklik: NoSQL veritabanları, farklı veri modelleri ve formatları için esneklik sunar.
Ölçeklenebilirlik: NoSQL veritabanları, yatay olarak ölçeklenebilir şekilde tasarlanmıştır.
Performans: NoSQL veritabanları, belirli veri modelleri için optimize edilmiştir ve bu nedenle RDBMS'den daha hızlı performans sunabilir.
NoSQL'in Dezavantajları:
Veri Tutarlılığı: NoSQL veritabanları, RDBMS'deki kadar güçlü veri tutarlılığı garantilerini sunmayabilir.
Sorgulama Karmaşıklığı: NoSQL veritabanları, RDBMS'deki kadar karmaşık sorguları desteklemeyebilir.
Güvenlik: NoSQL veritabanları, RDBMS'ye kıyasla daha az güvenli olabilir.
NoSQL'in Uygun Olup Olmadığını Belirleme:
NoSQL veritabanı, her uygulama için uygun olmayabilir. NoSQL'i kullanmayı düşünüyorsanız, aşağıdakileri göz önünde bulundurmanız gerekir:
Veri modeliniz: Veriniz şemalı mı yoksa şemasız mı?
Veri yükünüz: Ne kadar veri depolayacaksınız?
Performans gereksinimleriniz: Ne kadar hızlı performansa ihtiyacınız var?
Yetenek gereksinimleriniz: Karmaşık sorgulara ihtiyacınız var mı?

</details>

<details>

<summary>NoSQL Sistemlerin Dezavantajları Nelerdir?
?</summary>

NoSQL sistemler, ilişkisel veritabanlarına (RDBMS) kıyasla birçok avantaj sunsa da, bazı dezavantajları da vardır.
NoSQL Sistemlerin Dezavantajları:
Veri Tutarlılığı: NoSQL sistemler, ACID işlemleri gibi ilişkisel veritabanlarındaki veri tutarlılığı garantilerini sunmaz. Bu, bazı durumlarda veri tutarsızlığına yol açabilir.
Sorgulama Karmaşıklığı: NoSQL sistemler, ilişkisel veritabanlarına kıyasla karmaşık sorguları desteklemede daha zayıf olabilir.
Güvenlik: NoSQL sistemler, ilişkisel veritabanlarına kıyasla daha az güvenli olabilir.
Yedekleme ve Geri Yükleme: NoSQL sistemler için yedekleme ve geri yükleme işlemleri daha karmaşık olabilir.
İşlem Takibi: NoSQL sistemlerde işlem takibi ve hata ayıklama daha zor olabilir.
Yetenek Eksikliği: NoSQL sistemler, ilişkisel veritabanlarında bulunan bazı gelişmiş özelliklere sahip olmayabilir.
NoSQL Sistemlerin Dezavantajlarının Örnekleri:
Bir NoSQL sisteminde birden fazla veri tabanı arasında birleştirme yapmak zor olabilir.
NoSQL sistemlerde karmaşık sorguları çalıştırmak performans sorunlarına yol açabilir.
NoSQL sistemlerde veri tutarsızlığı riski daha yüksektir.
NoSQL Sistemlerin Dezavantajlarını Gidermek için Çözümler:
NoSQL sistemler için özel olarak tasarlanmış tutarlılık ve sorgular için araçlar ve kütüphaneler kullanılabilir.
Güvenliği artırmak için NoSQL sistemleri için özel güvenlik çözümleri kullanılabilir.
Yedekleme ve geri yükleme işlemleri için özel araçlar ve çözümler kullanılabilir.
NoSQL Sistemlerin Dezavantajlarını Dikkate Alırken:
NoSQL sistemlerin dezavantajları, her bir sistemin türüne ve kullanım amacına göre değişebilir. NoSQL sistemi seçerken, bu dezavantajları ve uygulamanız için ne kadar önemli olduklarını göz önünde bulundurmanız önemlidir.

</details>

<details>

<summary>Execution Plan Nedir?
?</summary>

Execution plan, bir veritabanı yönetim sisteminde (DBMS) bir SQL sorgusunun nasıl yürütüleceğini tanımlayan bir belgedir. Sorguyu işlemenin en verimli yolunu belirlemek için DBMS tarafından otomatik olarak oluşturulur.
Execution plan aşağıdaki bilgileri içerebilir:
Sorgulanacak tablolar: Sorgunun hangi tablolardan veri okuyacağı.
Katılım koşulları: Tablolardan hangi verilerin filtreleneceği.
Verilerin nasıl birleştirileceği: Birden fazla tablodan gelen verilerin nasıl birleştirileceği.
Verilerin nasıl sıralanacağı: Sonuç setinin nasıl sıralanacağı.
Hangi indekslerin kullanılacağı: Hangi indexlerin sorgunun performansını artırmak için kullanılacağı.
Tahmini maliyet: Sorguyu yürütmenin tahmini maliyeti, örneğin CPU, bellek ve disk I/O kullanımı.
Execution Planın Faydaları
Sorgu performansını optimize etmek: Execution planı, DBMS'nin en verimli yürütme planını seçmesine yardımcı olur ve böylece sorgu performansını iyileştirir.
Sorunları teşhis etmek: Karmaşık sorgularda veya performans sorunlarının yaşandığı durumlarda execution planı, sorunun kaynağını tanımlamaya yardımcı olabilir.
Sorguyu anlamak: Execution planı, veritabanı yöneticilerinin ve geliştiricilerin sorgunun nasıl çalıştığını daha iyi anlamasına yardımcı olabilir.
Execution Planı Nerede Bulunur?
Execution planın nasıl erişileceği ve görüntülenebileceği DBMS'ye göre değişebilir. Bazı DBMS'lerde execution plan otomatik olarak sorgunun sonucuyla birlikte döndürülürken, diğerlerinde özel araçlar kullanılarak elde edilmesi gerekebilir.
Umarım bu açıklamalar execution plan hakkında size daha fazla bilgi vermiştir. Eğer sorunuz varsa, çekinmeden sorun!

</details>

<details>

<summary>Mikroservis mimari bir projede Transactional bir problem ortaya çıkması durumunda neler yapabilirsin??</summary>

Mikroservis mimarisi, her biri kendi veri tabanına ve iş mantığına sahip bağımsız hizmetlerden oluşan bir sistemdir.
Transactional problemler:
Birden fazla servisi kapsayan işlemlerde tutarlılık sağlamak zor olabilir.
Bir serviste hata oluşması durumunda, diğer servislerde de tutarsızlıklar oluşabilir.
Veritabanları arasında veri kopyalama ve eşitleme işlemleri karmaşık olabilir.
Transactional problemleri çözmek için:
İki aşamalı commit (2PC): Her servis, işlemin ilk aşamasında yerel veritabanında değişiklikleri yapar ve ikinci aşamada ise commit veya rollback kararı verir.
Saga pattern: Her servis, işlemin bir adımını gerçekleştirir ve bir sonraki servise bir mesaj gönderir. Bir adımda hata oluşması durumunda, saga pattern işlemi geri alır.
Event sourcing: Her işlem, bir olay olarak kaydedilir ve bu olaylar, veritabanındaki durumu tutarlı tutmak için kullanılır.
Compensation pattern: Bir serviste hata oluşması durumunda, hatayı telafi etmek için bir işlem gerçekleştirilir.
Hangi çözümün kullanılacağı, projenin özel gereksinimlerine bağlıdır.
Ek olarak:
Servisler arasında iletişim için güvenilir bir mesajlaşma sistemi kullanılmalıdır.
Veritabanları arasında veri kopyalama ve eşitleme işlemleri için sağlam bir altyapı kurulmalıdır.
Tüm servisler ve veritabanları için izleme ve hata ayıklama araçları kullanılmalıdır.
Transactional problemler, mikroservis mimarili projelerde önemli bir zorluktur. Bu problemleri çözmek için çeşitli teknikler kullanılabilir. Hangi çözümün kullanılacağı, projenin özel gereksinimlerine bağlıdır.

</details>

<details>

<summary>Bearer token nedir ve ne için kullanılır?
?</summary>

Bearer token, bir kullanıcının bir API'ye kimlik doğrulaması için kullandığı bir kimlik doğrulama belirtecidir. Genellikle bir JWT (JSON Web Token) formatında olur ve Authorization HTTP başlığında gönderilir.
Bearer token'ın çalışma prensibi:
Kullanıcı, bir API'ye erişmek için bir kimlik doğrulama isteği gönderir.
API, kullanıcının kimlik bilgilerini doğrular ve doğruysa bir bearer token üretir.
Bearer token, Authorization HTTP başlığında "Bearer" ön eki ile birlikte kullanıcıya gönderilir.
Kullanıcı, API'ye erişmek için her istekte Authorization HTTP başlığında bearer token'ı gönderir.
API, bearer token'ı doğrular ve kullanıcıya erişim izni verir.
Bearer token'ın faydaları:
Kullanıcı kimlik doğrulama işlemini basitleştirir.
Kullanıcı kimlik bilgilerinin her istekte gönderilmesini önler.
API'ye erişimi kontrol etmek için kullanılabilir.
Bearer token'ın dezavantajları:
Çalınabilir veya tahmin edilebilir.
Güvenli bir şekilde saklanması gerekir.
Bearer token'ın kullanıldığı bazı durumlara örnek:
API'lere erişimi kontrol etmek
Kullanıcı oturumlarını yönetmek
Mobil uygulamalarda kimlik doğrulama
Bearer token'a alternatifler:
Session cookie'ler
OAuth
Hangi kimlik doğrulama yönteminin kullanılacağı, projenin özel gereksinimlerine bağlıdır.

session ve cookie nasıl çalışır?
Session:
Bir kullanıcının bir web sitesi veya uygulama ile etkileşimi sırasında geçici bir veri depolama alanıdır.
Kullanıcının kimlik bilgilerini, alışveriş sepeti gibi bilgileri ve diğer geçici verileri saklamak için kullanılır.
Sunucu tarafında saklanır.
Her kullanıcının ayrı bir session'ı vardır.
Session'ın süresi dolduğunda veya kullanıcı oturumunu kapattığında sona erer.
Cookie:
Bir web sitesi veya uygulamanın kullanıcının bilgisayarına yerleştirdiği küçük bir metin dosyasıdır.
Kullanıcının kimlik bilgilerini, tercihlerini ve diğer ayarları saklamak için kullanılır.
İstemci tarafında saklanır.
Birden fazla web sitesi veya uygulama tarafından kullanılabilir.
Cookie'nin süresi dolduğunda veya kullanıcı tarafından silinene kadar saklanır.
Session ve cookie arasındaki farklar:

<figure><img src="assets/tables/unnamed (15).png" alt=""><figcaption></figcaption></figure>

Session ve cookie birlikte nasıl çalışır:
Kullanıcı bir web sitesini veya uygulamayı ziyaret ettiğinde, sunucu bir session oluşturur ve kullanıcının bilgisayarına bir cookie yerleştirir.
Cookie, kullanıcının kimlik bilgilerini ve diğer ayarları içerir.
Kullanıcı web sitesi veya uygulama ile etkileşime girdiğinde, cookie sunucuya gönderilir.
Sunucu, cookie'yi kullanarak kullanıcının session'ını ve geçici verilerini alır.
Kullanıcı oturumunu kapattığında veya session'ın süresi dolduğunda, session ve cookie silinir.
Session ve cookie'nin kullanıldığı bazı durumlara örnek:
Kullanıcı kimlik doğrulama
Kullanıcı tercihlerini saklama
Alışveriş sepeti takibi
Session ve cookie'nin güvenliği:
Session ve cookie'ler, çalınabilir veya tahmin edilebilir.
Güvenli bir şekilde kullanılmaları gerekir.
HTTPS gibi güvenli bir protokol kullanılmalıdır.
Session ve cookie'lerin süresi dolduğunda veya kullanıcı oturumunu kapattığında silinmelidir.

</details>

<details>

<summary>soru?</summary>

public static void main(String [Jargs)
Integer a = 50;
Integer b = 50;
System.out.println(\*a == b?

- (a = b) );
  Integer c = 500:
  Integer d = 500;
  System.out-println(\*c = d?" + (c = d) );

JVM parametrelerinin default değerleri koruduğu varsayılarak -127 +128 değerleri arasını cacheler ve bu değerler arasına yazılan iki farklı sayıyı aynı referans noktalarına atar. Bundan dolayı birinci ifade true, ikinci ifade false çıktısını verir.

</details>

<details>

<summary>soru?</summary>

public static void main(String args[]) ‹
System.out -printin(0.1 _ 3 == 0.3);
System.out.println(0.1 _ 2 ==
0.2);

Float değişken derin binary formatinda nasil saklandığı
ile alakali olan bu soruda, 0.2 tam olarak binary sisteme
cevrilebilirken 0.3 tam olarak binary sisteme çevrilemez
ve bundan dolayı:
false
true
çıktısını alırız.

</details>

<details>

<summary>soru?</summary>

public static void main(String[] args) {
int intValue = Integer MAX_VALUE;
intValue++;
System.out.println(intValue);

overflow söz konusudur, max value üstüne bir değer daha eklenince min value -231231 gibi bir değere ulaşılır

</details>

<details>

<summary>soru?</summary>

class A {
static void staticMethod() {
System.out println( "Static Method");
public class MainClass { »
public static void main(String(] args) {
A a = null;
a.staticMethod();

static metotlar nesne üzerinden değil sınıf üzerinden çağrıldıkları için örneği yaratılmayan bir sınıfa ait static method da çağırıldığı zaman çalışılacaktır.

</details>

<details>

<summary>soru?</summary>

cevap

</details>

<details>

<summary>soru?</summary>

public static void main(String() args) ‹
String(] array = {"Turkey", "Java"};
List«String> v = Arrays.asList(array);
v.set(0, "Community");
System.out.println(v.contains("Community"));
}

true değeri verir, asList den dönen özelleştirilmiş listede elemanların eklenmesine veya çıkarılmasına izin verilmez ancak set operasyonunu gerçekleştirebiliriz.

</details>

<details>

<summary>soru?</summary>

public interface Interface {
static void main(String
args) €
System. out - printin("This is interface")
public class ClassA implements Interface {
public static void main(String) args) ‹
InterfaceA.main(new String [ 10]);
System.out println( "This is class");

This is interface
This is class

</details>
