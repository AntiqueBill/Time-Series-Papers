# Awesome Time Series Papers

- Introduction:
    - List of awesome papers from various research fields in time series analysis, mainly including algorithms based on machine learning. 
    - `*` after the title of the paper indicates that the full paper has been carefully read by [me](https://github.com/bighuang624).
    - A link of open source code is given if avaliable on [Papers With Code](https://paperswithcode.com/) or [Github](https://github.com/).
    - Any [contributions](https://github.com/bighuang624/Time-Series-Papers/blob/master/.github/contribution_template.md) including PR are welcomed.

- 介绍：
    - 收录时间序列分析中各个研究领域的高水平文章，主要包含基于机器学习的算法。
    - 论文标题后的`*`号表示[我](https://github.com/bighuang624)仔细地读过全文。
    - 如果 [Papers With Code](https://paperswithcode.com/) 或 [Github](https://github.com/) 上存在该论文的开源代码，则给出其链接。
    - 欢迎包括 PR 在内的一切[贡献](https://github.com/bighuang624/Time-Series-Papers/blob/master/.github/contribution_template.md)。

- - -

## Catelog (目录)

- [Awesome Time Series Papers](#awesome-time-series-papers)
    - [Time Series Forecasting (时间序列预测)](#time-series-forecasting-时间序列预测)
    - [Time Series Classification (时间序列分类)](#time-series-classification-时间序列分类) 
    - [Time Series Clustering (时间序列聚类)](#time-series-clustering-时间序列聚类)
    - [Anomaly Detection (异常检测)](#anomaly-detection-异常检测) 
    - [Sequence Modeling (序列建模)](#sequence-modeling-序列建模)

- - -

## Time Series Forecasting (时间序列预测)

Time series forecasting is the task of predicting future values of a time series (as well as uncertainty bounds).

<!--### Multivariate-->

#### 2018

- **Modeling Long- and Short-Term Temporal Patterns with Deep Neural Network** (**SIGIR18**) [[paper](https://arxiv.org/pdf/1703.07015v3.pdf)] [[code](https://paperswithcode.com/paper/modeling-long-and-short-term-temporal)] *
    - Propose LSTNet, which contains a recurrent-skip layer or a temporal attention layer to capture a mixture of short-term and long-term repeating patterns
    - 提出 LSTNet，使用 recurrent-skip layer 或 temporal attention layer 来建模短期和长期重复模式的混合

- **A Memory-Network Based Solution for Multivariate Time-Series Forecasting** [[paper](https://arxiv.org/pdf/1809.02105v1.pdf)] [[code](https://github.com/Maple728/MTNet)] *
    - Propose MTNet, which uses a memory component and attention mechanism to store the long-term historical data and deal with a period of time rather than a single time step
    - 提出 MTNet，使用一个记忆模块和注意力机制来存储长期的历史数据，并且可以同时处理一段序列而非单独的时间步

- **Temporal Pattern Attention for Multivariate Time Series Forecasting** [[paper](https://arxiv.org/pdf/1809.04206v2.pdf)] [[code](https://github.com/gantheory/TPA-LSTM)] *
    - Propose Temporal Pattern Attention, which learns to select not only time steps but also series relevant to the prediction
    - 提出 Temporal Pattern Attention，不仅能够选择与预测相关的时间步，还能够考虑到不同变量的影响

#### 2017

- **A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction** (**IJCAI17**) [[paper](https://arxiv.org/pdf/1704.02971v4.pdf)] [[code](https://paperswithcode.com/paper/a-dual-stage-attention-based-recurrent-neural)] *
    - Propose DA-RNN, which consists of an encoder with an input attention mechanism to select relevant driving series, and a decoder with a temporal attention mechanism to capture long-range temporal information of the encoded inputs
    - 提出 DA-RNN，其包含一个带有 input attention 机制的编码器来选择相关外部序列，和一个带有 temporal attention 机制的解码器来捕获已编码输入中的长期时间信息

- - -

## Time Series Classification (时间序列分类)

Time series forecasting is the task of assigning time series pattern to a specific category.

#### 2018

- **Towards a Universal Neural Network Encoder for Time Series** [[paper](https://arxiv.org/pdf/1805.03908.pdf)] *
    - Study the use of a time series encoder to learn representations that are useful on data set types with which it has not been trained on
    - 研究时序编码器的使用，来学习对其未接触过的数据集类型有用的表示

- **Transfer learning for time series classification** (**IEEE Big Data 2018**) [[paper](https://arxiv.org/pdf/1811.01533.pdf)] [[code](https://github.com/hfawaz/bigdata18)] *
    - Extensive experiments show that transferring the network's weights works on time series classification task, and the choice of the source dataset impacts significantly on the model's generalization capabilities
    - 使用大量实验表明，模型权值的迁移促进其在目标数据集上分类任务的表现，且源数据集的选择对模型的泛化能力有显著影响

- - -

## Time Series Clustering (时间序列聚类)

Time series clustering is the task of forming clusters given a set of unlabeled time series data.

#### 2018

- **Deep Temporal Clustering: Fully Unsupervised Learning of Time-Domain Features** (**ICLR18**) [[paper](https://arxiv.org/pdf/1802.01059.pdf)] [[code](https://github.com/saeeeeru/dtc-tensorflow)] *
    - Integrate dimensionality reduction and temporal clustering into a single end-to-end learning framework to jointly optimize
    - 将降维和时序聚类集成到一个端到端神经网络，以进行联合优化

#### 2016

- **Unsupervised Feature Learning from Time Series** (**IJCAI16**) [[paper](https://pdfs.semanticscholar.org/b4f5/8e005541c54b146e67b09094f09ba3297906.pdf)]
    - Present a new Unsupervised Shapelet Learning Model (USLM) to learn shapelets, which combines pseudo-class label, spectral analysis, shapelets regularization and regularized least-squares for learning (shapelets are time series short segments that can best predict class labels)
    - 给出一个结合了伪类标签、谱分析、shapelets 正则化和正则化最小二乘法的无监督 Shapelet 学习模型（shapelets 是时间序列的短片段，能够最好地预测类标签）

- - -

## Anomaly Detection (异常检测)

Anomaly detection is the task of identifying rare items, events or observations which raise suspicions by differing significantly from the majority of the data.

#### 2019

- **A Deep Neural Network for Unsupervised Anomaly Detection and Diagnosis in Multivariate Time Series Data** (**AAAI19**) [[paper](https://arxiv.org/pdf/1811.08055.pdf)]
    - Propose a Multi-Scale Convolutional Recurrent Encoder-Decoder (MSCRED), to perform anomaly detection and diagnosis in multivariate time series data
    - 提出了一种多尺度卷积循环编码器-解码器（MSCRED），对多变量时间序列数据进行异常检测和诊断

- - -

## Sequence Modeling (序列建模)

Specially designed sequence modeling methods can be applied to time series data and solve many problems, e.g. forecasting and classification.

#### 2018

- **An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling** [[paper](https://arxiv.org/pdf/1803.01271v2.pdf)] [[code](https://paperswithcode.com/paper/an-empirical-evaluation-of-generic)]
    - Describe a temporal convolutional network (TCN), which contains causal convolutions, dilated convolutions and residual connections
    - 描述了时间卷积网络（TCN），其包含有因果卷积、扩张卷积和残差连接

- - -

<!-- ## Spatio-temporal Forecasting (时空预测)

- - -

## Stock Market Prediction (股票市场预测)

- - -

## Traffic Prediction (交通预测)

- - --->

