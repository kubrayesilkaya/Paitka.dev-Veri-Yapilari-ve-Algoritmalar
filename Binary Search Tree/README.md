## BINARY SEACRH TREE
### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

Binary Search Tree veri yapısı node(düğüm)'lardan oluşur ve her bir düğümün sağ alt kısmındaki her bir child node, mevcut node'dan büyük değere sahiptir; 
sol alt kısmındaki her bir child node ise mevcut node'dan küçük değere sahiptir.

Örnek dizi için binary search tree aşamaları :

- İlk eleman olan 7 düğümü, binary search ağacnın kök (root) düğümüdür. 
  - **root = 7**

- İkinci eleman olan 5 ; root değerinden küçük bir değer olması nedeni ile, ağaçta sol alt düğüme (sol child node) yerleşir.

  ```
            7
           /
          5
   ```
   
- Üçüncü eleman olan 1 ; 5 değerinden küçük bir değer olması nedeni ile, 5 düğümünün sol alt düğümüne (sol child node) yerleşir.
    ```
            7
           /
          5
         /
        1
   ```
- 8 değeri ; root değerinden büyük bir değer olması nedeni ile, root değeri olan 7'nin sağ alt düğümüne (sağ chil node) yerleşir.
   ```
            7
           / \
          5   8
         /
        1
   ```
- 3 değeri 1'den büyük; 5'den küçük bir değer olması nedeni ile, 1'in sağ alt düğümüne yerleşir.
    ```
             7  
            / \
           5   8
          /    
         1      
          \   
           3           
   ```
- 6 değeri 5'den büyük; 7'den küçük bir değer olması nedeni ile 5'in sağ child düğümü olur.
  
   ```
             7  
            / \
           5   8
          / \   
         1   6    
          \   
           3
   ```
- 0 değeri 1'den küçük olması nedeni ile 1'in sol child düğümü olur.
     
   ```
             7  
            / \
           5   8
          / \   
         1   6    
        / \   
       0   3 
   ```

- 9 değeri, 7 olan root değerinden ve 8 değerinden büyük olması nedeni ile 8'in sağ alt düğümü olur.

    ```
             7  
            / \
           5   8
          / \   \
         1   6   9 
        / \   
       0   3
   ```
- 4 değeri, 3'den büyük; 5'den küçük olması nedeni ile 3 düğümünün sağ alt düğümü olur.
     ```
             7  
            / \
           5   8
          / \   \
         1   6   9 
        / \   
       0   3  
            \
             4   
      
   ```
- 2 değeri, 1 değerinden büyük; 3 değerinden büyük olması nedeni ile 3 düğümünün sol alt düğümü olur.
  ```
             7  
            / \
           5   8
          / \   \
         1   6   9 
        / \   
       0   3  
          / \
         2   4 
   ```
   
**Aşamaların sonunda Binary Tree Ağacımızın son hali :**
```
             7  
            / \
           5   8
          / \   \
         1   6   9 
        / \   
       0   3  
          / \
         2   4
   ```

  
