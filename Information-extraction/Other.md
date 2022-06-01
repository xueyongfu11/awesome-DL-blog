
- [信息抽取新SOTA！首个结构化生成式信息抽取预训练模型，一统信息抽取四大任务](https://zhuanlan.zhihu.com/p/495619962)
  - 区别与生成式模型，而是生成结构化的结果.可是使用多个任务的数据源，有更好的少样本学习泛化能力。
  - 预训练任务：
    - 基于schema的prompt + token sequence -> 结构化的输出
    - encoder无任何输入 -> 结构化的输出，让模型学习固定格式的输出
    - mask language model
  - 微调同预训练任务1