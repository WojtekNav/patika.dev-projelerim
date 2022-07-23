# patika.dev-projelerim
www.patika.dev
"""""
Proje 1
[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.
Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.


[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
"""
[22,27,16,2,18,6]
#Aşama1 --> 22 ve 27 kontrol edildi sıralı olduğundan değişim yok
[22,22,27,2,18,6] key:16
[16,22,27,2,18,6]
#Aşama2--> 16 ya gelindikten sonra önce 27 yerine geçti daha sonra 22 ile kontrolü sağlanıp listenin başına alındı
[16,16,22,27,18,6] key:2
[2,16,22,27,18,6]
#Aşama3--> 2 Sayısı görüldükten sonra tekrar geriye doğru tek tek büyüklük kontrolü yapılarak 2 listenin en başına alındı
[2,16,22,22,27,6] key:18
[2,16,18,22,27,6]
#Aşama 4 ---> 18 Sayısına gelindikten sonra geriye dönük tekrar büyüklük kontrolü yapılarak 22 sayısı ötelendi.
[2,16,16,18,22,27] key:6
[2,6,16,18,22,27]
#Aşama 5 ---> 6 Sayısı geriye dönük kontrolle 2 sayısının önüne getirildi.


#O(n)
#Avarage Case: O(n**2)
#Worst Case:O(n**2)
#Best Case:O(n)
#Dizi sıralandıktan sonra 18 sayısı Avarage Case olacaktır.

[7,3,5,8,2,9,4,15,6]
[7,7,5,8,2,9,4,15,6] key:3
[3,7,5,8,2,9,4,15,6]
# Aşama1 --> 7 ve 3 sayılarının değiştirilmesiyle başlar
[3,7,7,8,2,9,4,15,6] key:5
[3,5,7,8,2,9,4,15,6]
#Aşama2 --> 7 ve 5 sayıları yer değiştirilir.
[3,5,7,8,2,9,4,15,6]
#Aşama3 --> 7 ve 8 sıralaması normal olduğundan bir sonraki sıraya geçilir.
[3,5,7,8,2,9,4,15,6]
[3,5,7,8,8,9,4,15,6] key:2
[2,3,5,7,8,9,4,15,6]
#Aşama4 --> 2 key değeri listenin en başına ötelenir.
