# Binary Search Tree Projesi

1. [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary Search Tree aşamalarının yazılması.

* Öncelikle bir root belirlenir. Daha sonra diğer elemanlar içerisinden roottan küçük olanlar rootun soluna, büyük olanlar ise sağına yazılır ve tree bu şekilde devam eder.

* Root elemanımız '6' olsun. Dizinin ilk elemanı olan 7, 6'dan büyük olduğu için 6(root)'nın sağ tarafına, dizinin ikinci elemanı olan 5, 6'dan küçük olduğu için 6'nın sol tarafına yazılmalıdır.
```
                                6
                               / \
                              5   7   1. Düğüm satırı
```
* Dizinin üçüncü elemanı olan 1, 6'dan da 5'ten de küçük olduğu için 5'in sol tarafına yazılır.
```
                                6        Root Satırı
                               / \
                              5   7      1. Düğüm satırı
                             /
                            1
```
* Dizinin dördüncü elemanı olan 8, 6'dan da 7'den de büyük olduğu için 7'nin sol tarafına yazılır.
 ```
                                6       Root Satırı
                               / \
                              5   7     1. Düğüm satırı
                             /     \
                            1       8   2. Düğüm Satırı
```
* Dizinin beşinci elemanı olan 3, 6 ve 5'ten küçük fakat 1'den büyüktür. Bu sebeple 1'in sağ tarafına yazılır.
 ```
                                6       Root Satırı
                               / \
                              5   7     1. Düğüm satırı
                             /     \
                            1       8   2. Düğüm Satırı
                             \
                              3
```
* Dizinin altıncı elemanı olan 6 root olduğundan yedinci elemana bakıyoruz. Dizinin yedinci elemanı olan 0; 6'dan, 5'ten ve 1'den küçüktür. Bu sebeple 1'in solunda yer alır.
 ```
                                6       Root Satırı
                               / \
                              5   7     1. Düğüm satırı
                             /     \
                            1       8   2. Düğüm Satırı
                           / \
                          0   3    
```
* Dizinin sekizinci elemanı olan 9; 6'dan, 7'den ve 8'den büyüktür. Bu sebeple 8'in sağına yazılır.
```
                                6           Root Satırı
                               / \
                              5   7         1. Düğüm satırı
                             /     \
                            1       8       2. Düğüm Satırı
                           / \       \
                          0   3       9     3. Düğüm Satırı
```
* Dizimizin dokuzuncu elemanı 4, 6'dan ve 5'ten küçük fakat 1'den ve 3'ten büyük olduğu için 3'ün sağ tarafına konumlanır.
 ```
                                6           Root Satırı
                               / \
                              5   7         1. Düğüm satırı
                             /     \
                            1       8       2. Düğüm Satırı
                           / \       \
                          0   3       9     3. Düğüm Satırı
                               \
                                4
```
* Dizimin onuncu ve son elemanı olan 2, 6'dan ve 5'ten küçük fakat 1'den büyük olduğu için 1'in sağında yer almalıdır. 1'in sağında 3 olduğu için ve 2, 3'ten küçük olduğu için 3'ün solunda yer alır.
 ```
                                6           Root Satırı
                               / \
                              5   7         1. Düğüm satırı
                             /     \
                            1       8       2. Düğüm Satırı
                           / \       \
                          0   3       9     3. Düğüm Satırı
                             / \
                            2   4           4. Düğüm Satırı
```


