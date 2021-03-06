  **原文链接**：[https://dev.bitshares.works/en/master/knowledge_base/wiki_legacy/theoretical_theories.html](https://dev.bitshares.works/en/master/knowledge_base/wiki_legacy/theoretical_theories.html)
 
 **译者**：[https://github.com/b-t-s-1](b-t-s-1)
 
 **校对者**： 
  
***

theoretical theories
===============================

这些是我（@理论）想要讨论的可能特征。 

- 可售/可转让空头头寸

空头头寸应该是自己的对象，可以在账户之间转移。 包括“待售”标志，允许其以一定数量的资产进行原子交易。

NB它类似于房地产市场，由于拥有自己的债务抵押比率，每个空头头寸都是独一无二的。

- 空头“我想进”或“我想出”

在BitAssets 3.0中，应该允许卖空指定一个标志，指示他们是否想要留在（尽可能多）或者是否想要留在外面。 如果一个卖空者想要兑换，他们将被部分承保; 如果一个空头需要，他们将被轻微覆盖。

- 传播期权头寸

长期期权（例如允许你购买）可以与短期权相结合（例如要求你出售），然后你只需提供资金来行使长期权利，而不是提供你可能需要出售的头寸。嗯，这可以通过一系列期权练习创造无限的负荷吗？

- 私有化BitAssets：将资源所有者与资产所有者分开

提供feed很简单，提供资产是一项必须关注特定类型的营销和用户获取的业务。为某些组织提供一种方法，其中唯一的业务是发布Feed，并让其他任何想要负责创建和营销使用该Feed的资产的人。

feed供应商可以拥有自己的品牌，有很多组织在现实世界中发布高度信任的feed，他们可能有兴趣通过将feed放在我们的平台上来实现feed货币化（例如，如果WSJ希望成为feed供应商，那么就有人将能够拥有根据WSJ号码结算的资产.WSJ获得部分费用以换取允许资产使用其品牌）。 从技术上讲，没有办法阻止“剥离”，例如，其他人发布减少费用或免费feed，使得feed等同于WSJ feed，但人们必须相信剥离者始终保持忠诚。 相信WSJ比信任那些承诺永远反映WSJ的随机模糊的商人更容易。 我们将为WSJ提供一种方法来提取高端人士愿意为其品牌的信任付出代价。

- 保证金追缴保费

Arhag在这里提到了优惠保证金追缴保费: https://bitsharestalk.org/index.php/topic,15775.msg202705.html#msg202705

- 兑换请求的市场匹配

尽管我在这里反驳了arhag：https：//bitsharestalk.org/index.php/topic,15775.msg202832.html#msg202832

事实证明，我们实际上可以进行兑换请求的市场匹配。 如果有一方愿意给予他们自愿要求的长期，我们应该通过与对方的匹配来提供他们所要求的长期，而不是强迫短期非自愿地解决。

- 随机赎回时间

兑换订单有可能每个区块执行，而不是在维护块期间兑换。 前24小时的机会是0％（给出了追赶的feed时间），然后根据一些曲线在48小时时逐渐上升到100％（找到一条好的曲线是一个有趣的问题）。
