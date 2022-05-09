# Diagnosis_Of_Diabetes

Comment lines have been added step by step within the project. (In Turkish Language) Hope it will be a useful study... I decided to publish some of my works in Turkish in this area where Turkish resources are lacking. Therefore, this project will not have a readme file in English.

---
### Şeker Hastalığı Teşhisi Projesi :
  <img algin = "center" src="Diabetes_image.jpeg">

* Proje ile ilgili gerekli bilgiler .ipynb dosyasında yer almaktadır. 
* Proje kapsamında kullanılan algoritma K-Nearest Neighbors algoritmasıdır.

--- 
###  K-Nearest Neighbors Algoritması :

K-En Yakın Komşu Algoritması (veya KNN), hem sınıflandırma hem de regresyon sorunlarını çözebilen popüler bir denetimli makine öğrenimi algoritmasıdır. Algoritma oldukça sezgiseldir ve bir tahminde bulunmak için yeni, etiketlenmemiş bir veri noktasına en yakın k komşuyu bulmak için mesafe ölçümlerini kullanır. 
* Sınıflandırma problemlerinde **In classification problems**, KNN algoritması, k komşusunun çoğunluğunun sınıflarına bakarak sonuca varmaktadır. Yani yeni bir veri noktasının sınıfını çıkarmaya çoğunluğun sınıfına bakarak sonuca varacaktır. Örneğin, yeni bir veri noktasının komşularından beşinin sınıfı "Beyaz" iken yalnızca ikisinin sınıfı "Siyah" ise, algoritma yeni veri noktasının sınıfının "Beyaz" olduğunu tahmin edecektir.
* Regresyon problemlerinde **In regression problems**, KNN algoritması, k komşunun değerlerinin ortalamasını döndürerek yeni bir veri noktasının sürekli değerini tahmin edecektir. Örneğin, en yakın beş komşu [100, 105, 95, 100, 110] değerine sahipse, algoritma bu beş değerin ortalaması olan 102 değerini döndürür.

###  K-Nearest Neighbors Algoritması Neden Öğrenilmeli? :

K-En Yakın Komşu Algoritması, yeni başlayanların öğrenmesi için harika bir makine öğrenimi algoritmasıdır.

KNN algoritmasının öğrenmek için harika olmasının üç sebebine bakalım:

* **1.)** Görselleştirmesi kolay, sezgisel bir algoritmadır. Bu, yeni başlayanlar için öğrenmeyi harika ve teknik olmayan kitlelere açıklamayı kolaylaştırır.
* **2.)** Hem regresyon hem de sınıflandırma problemlerine uygulanabildiği için çok yönlüdür.
* **3.)** Algoritma nispeten küçük veri setleriyle çalışabilir ve oldukça hızlı çalışabilir. 

###  K-Nearest Neighbors Algoritması Nasıl Çalışır? :

K-En Yakın Komşu algoritması, en benzer komşularına bakarak yeni bir veri noktası sınıfı (sınıflandırma durumunda) veya değer (gerileme durumunda) hesaplayarak çalışır ve öyle bir sonuca varır. Hangi veri noktalarının en benzer olduğunu, genellikle  Öklid mesafesi veya Manhattan mesafesi gibi bir mesafe hesaplaması kullanılarak belirlemektedir.

Bir makine öğrenimi uzmanı olarak aşağıdakileri belirlemek sizin işiniz:

* Hangi benzerlik ölçüsünün kullanılacağı...
* Bakılacak komşu sayısı (k)...
* Verilerinizin hangi özellikleri (veya boyutları) en önemli olduğunu belirlemek...

###  K-Nearest Neighbors Algoritmasını Projemde Nasıl Kullanabilirim? :

KNN algoritmasından yararlanmak için popüler Scikit-Learn (sklearn) Modülünün nasıl kullanılacağını bilmeniz gerekir. Başlamak için, bazı kritik modülleride projenizde bulundurmalısınız. (Aynı zamanda o kritik modüllerin kullanımı ile ilgili bilgi sahibi olmanız gerekmektedir.) Keza: pandas, numpy vb... Bu modüller veri bilimi, yapay zeka, makine öğrenmesi, derin öğrenme gibi alanlarda oldukça yaygın bir biçimde kullanılmaktadır.

```console
import pandas as pd #Örnek1, kritik modül
from sklearn.neighbors import KNeighborsClassifier #KNN İmport işlemi
from seaborn import load_dataset #Örnek2, kritik modül
```
---
