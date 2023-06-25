#### [22,27,16,2,18,6] SELECTION SORT

Selection sort algoritmasında, dizideki en küçük elemanı bularak bu sayı ile dizinin başındaki elemanı yer değiştirerek dizimizi sıralarız ve dizimiz küçükten büyüğe sıralanmış olur.
Big O değeri O(n^2) olmaıs nedeni ile quick sort ve merge sort algoritmaları ile karşılaştırıldığında daha düşük bir performansa sahiptir.

Şimdi örnekteki dizi için adım adım selection sort algoritmaısnı uygulayalım:

 **[22, 27, 16, 2, 18, 6]** | Big-O = O(n) 
 
 Dizideki en küçük elemanı bulmak için dizinin tamamı taranır ve en küçük değer olan 2 bulunur. 2 ile diznin başındaki 22 değeri yer değiştirir :

 **[2, 27, 16, 22, 18, 6]** | Big-O = O(n-1)

 Algoritma aynı şekilde devam eder ve sıralanan dizide 1.indexdeki sayı olan 27 ile, dizinin kalan kısmı tarandığında bulunan en küçük sayı yer değiştirir :

 **[2, 6, 16, 22, 18, 27** | Big-O = O(n-2) 

 Dizinin sıralanmış son hali : **[2, 6, 16, 18, 22, 27]** | Big O = O(1)

#### Big - O Notation 

 Big-O değeri = n+ (n-1) + (n-2) + ... + 1 = (n*(n+1)) /2 hesaplaması ile **O(n^2**) olarak bulunur.

 
