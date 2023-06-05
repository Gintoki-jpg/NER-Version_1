## 1.实验任务

实验内容：基于给定的暴雨洪涝中文语料库，利用已人工标注的样本作为训练集和测试集，基于深度学习和预训练模型，编程实现暴雨洪涝中文文本中的发生时间和发生地点两类实体的识别和抽取

实验目标：本实验旨在展示如何使用深度学习模型进行实体抽取任务。实体抽取是自然语言处理中的一个重要任务，其目标是从自然语言文本中识别出特定类型的实体，如人名、地名、组织机构等，并将其标记出来。在实际应用中，实体抽取任务被广泛应用于信息提取、问答系统、机器翻译等领域。

## 2.数据集

本实验使用老师所给的气象文本数据集，该数据集包含暴雨洪涝中文文本及其对应的时间和位置实体标注，详情参考Pycharm目录中的TheNews.pkl文件，或参考实验报告中数据集部分介绍。

## 3.模型

本实验使用了基于深度学习的模型进行实体抽取。具体来说，我们使用了BiLSTM-CRF模型，该模型在自然语言处理领域的实体抽取任务中表现出色。BiLSTM-CRF模型的具体实现细节可参考Pycharm目录中的BiLSTMCRF.py文件.

## 4.依赖

本实验依赖以下Python包：

- PyTorch
- scikit-learn
- numpy
- pandas

更多详细信息可以参考根目录下的enviroment.yml文件，可以使用命令

```shell
conda env create -n simclr -f environment.yml
```

进行环境配置

## 5.如何使用

（1）conda安装虚拟环境并使用conda命令

```shell
conda env create -n simclr -f environment.yml
```

创建对应的虚拟环境，假设这里创建的环境名为tf1，使用

```shell
conda activate tf1
```

激活环境

（2）使用

```shell
cd 
```

进入当前环境目录，使用命令

```shell
python main.py
```

对模型进行训练

（3）训练完毕后使用

```
python main.py test
```

进行测试，测试结果将输出到控制台

## 6.参考文献

- 实体识别抽取综述：[小知识 | 知识图谱：知识抽取之命名实体 (qq.com)](https://mp.weixin.qq.com/s/HJxOZOainC5Dk8SgSbkA9Q)；
- 项目参考：[零基础入门--中文命名实体识别 (qq.com)](https://mp.weixin.qq.com/s/DUxbiVUykVSCLeYxRYd-LA)；