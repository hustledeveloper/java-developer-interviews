# java-developerMulakat-Sorulari

### *Java ve OOP*

<details>

<summary>soru?</summary>

cevap


```java
kodlar kodlar
```

</details>


<figure><img src="assets/solid.gif" alt=""><figcaption></figcaption></figure>



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

<summary>++İmplement, extend ve instanceof kavramlarını açıklayınız?
</summary>

Implement: Bir sınıfın belirli bir davranışa sahip olduğunu belirtmek için kullanılmalıdır. Bu davranış arayüzde tanımlanır ve sınıf bu arayüzü implement ederek bu davranışı sağlamalıdır.
Extend: Bir sınıftan yeni bir sınıf oluşturmak ve üst sınıfa ait özellikleri ve metotları kullanarak yeni bir davranış eklemek istediğinizde kullanılır.
Instanceof operatörü, bir nesnenin belirli bir sınıftan veya arayüzden olup olmadığını kontrol etmek için kullanılır.


</details>

<details>

<summary>++Java'da Encapsulation Nedir?</summary>

Encapsulation, bir sınıfın üyelerini (değişkenler ve metotlar) korumak ve saklamak için kullanılan bir tekniktir. Bu teknik, sınıfın iç yapısını kullanıcılardan gizleyerek ve sadece belirli erişim izinleri sağlayarak kodun daha güvenli ve sağlam olmasını sağlar.
Encapsulation'ın faydaları:
Güvenlik: Sınıfın üyelerini yetkisiz erişimden korur.
Değişiklik esnekliği: Sınıfın iç yapısını değiştirmeyi kolaylaştırır.
Kodun sağlamlığı: Hatalı kodların ve veri tutarsızlıklarının önüne geçer.
Bakım kolaylığı: Kodun daha okunabilir ve anlaşılır olmasını sağlar.
Encapsulation nasıl uygulanır:
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

<summary>++Java'da Polymorphism Nedir?
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

<summary>++Java’da hata ayıklanması (exception handling) nasıl yapılır?
?</summary>

Java'da hata ayıklama, try-catch blokları ve throw anahtar sözcüğü ile yapılır.
try-catch Blokları:
try bloğu, hataya neden olabilecek kodları içerir.
catch bloğu, hataya ne zaman ve nasıl tepki verileceğini tanımlar.
throw Anahtar Sözcüğü:
throw anahtar sözcüğü, kasıtlı olarak bir hata oluşturmak için kullanılır.


</details>

<details>

<summary>++throw ile throws arasındaki fark nedir??</summary>

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


</details>


<details>

<summary>++Java’da nesneleri karşılaştırıken .equals() ile == kullanmanın farkı nedir?</summary>

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

<summary>++Java’da bir alt sınıf üstün private metodları kullanabilir mi?
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

<summary>soru?</summary>

cevap


```java
kodlar kodlar
```

</details>


<details>

<summary>soru?</summary>

cevap


```java
kodlar kodlar
```

</details>


<details>

<summary>soru?</summary>

cevap


```java
kodlar kodlar
```

</details>
