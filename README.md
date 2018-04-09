# CNN-for-MNIST
---
　
#### 一、概述
```
本程式為使用python語法。用CNN(兩個convolution層與兩個pooling層)來分類MNIST資料集，並使用keras函式庫。
```

#### 二、資料集：
```
手寫辨識(MNIST)
```

#### 三、程式概解
##### 1. Convolution 設置
*第一個convolution：filter數量為 16，size為 5*5，padding為不改變長度與寬度，input為 28x28 的平面圖，激發函數為 relu。*
```
model.add(Conv2D(filters = 16,
                 kernel_size = (5,5),
                 padding = 'same',
                 input_shape = (28 , 28 , 1),
                 activation = 'relu'))
```

##### 2. Pooling 設置
*第一個pooling：pool shape為 2x2*
```
model.add(MaxPool2D(pool_size = (2 , 2)))
```

#### 四、結果
![](https://i.imgur.com/fdHutDt.png)








