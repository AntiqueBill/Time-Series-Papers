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
  - [Catelog (目录)](#catelog-%E7%9B%AE%E5%BD%95)
  - [Time Series Forecasting (时间序列预测)](#time-series-forecasting-%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E9%A2%84%E6%B5%8B)
    - [Univariate (单变量)](#univariate-%E5%8D%95%E5%8F%98%E9%87%8F)
    - [Multivariate to Univariate (多变量预测单变量)](#multivariate-to-univariate-%E5%A4%9A%E5%8F%98%E9%87%8F%E9%A2%84%E6%B5%8B%E5%8D%95%E5%8F%98%E9%87%8F)
      - [2017](#2017)
    - [Multivariate to Multivariate (多变量预测多变量)](#multivariate-to-multivariate-%E5%A4%9A%E5%8F%98%E9%87%8F%E9%A2%84%E6%B5%8B%E5%A4%9A%E5%8F%98%E9%87%8F)
      - [2018](#2018)
  - [Time Series Classification (时间序列分类)](#time-series-classification-%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E5%88%86%E7%B1%BB)
      - [2018](#2018-1)
      - [2017](#2017-1)
  - [Time Series Clustering (时间序列聚类)](#time-series-clustering-%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E8%81%9A%E7%B1%BB)
      - [2019](#2019)
      - [2018](#2018-2)
      - [2016](#2016)
  - [Anomaly Detection (异常检测)](#anomaly-detection-%E5%BC%82%E5%B8%B8%E6%A3%80%E6%B5%8B)
      - [2019](#2019-1)
  - [Sequence Modeling (序列建模)](#sequence-modeling-%E5%BA%8F%E5%88%97%E5%BB%BA%E6%A8%A1)
    - [Supervised Sequence Modeling (监督序列建模)](#supervised-sequence-modeling-%E7%9B%91%E7%9D%A3%E5%BA%8F%E5%88%97%E5%BB%BA%E6%A8%A1)
      - [2018](#2018-3)
    - [Unsupervised Representation Learning (无监督表示学习)](#unsupervised-representation-learning-%E6%97%A0%E7%9B%91%E7%9D%A3%E8%A1%A8%E7%A4%BA%E5%AD%A6%E4%B9%A0)
      - [2019](#2019-2)
  - [Time Series Segmentation (时间序列分割)](#time-series-segmentation-%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E5%88%86%E5%89%B2)
  - [Study of Stock Market (股票市场研究)](#study-of-stock-market-%E8%82%A1%E7%A5%A8%E5%B8%82%E5%9C%BA%E7%A0%94%E7%A9%B6)
      - [2017](#2017-2)
  - [Others (其他)](#others-%E5%85%B6%E4%BB%96)
      - [2019](#2019-3)
      - [2018](#2018-4)

- - -

## Time Series Forecasting (时间序列预测)

Time series forecasting is the task of predicting future values of a time series (as well as uncertainty bounds).

### Univariate (单变量)

### Multivariate to Univariate (多变量预测单变量)

The model predicts the current value of **a time series** based upon its previous values as well as the current and past values of multiple driving (exogenous) series.

#### 2017

- **A Dual-Stage Attention-Based Recurrent Neural Network for Time Series Prediction** (**IJCAI17**) [[paper](https://arxiv.org/pdf/1704.02971v4.pdf)] [[code](https://paperswithcode.com/paper/a-dual-stage-attention-based-recurrent-neural)] *
    - Propose DA-RNN, which consists of an encoder with an input attention mechanism to select relevant driving series, and a decoder with a temporal attention mechanism to capture long-range temporal information of the encoded inputs
    - 提出 DA-RNN，其包含一个带有 input attention 机制的编码器来选择相关外部序列，和一个带有 temporal attention 机制的解码器来捕获已编码输入中的长期时间信息


### Multivariate to Multivariate (多变量预测多变量)

The models predicts the future values of **multivariate time series** only based upon their previous values.

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

- - -

## Time Series Classification (时间序列分类)

Time series forecasting is the task of assigning time series pattern to a specific category.

#### 2018

- **Towards a Universal Neural Network Encoder for Time Series** [[paper](https://arxiv.org/pdf/1805.03908.pdf)] *
    - Use multi-task learning to enable a time series encoder to learn representations that are useful on data set types with which it has not been trained on. The encoder is formed of a convolutional neural network whose temporal output is summarized by a convolutional attention mechanism
    - 使用多任务学习的方式让时序编码器学习对未接触过的数据集类型有用的表示。本文使用的编码器由卷积神经网络构成，其时间输出由卷积注意机制汇总而成

- **Transfer learning for time series classification** (**IEEE Big Data 2018**) [[paper](https://arxiv.org/pdf/1811.01533.pdf)] [[code](https://github.com/hfawaz/bigdata18)] *
    - Extensive experiments show that transferring the network's weights works on time series classification task, and the choice of the source dataset impacts significantly on the model's generalization capabilities
    - 使用大量实验表明，模型权值的迁移促进其在目标数据集上分类任务的表现，且源数据集的选择对模型的泛化能力有显著影响

#### 2017

- **Time series classification from scratch with deep neural networks: A strong baseline** (**IJCNN17**) [[paper](https://arxiv.org/pdf/1611.06455.pdf)] [[code](https://paperswithcode.com/paper/time-series-classification-from-scratch-with#code)]
    - Propose Fully Convolutional Network (FCN), which can be a strong baseline for similar tasks as one of the earliest deep learning time series classifiers
    - 提出了完全卷积网络（FCN），作为最早的深度学习时间序列分类器之一，它可以作为类似任务的强基准模型

- - -

## Time Series Clustering (时间序列聚类)

Time series clustering is the task of forming clusters given a set of unlabeled time series data.

#### 2019

- **SOM-VAE: Interpretable Discrete Representation Learning on Time Series** (**ICLR19**) [[paper](https://arxiv.org/pdf/1806.02199.pdf)] [[code](https://paperswithcode.com/paper/som-vae-interpretable-discrete-representation)] [[SOM-YouTube](https://www.youtube.com/watch?v=3osKNPyAxPM)]
    - Design SOM-VAE for interpretable discrete representation learning on time series, and show that the latent probabilistic model in the representation learning architecture improves clustering and interpretability of the representations on time series
    - 针对时间序列上的可解释离散表示学习设计了 SOM-VAE，并表明在表示学习体系结构中的潜在概率模型提高了时间序列表示的聚类效果和可解释性

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
    - 提出一种多尺度卷积循环编码器-解码器（MSCRED），对多变量时间序列数据进行异常检测和诊断

- - -

## Sequence Modeling (序列建模)

Specially designed sequence modeling methods can learn the representation of the input time series data, which will be helpful to solve many tasks, e.g. forecasting and classification.

### Supervised Sequence Modeling (监督序列建模)

#### 2018

- **An Empirical Evaluation of Generic Convolutional and Recurrent Networks for Sequence Modeling** [[paper](https://arxiv.org/pdf/1803.01271v2.pdf)] [[code](https://paperswithcode.com/paper/an-empirical-evaluation-of-generic)]
    - Describe a temporal convolutional network (TCN), which contains causal convolutions, dilated convolutions and residual connections
    - 描述了时间卷积网络（TCN），其包含有因果卷积、扩张卷积以及残差连接

- **Multilevel Wavelet Decomposition Network for Interpretable Time Series Analysis** (**KDD18**) [[paper](https://arxiv.org/pdf/1806.08946v1.pdf)] [[code](https://paperswithcode.com/paper/multilevel-wavelet-decomposition-network-for)]
    - Propose a wavelet-based neural network structure called multilevel Wavelet Decomposition Network (mWDN), which preserves the advantage of multilevel discrete wavelet decomposition in frequency learning while enables the fine-tuning of all parameters under a deep neural network framework
    - 提出了一种基于小波的多层次小波分解神经网络结构（mWDN），它既保留了多层次离散小波分解在频率学习中的优势，又能在深度神经网络框架下对所有参数进行微调

### Unsupervised Representation Learning (无监督表示学习)

#### 2019

- **Unsupervised Scalable Representation Learning for Multivariate Time Series** [[paper](https://arxiv.org/pdf/1901.10738v1.pdf)] [[code](https://paperswithcode.com/paper/unsupervised-scalable-representation-learning)]
    - Propose an unsupervised method to learn universal embeddings for variable length and multivariate time series, which combines an encoder based on causal dilated convolutions with a triplet loss employing time-based negative sampling
    - 提出一种无监督学习长度可变和多变量时间序列通用嵌入的方法，它结合了基于因果扩张卷积的编码器与基于时间的负采样的三重损失

- - -

## Time Series Segmentation (时间序列分割)

Time series segmentation is a method of time-series analysis in which an input time-series is divided into a sequence of discrete segments in order to reveal the underlying properties of its source.

- - -

## Study of Stock Market (股票市场研究)

#### 2017

- **Deep Neural-Network Based Stock Trading System Based on Evolutionary Optimized Technical Analysis Parameters** [[paper](https://www.sciencedirect.com/science/article/pii/S1877050917318252)] [[code](https://github.com/omerbsezer/SparkDeepMlpGADow30)]
    - Propose a stock trading system based on technical analysis parameters optimized by genetic algorithms, and the optimized parameters are then passed to a deep MLP neural network as features for buy-sell-hold predictions
    - 提出一种基于遗传算法优化的技术分析指标的股票交易系统，优化后的技术分析指标作为特征被传入深度 MLP 神经网络进行买入-卖出-持有预测

- - -

## Others (其他)

This section contains papers dealing with time series data or applying them to time series tasks, but not appropriate for previous sections.

#### 2019

- **Adversarial Attacks on Time Series** [[paper](https://arxiv.org/pdf/1902.10755v2.pdf)] [[code](https://github.com/houshd/TS_Adv)] *
    - Utilize an adversarial transformation network (ATN) on a distilled model to attack various time series classification models and datasets. Model distillation technique is used to solve the problem that traditional classification model is considered a black-box model with a non-differentiable internal computation
    - 利用基于蒸馏模型的对抗变换网络（ATN）攻击各种时间序列分类模型和数据集。模型蒸馏技术被用于解决传统分类模型被认为是一个内部计算不可微的黑盒模型的问题

- **Data-driven Neural Architecture Learning For Financial Time-series Forecasting** [[paper](http://arxiv.org/abs/1903.06751)]
    - Adapt Heterogeneous Multilayer [Generalized Operational Perceptron](https://www.researchgate.net/publication/318327067_Generalized_model_of_biological_neural_networks_Progressive_operational_perceptrons) (HeMLGOP) algorithm to progressively learn a heterogeneous neural architecture for the given financial time series forecasting problem with imbalanced data distribution problem
    - 采用异构多层[广义操作感知器](https://www.researchgate.net/publication/318327067_Generalized_model_of_biological_neural_networks_Progressive_operational_perceptrons)（HeMLGOP）算法，来逐步学习得到异构神经网络，以解决具有不平衡数据分布的给定财经时序预测问题

#### 2018

- **Recurrent Neural Networks for Multivariate Time Series with Missing Values** (**Scientific Reports 2018**) [[paper](https://www.nature.com/articles/s41598-018-24271-9.pdf)]
    - Propose GRU-D, which utilizes the missing patterns to achieve better prediction results by incorporating two representations of missing patterns, i.e., masking and time interval
    - 提出 GRU-D，其通过结合缺失的 patterns 的两种表示，即掩蔽（masking）和时间间隔（time interval），来获得更好的预测结果