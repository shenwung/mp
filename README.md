# mp(Micro Payment)

## 客戶交易資料行為預測
+ train data: 2015/07 ~ 2015/10
+ test data:  2016/03 ~ 2015/06
+ 客戶164個屬性(4個月) = 164 * 4 = 656

```
1. DNN: dnn_mp.ipynb
   data shape: (None, 656)
   # 後續加上3個變數(NES), 每個變數16週(16個時間點), 3 * 16 = 48 => 656 + 48 = 704
   data shape after add nes vars: (None, 704)
   
2. CNN: cnn_mp.ipynb
   data shape: (None, 164, 4)
   # 後續加上3個變數(NES), 每個變數4個月(4個時間點)
   data shape after add nes vars: (None, 167, 4)
```
