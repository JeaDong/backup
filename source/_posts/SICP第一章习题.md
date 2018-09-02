---
title: SICP第一章习题
date: 2018-09-05 19:24:28
tags: SICP
---
*终于要开始啃这本极其讨厌的书了！！！*  
*没办法，毕竟很多大佬都推荐，要达到他们的水平，拿上他们那种工资，就应该好好啃。诸君，加油～*
<!-- more -->
#### 1.1
没啥难度，直接贴答案
```
1 ]=> (define a 3)

;Value: a

1 ]=> (define b (+ a 1))

;Value: b

1 ]=> b

;Value: 4

1 ]=> (+ a b (* a b))

;Value: 19

1 ]=> (= a b)

;Value: #f

1 ]=> ( if (and (> b a) (< b (* a b))) b a)

;Value: 4

1 ]=> a

;Value: 3

1 ]=> ( cond ((= a 4) a) ((= b 4) (+ 6 7 a)) (else 25))

;Value: 16

1 ]=> (+ 2 (if (> b a) b a))

;Value: 6

1 ]=> (* (cond ((> a b) a) ((> b a) b) (else -1))
(+ a 1))

;Value: 16

1 ]=> (/ 4 5)

;Value: 4/5
```

#### 1.2
没啥好说，拆分！！！
```
1 ]=> (/ (+ 5 4 (- 2 (- 3 (+ 6 (/ 4 5))))) (* 3 (- 6 2) (- 2 7)))

;Value: -37/150
```

#### 1.3

```
1 ]=> (define (sum a b c) (cond ((and (<= a b ) (<= a c )) (+ b c )) ((and (<= b a) (<= b c)) (+ a c)) (( and (<= c a) (<= c b)) (+ a b))))
```

#### 1.4

```
if b > 0 then (+ a b)
else (- a b)
```

#### 1.5
完全没有看懂题意在说啥～～～  
后续好好理解一下