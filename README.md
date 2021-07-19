# sklearn_for_psychology

本文包括两个ridge L2 regression model
主要难点在于报告p值与mse，因为机器学习不太关注p值，因此调用了statsmodels包来解决该问题。
此外，本文使用了seaborn包绘制预测图。

首先，通过kfold函数准备cross validation
然后，使用sklearn包中的linear_model建立回归模型，并返回了p值,r值与mse值----这一切封装在get_rs函数中。
此外，main函数将结果转化为更容易观看的dataframe格式
最后，进行了绘图，并保存图片。

此文的目的在于提供一个参考模板，以便不熟悉sklearn模块的同学使用。因此，其中的参数与函数是非常方便大家自定义的。
注意，本文并没有解决permutation test如何运行的问题。
