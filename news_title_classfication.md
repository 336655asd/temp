## 数据
- ~~正则表达式过滤文本~~
- ~~标题与内容分开~~ <效果一般>
- ~~正负样本平衡~~


## 模型

- ~~集成学习~~
- ~~将待分类文本丢入BERT中进行futher train训练~~
- 先将中性样本进行二分类，然后再对有情感极性的样本进行二分类。
- 文本标题与内容进行attention


## 降低过拟合
- ~~dropout~~
- ~~normalization~~
- ~~冗余数据~~


## 关于BERT的进一步应用
- ~~将[SEP]引入，考虑title-sep-content~~
- 进一步的想法，利用[SEP]代替'but','and'等转折词


## 文本数据增强
- ~~删除无用字段： 更多精彩，本文来源，本文来自，原标题~~
- UDA 无监督数据增强
- ~~同义词替换~~  <没有外部数据因此较难应用>
- 随机mask一些词语，[MASK]
- 文本顺序交换
- ~~长文本分为前后两部分~~
- ~~中性文本随机插入到非中性文本中~~


## 情感极性强度
- 根据极性强度删除效果无用语句，充分利用512的长度 > 放在验证集和测试集上


## 问题
keras 中的BN在训练frozen的网络时候是坏的 http://blog.datumbox.com/the-batch-normalization-layer-of-keras-is-broken/
<br>   
这个还可以
