  **原文链接**：[http://how.bitshares.works/en/master/bts_holders/community_members.html#](http://how.bitshares.works/en/master/bts_holders/community_members.html#)
 
 **译者**：[https://github.com/b-t-s-1](b-t-s-1)
 
 **校对者**： 
  
***    

# 4. 社区成员

目录

* 关于BitShares会员
* BTS持有人
* 委员会
* 见证人
* 工人/预算条目
  - 支付
  - 为BitShares工作
  - 伪工
    + 投票工人
    + 退款工人
    + 销毁工人

## 4.1. 关于BitShares会员

BitShares 2.0将有利于网络的责任和激励活动分开，从而承认不同的技能组合和感兴趣的社区成员有动力以最恰当的方式做出贡献。

* 见证人是为维持骨干网络而获得收入。
* 委员会成员是组织社区并建议网络改变的无偿志愿者。
* 营销人员支付推荐费。
* 工人的报酬和建议都是如此。
* BTS持有人是持有BTS的人。他们可以投票并影响DAC的业务

上述每个（营销人员除外）都要求用户对人员，提案和/或更改进行投票。获得足够批准的人将获得补偿。

工人是“catch all”的群体，如果你对可以改善网络的东西有想法，你就可以通过网络得到“付费”来实现这一目标。组织聚会，为社区开发新工具或功能，以及维护网站和基础设施（例如，mumble服务器团队或Linux发行版）都是工作人员可能做的事情的例子。

## 4.2. BTS持有人

与大多数加密货币相比，BitShares并不是一个货币，而是一个分散的自治公司（DAC)。因此，BitShares的市场估值是自由浮动的，并且可能与任何其他股权（例如传统公司）一样波动。

持有核心代币（BTS）的每个实体都被视为BitShares去中心化公司的BTS持有者。

尽管如此，BTS代币可以用作在金融智能合约（例如市场锚定资产）的抵押，从而支持每个现有的智能货币，例如bitUSD。

## 4.3. 委员会

由于比特币努力就其区块大小达成共识，因此加密货币领域的人们意识到DAC的治理不应该被忽视。因此，BitShares提供了一种工具，可以就业务管理决策达成链上共识。

BitShares区块链具有一组可用的参数，这些参数由BTS Holder批准。 BTS持有人可以定义他们的首选参数集，从而创建一个所谓的委员会成员或者投票给现有的委员会成员。 BitShares委员会由几名active_ committee组成。

BitShares生态系统具有一组可用的参数，这些参数由BTS Holder批准。最初，BitShares具有以下区块链参数：

* **费用结构**: _费用必须由客户支付个人交易_
* **块间隔**: _例如，块间​​隔，块/交易的最大大小_
* **到期参数**: _例如，最大到期时间间隔_
* **见证人参数**: _例如，最大数量的见证人（区块生产者）_
* **委员会参数**: _例如，最多人数的委员会成员_
* **见证人支付**: _每个见证人签名区块的付款_
* **工人预算**: _用于项目的可用预算（例如开发）_

请注意，给定的参数集用作示例，并且网络的参数可能随时间而变化。

除了定义参数之外，任何活跃见证人都可以提出可以由BTS持有者投票（或反对）的协议或业务升级（即硬分叉）。当硬分叉的总票数大于中值见证人权重w时，硬分叉生效。

## 4.4. 见证人

在BitShares中，见证人的工作是收集交易，将它们打包成块，签署块并将其广播到网络。他们基本上是潜在共识机制的区块生产者。

对于每个成功构建的区块，见证人按照股东通过批准投票确定的比率从有限储备池中获得的股份支付。

## 4.5. 工人/预算条目

由于存储在储备池中的资金，BitShares不仅可以为自己的开发和协议改进付费，还可以支持和鼓励生态系统的发展。

### 4.5.1. 支出

区块链参数（由股东通过委员会定义）定义了每日可用预算。在任何时候，所有工人的工资总和都不能超过这个数额。

每日预算分配如下：

* 可用预算从储备池中取出。
* 预算条目按照批准率（Pro-Con）按降序排序。
* 从具有最高批准率的工人开始，支付所要求的每日工资，直到每日预算耗尽为止。
* 支付最低批准率的工人可能会收到低于要求的工资

因此，为了成功地由BitShares生态系统提供资金，BTS持有人对你的预算项目的批准需要得到高排名。

由于来自非流动性储备库的工人付款导致BTS供应增加，这些付款将在股东规定的一段时间内冻结。

### 4.5.2. 为BitShares工作

为了获得BitShares的支付，提案包含

* 工作日期开始，
* 工作日期结束，
* 每日工资（以BTS表示），
* 工人的名字，和
* 互联网地址。

必须在区块链上发布并经股东批准。

工人还可以选择以下属性：

* **归属**: _支付给工人的账户_
* **退款**: _退回到预留池的收益，用于将来的项目_
* **销毁**: _降低工资，从而减少股票供应，相当于公司股票的股份回购_

### 4.5.3. 伪工

存在三种主要不用付工资的伪工人。

#### 4.5.3.1. 投票工人

工人提案可用于股东的民意调查。 这些工人通常没有或很少有工资。 此外，它们还带有提议，建议或其他主题，股东可以在其中发布二元意见（赞成或反对意见）。

#### 4.5.3.2. 退款工人

该工人用于通过简单地将其付款/工资退还到储备池来为工人提案及其支付设置批准限额。 如果其每日工资额与每日可用资金一样大，并且工人在所有工人提案中获得最高批准，则所有资金将返还到储备金，并且不会支付任何人。 但是，如果有其他工人提案
比退款工人更多的选票，提案得到了工资，剩下的退回。

#### 4.5.3.3. 销毁工人

这种类型的工人类似于上面的退款工人，但**销毁**了他的工资。

