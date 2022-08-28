# VeriYapilariveAlgoritmalar
Veri Yapıları ve Algoritmalar dersine ait ödevler için oluşturulmuştur. 

# Proje 3

```
[7,5,1,8,3,6,0,9,4,2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Örnek: root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.
```
1. Aşama
    
    root: 7

    dizideki rakamları soldan sağa doğru ekleyerek şablonumuzu oluşturalım.
    5 rakamı 7' den küçük olduğu için soluna gelecek
                          
                          7
                         /
                        5
2. Aşama
    
    1 rakamı 7 ve 5 rakamlarından küçük o yüzden her ikisinin de solunda yer alacak

                          7
                         /
                        5
                       /
                      1
3. Aşama
   
    8 rakamı 7'den büyük olduğu için sağına yazılır
    
                          7
                         / \
                        5   8
                       /
                      1
4. Aşama

    3 rakamı 1' den büyük olduğu için 1' in sağına yazılır
        
                          7
                         / \
                        5   8
                       /
                      1
                       \
                        3
5. Aşama

    6 rakamı 7'den küçük ama 5' ten büyüktür, bu yüzden 5' in sağına yazılır.
            
                          7
                         / \
                        5   8
                       / \
                      1   6
                       \
                        3
6. Aşama

    0 rakamı 1' den küçüktür soluna yazılır
                
                          7
                         / \
                        5   8
                       / \
                      1   6
                     / \
                    0   3
7. Aşama

    9 rakamı 7 ve 8 den büyüktür, her ikisinin de sağında yer alır
                    
                          7
                         / \
                        5   8
                       / \   \
                      1   6   9
                     / \
                    0   3
8. Aşama

    4 rakamı 7 ve 5' ten küçük olduğu için bu rakamların solunda 1 ve 3' ten büyük olduğu için bu rakamların sağında yer alır.
                        
                          7
                         / \
                        5   8
                       / \   \
                      1   6   9
                     / \
                    0   3
                         \
                          4
9. Aşama

    2 rakamı 7 ve 5' ten küçük olduğu için bu rakamların solunda 1' den büyük olduğu için 1' in sağında ve 3' ten küçük olduğu için 3' ün solunda yer alır.
                        
                          7
                         / \
                        5   8
                       / \   \
                      1   6   9
                     / \
                    0   3
                       / \
                      2   4
                      