## MERGE SORT
### [16,21,11,8,12,22] 

Merge Sort algoritmasında dizi, en küçük birimlerine kadar bölünür ve ardından karşılaştırmalar yaparak sıralanır. Selection sort algoritması ile karşılaştırıldığında, çok daha hızlı ve performanslı bir yaklaşımdır; çünkü bir elemanın dizideki yerini bulmak için selection sort algoritmasındaki gibi tüm diziyi taramak gerekmez; kontrol edilmesi gereken eleman sayısını azaltan bir yaklaşmdır.

Örnekteki dizi için merge sort algoritmasının uygulanmasına bakalım :

İlk olarak dizi iki parçaya ayrılır : 

[16, 21, 11] ve [8, 12, 22]

Her bir bölünen parça için en küçük birime kadar tekrar bölme işlemi uygulanır :

- [16, 21, 11] :

  - [16] | [21, 11] :
  
     - [16] | [21] | [11]
 
- [8, 12, 22] :

  - [8] | [12, 22] :
  
    - [8] | [12] | [22]
   
Dizi en küçük birimlerine ayrıldıktan sonra elemanları karşılaştırarak tekrar sıralama aşamasına geçilir. Merge Sort algoritmasındaki, selection sort algortimasına
kıyas ile çok daha az sayıda sorgu yaparak dizimizi sıralayabiliyoruz. Küçük birimlere ayırdığımız diziyi, alt birimlerinden itibaren sıralamamız nedeni ile, birimleri kendi arasında karşılaştırırken sıralamaları göz önüne alarak daha az sorguya ihtiyaç duyarız.

  - [16] | [21] | [11] ->  [16] | [11, 21] -> [11] | [16] | [21]  

  - [8] | [12] | [22] ->   [8] | [12, 22]  -> [8] | [12] | [22]

  - [11] | [16] | [21] , [8] | [12] | [22] -> [8, 11, 12, 16, 21, 22]

### Big-O Notation

Merge Sort algoritmasında diziyi küçük parçalara böler iken her adımda iki parçaya ayırarak ilerlememizden dolayı, bölme aşamasında Big-O değeri  2^x = n -> x = log2n => O(logn) olarak hesaplanır. Parçalama aşamasından sonra sırala aşamasında ise, her adımda n eleman üzerinde işlem yapılır. Her işlemden gelen O(n) time complexity değeri ile, merge sort algoritmasını **Big-O değeri O(nlogn)** 'dir.



  
