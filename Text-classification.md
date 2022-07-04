<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [分类](#%E5%88%86%E7%B1%BB)
- [多标签分类](#%E5%A4%9A%E6%A0%87%E7%AD%BE%E5%88%86%E7%B1%BB)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->



# 分类

- [6个你应该用用看的用于文本分类的最新开源预训练模型](https://zhuanlan.zhihu.com/p/130792659)
- [从理论到实践解决文本分类中的样本不均衡问题](https://mp.weixin.qq.com/s?__biz=MzU1NjYyODQ4NA==&mid=2247484661&idx=1&sn=8a91b910e941c87fba79a6154c819d66&chksm=fbc36b9eccb4e288c0e37d811b8511c1b093bb664f6442ec9d9e2189d1ea201613da37a3cd33&mpshare=1&scene=24&srcid=0703DjmDK4AfPSuBKxT8gEMH&sharer_sharetime=1625253571562&sharer_shareid=9d627645afe156ff11b0a8519d982bcd&exportkey=A17XMeW6otqsYpmcg5f1gW0%3D&pass_ticket=ahSCjZBnxTVe3IcKWMxBQVeAXXap9Se8HXejNWF3PIlQHiDsRH5Yr1%2FzLdG%2FTkZA&wx_header=0#rd)
  - 数据的采样方法层面，相似样本生成（simbert），loss层面

##少样本
- [文本分类大杀器：PET范式](https://mp.weixin.qq.com/s/qW0iwqWhkj12euEXRenZDg)
  - 使用prompt learning方式进行文本分类
  - 不通pattern对效果有很大影响
  - 构造soft label训练数据+无标签MLM任务
- [少样本文本分类 InductionNet](https://mp.weixin.qq.com/s?__biz=MzI3ODgwODA2MA==&mid=2247502646&idx=4&sn=d1cccfd219b485bf2e5b412d3f08056c&chksm=eb53dfa5dc2456b37657207d86c33758b10884f958909c982ef5926eacd5f08b220fa51536ec&mpshare=1&scene=24&srcid=0527W5ME2Zj4D1bpqs1JhWuZ&sharer_sharetime=1622127690299&sharer_shareid=9d627645afe156ff11b0a8519d982bcd&exportkey=A8UlYy8n%2F03u15ioi5Fk7t8%3D&pass_ticket=ahSCjZBnxTVe3IcKWMxBQVeAXXap9Se8HXejNWF3PIlQHiDsRH5Yr1%2FzLdG%2FTkZA&wx_header=0#rd)


# 多标签分类

- [多标签分类(multi-label classification)综述](https://www.cnblogs.com/cxf-zzj/p/10049613.html)
  - 问题转化方法：分类器链，基于生成的方法，多标签转成单标签
  - 直接建模
- [EMNLP2021论文：元学习大规模多标签文本分类](https://mp.weixin.qq.com/s?__biz=MjM5ODkzMzMwMQ==&mid=2650427439&idx=4&sn=3cb2d0edac444a20d61174d877e661d3&chksm=becdd67589ba5f632533c05ac744d8dffb9d825e99e46fb45b6c9e1f69b0ead11819a3384f06&mpshare=1&scene=24&srcid=1127vW4uT3jw6Xmn9tyxtOeN&sharer_sharetime=1637963151380&sharer_shareid=9d627645afe156ff11b0a8519d982bcd&exportkey=A2REQqlB2R5ChUzrLQzPhuU%3D&pass_ticket=ahSCjZBnxTVe3IcKWMxBQVeAXXap9Se8HXejNWF3PIlQHiDsRH5Yr1%2FzLdG%2FTkZA&wx_header=0#rd)
  - 提出了一种多标签数据的采样策略
- [nn.BCEWithLogitsLoss和nn.MultiLabelSoftMarginLoss有啥区别](https://blog.csdn.net/jiangpeng59/article/details/92016262?utm_medium=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.compare&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-BlogCommendFromMachineLearnPai2-1.compare)
- [标签感知的文档表示用于多标签文本分类（EMNLP 2019）](https://zhuanlan.zhihu.com/p/207221522)
  - 对label的文本表示信息进行embedding
  - 文档self-attention,label-document attention
  - attention fusion, 计算权重后加权
