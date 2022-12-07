# location_clustering
用户地理位置的聚类算法实现—基于DBSCAN和Kmeans的混合算法

https://blog.csdn.net/jackaduma/article/details/52734731

![静态代码检查首页](https://github.com/jackaduma/location_clustering/blob/master/a.jpg)



python2.7 -> python3 修改修改部分代码
```bash
Examples
--------
>>> from numpy import array
>>> from scipy.cluster.vq import vq, kmeans2, whiten
>>> import matplotlib.pyplot as plt
>>> features  = array([[ 1.9,2.3],
...                    [ 1.5,2.5],
...                    [ 0.8,0.6],
...                    [ 0.4,1.8],
...                    [ 0.1,0.1],
...                    [ 0.2,1.8],
...                    [ 2.0,0.5],
...                    [ 0.3,1.5],
...                    [ 1.0,1.0]])
>>> whitened = whiten(features)
>>> book = np.array((whitened[0],whitened[2]))
>>> kmeans2(whitened,book)
(array([[ 2.3110306 ,  2.86287398],    # random
       [ 0.93218041,  1.24398691]]), 0.85684700941625547)

>>> codes = 3
>>> kmeans2(whitened,codes)
(array([[ 2.3110306 ,  2.86287398],    # random
       [ 1.32544402,  0.65607529],
       [ 0.40782893,  2.02786907]]), 0.5196582527686241)
```


