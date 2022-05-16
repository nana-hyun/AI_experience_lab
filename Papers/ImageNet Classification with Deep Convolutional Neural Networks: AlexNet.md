# Abstract

* ImageNet LSVRC-2010 contest
    * classify 1.2 million high-resolution images into 1000 diferent class
    * error rate
        * top 1, top 5 : 37.5 %, 17.0 %
* ILSVRC-2012 contest
    * error rate
        * top 5 : 15.3%
---
what is top 1, top 5 error rate?

mnist 데이터를 가지고 생각해보자.

0|1|2|3|4|5|6|7|8|9|
--|--|--|--|--|--|--|--|--|--
0.1|0.5|0.16|0.05|0.05|0.03|0.02|0.01|0.04|0.04

가장 높은 확률을 가지는 1이 top-1 class가 된다.

top-5 class는 0,1,2,3,4 가 된다.

* 만일 true 값이 1이라면 top-1 error : 0%
* 만일 true 값이 top-5 class 중 (1이 아닌) 하나라면 top-5 error : 0%

---
* 60 million parameters and 650,000 neurons
* 5 convolution layers (some - followed by max-pooling layers)
* 3 fully-connected layers : 1000-way softmax

to make training faster
* non-saturating neurons
* very efficient GPU implementation of the convolution operation

to reduce overfitting in fully-connected layers
* regularization : "dropout"


# I. Introduction
