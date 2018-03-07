# SentimentAnalysis_LSTM
基于Keras使用LSTM对电商评论进行情感分析


## 框架：
- 以词为单位，进行分词，将每个句子截断为MAX_SEQUENCE_LENGTH长度的词（长则截断，不够则补空字符串）
- 将句子以“词-词向量(embedding)”的矩阵形式输入到LSTM模型中进行学习分类
- 模型运行完毕后，使用Keras的预测函数，输入将要预测的词传到函数中进行分类预测


## 说明
- 本次数据来自CCF大赛的情感分析比赛
- 其中content.bin该词向量来自于比赛的数据，进行转换后成为词向量
- 其中代码给了详细的注释
- 由于我们组该比赛最终未采用我的方案，所以读取csv文件自动化预测每个词的功能没有完
>     1. 其中只完成了自动读取csv文件转换为list的功能
>     2. 模型运行时将list传入，运行完毕后，将csv文件转换为list，进行预测，并将预测结果转化为csv文件格式，与原来预测的词一一对应，不过后面这个功能未完成
>     3. 嵌套字典功能代码在这里，并进行详细的讲解：https://github.com/xs-L/NestedDict
- 欢迎大家star


