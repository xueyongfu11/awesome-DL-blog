<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [KD](#kd)
  - [bert](#bert)
- [Survey](#survey)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# KD

- [知识蒸馏综述：代码整理](https://mp.weixin.qq.com/s/TbDpGrpsIYG3khsXrazyHw)
- [模型压缩究竟在做什么？我们真的需要模型压缩么？](https://mp.weixin.qq.com/s/u94NZVwb_ywqjTMla2upbQ)
  - paper:Do We Really Need Model Compression?
  - 解释相对直接训练一个小模型，先训练大模型再进行蒸馏到小模型的必要性。直接训练一个小模型可能是非凸的，难以进行优化
  - 训练有素的神经网络存在某种简单性，比如：许多权重接近于0，矩阵是可以低秩分解的，权重可以使用少量的比特来表示，层直接趋向于学习相同的特征
- [「深度学习中知识蒸馏」最新2022研究综述](https://mp.weixin.qq.com/s/2cgUFClQeJ2Jss6adDjUjA)


## bert

- [所有你要知道的 BERT 模型压缩方法，都在这里！](https://mp.weixin.qq.com/s?__biz=MzA5ODEzMjIyMA==&mid=2247495697&idx=3&sn=445b198682cdd7afa9e5b9a105d280af&source=41#wechat_redirect)
- [bert蒸馏瘦身相关的预训练语言模型](https://mp.weixin.qq.com/s/8xNWYJsIDz7j3KW4YyIBKA)
- [4层小模型吊打BERT-large？亚马逊最新瘦身秘籍](https://mp.weixin.qq.com/s/Nt7KJvmL1WnGFgIyhOraBw)
  - 非蒸馏方法，砍掉bert模型的一些层，然后进行精调，但是砍掉不同层，对最终结果的影响很大
  - 模型提出一种最有子结构的搜索方法，然后进行预训练和精调
- [bert模型压缩：量化、剪枝和蒸馏](https://mp.weixin.qq.com/s/6RUvMR-fjzB5PkZBQ4YFNQ)
  - 介绍bert模型各层的参数量及其推理速度
  - bert模型在几种模型压缩方法上的具体操作方法
- [bert家族模型的压缩与蒸馏](https://mp.weixin.qq.com/s/UNHu1eVNorWWKbDb0XBJcA)
  - albert, tinyBert, distilBert等
- [MobileBERT：一种任务无关的模型压缩方法](https://zhuanlan.zhihu.com/p/160833990)
- [NeurIPS 2020 | MiniLM：预训练语言模型通用压缩方法](https://zhuanlan.zhihu.com/p/298390577)


# Survey

- [谷歌、Meta算法工程师给大模型瘦身-书](https://mp.weixin.qq.com/s/ax_SJmQ1SSUn_jutjY1jog)
- [面向大规模神经网络的模型压缩和加速方法](https://mp.weixin.qq.com/s/ZqEJwYt7my2JQwY6yTTwHQ)