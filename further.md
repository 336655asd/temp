# 数据
- 标题与内容分开
- 正负样本平衡


# 模型

- attention


- 将待分类文本丢入BERT中进行mask训练

## 关于BERT的进一步应用
- 将<sep>引入，考虑title-sep-content
- 进一步的想法，利用<sep>代替'but','and'等转折词
