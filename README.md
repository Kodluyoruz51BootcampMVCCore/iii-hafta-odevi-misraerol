# III-hafta-odevi


1.Task vs process- task vs Thread vs .. ve c# task vs thread vs .. kıyaslamalarını ve task haricinde diğer yöntemler nelerdir araştırınız.
2.Extension Nedir? --> Extra paket ekleme. <br/>
3.SQLite, bunu doğru şekilde (en güncel yol ile) nasıl kullanmalıyız? (Aktif halde kullanıp uygulama)

## TASK vs Thread
Async programlama ile daha sıklıkla kullanılan Task yapısı thread yapısına göre üst seviyede. Task yapısını kullanarak daha gelişmiş işlemler yapabiliriz. Thread pooling yapısını otomatik olarak kullanıp birbiri ardına eklenebilecek olan işlemleri daha iyi organize etmektedir.


## TASK vs Process
Thread yapıları işletim sistemi işlemlerine benzemektedir. OS içerisinde işlemler birbirine paralel olarak çalışmaktadır. Thread yapısında ise, threadler bir process içerisinde birbirlerine paralel olarak çalışmaktadırlar. İşlemler birbirlerine tamamen izoledir. Threadler birbirlerine tamamen izole değillerdir. Aynı hafızayı paylaşırlar bundan dolayı birlikte çalışan threadler arasından veriler rahatça paylaşılmaktadır.

## TASK vs ValueTask


## TASK vs Parallel
Paralel programlama ise farklıdır. Her ne kadara bu yazıda bahsetmeyecek olsak bile bahsetmekte fayda olduğunu düşünüyorum.  Paralel programlama ile sistemin CPU performansı gibi özellikler ön plandadır ve tüm çalışan thread yapıları tek bir işlemi yapmak için çalışır. Belirli bir task’ı birden fazla thread kullanacak hızlıca tamamlamaktır. Task’ı tamamlamak için birden fazla kaynak kullanmak olarak düşünebiliriz.

## Extension Nedir?
Kelime anlamı genişletilebilir metod olan Extension Method'lar C#3.0 ile hayatımıza girmiştir ve yaptığı iş itibatiyle kullanım açısından son derece faydalı metodlardır. Tek cümleyle özetlemek gerekirse class ve struct yapılarını modify etmeden ilgili struct yada class'için extension metodlar eklememizi sağlar.</br>
<ul>

<li>Bizi sürekli aynı kodları yazmaktan kurtarır.</li>
<li>Statik metodlar ve statik classlardan oluşur.Referans olarak oluşturduğumuz obje üzerinden çağrılır. </li>
<li>Extension metodlar statik metodlar ve statik classlardan oluşmaktadır. Fakat referans olarak oluşturduğunuz obje üzerinden çağrılırlar.  </li>
<li> Extension metodların aldığı ilk parametre, bu metodun hangi nesne üzerinde çalışacağını belirtir. Ve alacağı ilk parametrenin önüne "this" anahtar kelimesi getirilir. Böylece metodun bu nesne üzerinde işlem yapacağı belirtilmiş olur. </li>
<li>Extension metodların kullanımı da çok kolaydır. Extension metodları kullanacağınız kaynak koda, using anahtar kelimesini kullanarak eklediğinizde bu metodlarınızı kullanabilirsiniz.</li>
</ul>
