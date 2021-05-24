# Pytorch环境下实现一些推荐系统算法

## 数据来源
RecBole里处理好的ml-100k数据

## 1. MF(Matrix Factorication)矩阵分解算法
参考文献：Matrix Factorization Techniques for Recommender Systems  
1.MF_base.ipynb：完全手动借助SGD实现MF算法，时间性能较差  
2.MF_improve.ipynb：首先，尽量借助Pytorch中的已有库，比如optim等等；其次，采用分批batch的方式，改进时间性能；最后，尽可能减少对df文件以及评分矩阵的遍历，优化时间性能  
MF_notes.pdf：阅读论文的笔记  
MF_papar.pdf：原文加备注  

## 2. BPR(Bayesian Personalized Rankin)贝叶斯个性化排名算法
参考文献：BPR: Bayesian Personalized Ranking from Implicit Feedback  
1.BPR_base.ipynb：完全手动借助SGD实现BPR算法，只使用了50个user和50个item的数据  
2.BPR_tensorflow.ipynb：运行了博客园中的一份tensorflow版本代码  
3.BPR_improve.ipynb：首先，尽量借助Pytorch中的已有库，比如optim等等；其次，采用分批batch的方式，改进时间性能；最后，采用多次采样的方式，不然三元组数目巨大  
BPR_notes1.pdf：阅读论文的笔记  
BPR_notes2.pdf：找的一篇博客总结  
BPR_papar.pdf：原文加备注
