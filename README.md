# Pytorch环境下实现一些推荐系统算法

## 数据来源
RecBole里处理好的ml-100k数据

## 1. MF(Matrix Factorication)矩阵分解算法
参考文献：Matrix Factorization Techniques for Recommender Systems  
1.MF_base.ipynb：完全手动借助SGD实现MF算法，时间性能较差  
2.MF_improve.ipynb：首先，尽量借助Pytorch中的已有库，比如optim等等；其次，采用分批batch的方式，改进时间性能；最后，尽可能减少对df文件以及评分矩阵的遍历，优化时间性能
