---
title: 機器學習面試題目
description: 機器學習面試被問到的題目
date: 2023-09-22
image: 2.jpg
categories:
    - 機器學習
    - 題目
tags:
    - 題目
---

#  

## 結果
* 職務類別:機器識別研發工程師
* 2 hours
* 很多都回答不出來硬回答
* 在面試前要多複習，不要都只會用
* leetcode 1*easy 1*Medium

### 1.Batch Normalization 和一般 Normalization 差別
* Google 於 2015 年提出了 Batch Normalization 的方法，和輸入數據先做 feature scaling 再進行網路訓練的方法類似。在輸入數據時，通常都會先將 feature 做 normalize 後再進行訓練，可以加速模型收斂；而 Batch Normalization 就是指在每一層輸入都做一次 normalize

* Batch Normalization 的作法就是對每一個 mini-batch 都進行正規化到平均值為0、標準差為1的常態分佈，如此一來可以將分散的數據統一，有助於減緩梯度消失以及解決 Internal Covariate Shift 的問題，同時可以加速收斂，並且有正則化的效果 (可以不使用Dropout)

* 多的請參考：https://medium.com/ching-i/batch-normalization-%E4%BB%8B%E7%B4%B9-135a24928f12

### 2.BatchNormalization与LayerNormalization的區別

* Batch Normalization 的處理對像是對一批樣本， Layer Normalization 的處理對像是單一樣本。 Batch Normalization 是對這批樣本的同一維度特徵做歸一化， Layer Normalization 是對這單一樣本的所有維度特徵做歸一化。

### 3.Optimizer 在影像上和NLP上使用的差別

* https://medium.com/programming-with-data/34-%E8%AA%BF%E5%8F%83%E7%89%88bert%E6%87%89%E7%94%A8%E7%AF%84%E4%BE%8B-328f56308e64

### 4.selfAttention 為什麼要除一個Scale

* https://zhuanlan.zhihu.com/p/503321685

### 5.Activation function(沒問但我不小心答非所問，還講錯)

* https://medium.com/%E6%B7%B1%E6%80%9D%E5%BF%83%E6%80%9D/ml08-activation-function-%E6%98%AF%E4%BB%80%E9%BA%BC-15ec78fa1ce4


### 6.影像 segmentation 

* https://medium.com/ching-i/%E5%BD%B1%E5%83%8F%E5%88%86%E5%89%B2-image-segmentation-%E8%AA%9E%E7%BE%A9%E5%88%86%E5%89%B2-semantic-segmentation-1-53a1dde9ed92

### 7.梯度消失梯度爆炸

* https://zhuanlan.zhihu.com/p/33006526

### 8.梯度消失梯度不只在RNN會發生

* https://ithelp.ithome.com.tw/m/articles/10280019

### 9. LayerNormalization 通常放在哪裡 為什麼

* https://hackmd.io/@CZ-Chuang/BJ39oZnvD