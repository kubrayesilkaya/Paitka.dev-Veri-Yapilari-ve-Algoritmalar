## MERGE SORT
### [16,21,11,8,12,22] 

Merge sort algoritmasında dizi, en küçük birimlerine kadar bölünür ve ardından karşılaştırmalar yaparak sıralanır. Selection sort algoritması ile karşılaştırıldığında, 
çok daha hızlı ve performanslı bir yaklaşımdır; çünkü bir elemanın dizideki yerini bulmak için selection sort algoritmasındaki gibi tüm diziyi taramak gerekmez; 
kontrol edilmesi gereken eleman sayısını azaltan bir yaklaşmdır.

Örnekteki dizi için merge sort algoritmasının uygulanmasına bakalım :

İlk olarak dizi iki parçaya ayrılır : 

[16, 21, 11] ve [8, 12, 22]

Her bir bölünen parça için en küçük birime kadar tekrar bölme işlemi uygulanır :

[16, 21, 11] :
  [16] | [21, 11] :
     [16] | [21] | [11]
 
[8, 12, 22] :
  [8] | [12, 22] :
    [8] | [12] | [22]
