# 使用K-Means(K-均值)算法给20支亚洲球队做聚类


## K-Means的工作原理给亚洲球队做聚类步骤
工作原理
- step1：选取K个点作为初始的中心点。
- Step2：将每个点分配到最近的类中心点，然后重新计算每个类的中心点。
- Step3: 重复Step2，直到类不发生变化，或者达到最大的迭代次数为止。



## 使用sklearn中的K-Means算法
- sklearn_cluster提供了9种聚类的方法
- 引用：from sklearn.cluster import KMeans
- 创建KMeans()
    - n_cluster:K值
    - max_iter：最大的迭代次数
    - n_init：初始化中心点的运算次数
    - init：初始值选择的方式，默认是k-means++的方式
    - algorithm：kmeans的实现算法，默认是auto
- 功能调用
    - fit(data):对data数据进行K-Means聚类
    - predict(data):针对data中的每个样本，计算最近的类

## 总结
- K—Means和KNN的区别
    - 分类or聚类：K—Means是聚类，KNN是分类
    - 监督学习or非监督学习：K-Means非监督学习，KNN监督学习
    - K值含义：K-Means中代表K类，KNN中代表K个最接近的邻居