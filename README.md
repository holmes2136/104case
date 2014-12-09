104case
=======

What is bloom filter
=======
Bloom filter 為判斷某一元素是否在集合中 , 而 Bloom filter 可以用比 hash 更少的空間
完成同樣的問題 , 其中元素越多，誤報率越大，但是漏報是不可能的。

Demo Code 所使用的 bloom filter 可參考
[Github](https://github.com/jasondavies/bloomfilter.js)

What inspire me 
=======
104 人力網站或 518 租屋網都會有儲存工作物件或者房屋物件的功能 , 若儲存了相同的物件
則應會提示 : 你已經儲存了相同的東西 , 不過看起來 104 似乎沒有提示..然而去檢查
user 是否已經儲存了相同的物件而再去 db 搜尋似乎不是很必要的事情 , 因此可以
在頁面初始時便把所有已儲存物件初始化到 bloom filter , 這樣子就可以很輕鬆的檢查物件
是否存在了


Demo sample
=======
示範了使用 bloom filter 來判斷案件是否存在與否


